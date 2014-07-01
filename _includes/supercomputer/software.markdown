
### Operating systems
Since the end of the 20th century, supercomputer operating systems have 
undergone major transformations, based on the changes in supercomputer 
architecture. While early operating systems were custom tailored to each 
supercomputer to gain speed, the trend has been to move away from in-house 
operating systems to the adaptation of generic software such as Linux.

Since modern massively parallel supercomputers typically separate computations 
from other services by using multiple types of nodes, they usually run 
different operating systems on different nodes, e.g. using a small and 
efficient lightweight kernel such as CNK or CNL on compute nodes, but a larger 
system such as a Linux-derivative on server and I/O nodes.

While in a traditional multi-user computer system job scheduling is in effect a 
tasking problem for processing and peripheral resources, in a massively 
parallel system, the job management system needs to manage the allocation of 
both computational and communication resources, as well as gracefully dealing 
with inevitable hardware failures when tens of thousands of processors are 
present.

Although most modern supercomputers use the Linux operating system, each 
manufacturer has its own specific Linux-derivative, and no industry standard 
exists, partly due to the fact that the differences in hardware architectures 
require changes to optimize the operating system to each hardware design.

### Software tools and message passing

The parallel architectures of supercomputers often dictate the use of special 
programming techniques to exploit their speed. Software tools for distributed 
processing include standard APIs such as MPI and PVM, VTL, and open 
source-based software solutions such as Beowulf.

In the most common scenario, environments such as PVM and MPI for loosely 
connected clusters and OpenMP for tightly coordinated shared memory machines 
are used. Significant effort is required to optimize an algorithm for the 
interconnect characteristics of the machine it will be run on; the aim is to 
prevent any of the CPUs from wasting time waiting on data from other nodes. 
GPGPUs have hundreds of processor cores and are programmed using programming 
models such as CUDA.

Moreover, it is quite difficult to debug and test parallel programs. Special 
techniques need to be used for testing and debugging such applications.
