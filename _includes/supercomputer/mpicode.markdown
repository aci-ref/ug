
The following MPI example shows an implementation of `MPI_Bcast`
in $$\mathcal{O}\left(\log n\right)$$ time.

{% highlight cpp %}
#include <stdio.h>
#include <mpi.h>

void bcast(void *message,
           int count,
           MPI_Datatype datatype,
           int root,
           MPI_Comm comm)
{
   int size, rank;
   int distance;
   MPI_Status stat;

   if(root != 0) {
      fprintf(stderr, "Root process for bcast must be 0.\n");
      MPI_Abort(comm, 0);
   }

   MPI_Comm_size(comm, &size);
   MPI_Comm_rank(comm, &rank);

   if(size & (size - 1)) {
      fprintf(stderr, "Process group size must be a power of 2.\n");
      MPI_Abort(comm, 0);
   }

   distance = 1;
   while(distance <= size / 2) {
      if(rank < distance) {
         MPI_Send(message, count, datatype, rank + distance, TAG_BCAST, comm);
      }
      else if(rank < 2 * distance) {
         MPI_Recv(message, count, datatype, rank - distance, TAG_BCAST, comm, &stat);
      }
      distance *= 2;
   }
}

{% endhighlight %}


*[MPI]: Message passing interface
