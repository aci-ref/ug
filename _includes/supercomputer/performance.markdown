
### Capability vs capacity
Supercomputers generally aim for the maximum in capability computing rather 
than capacity computing. Capability computing is typically thought of as using 
the maximum computing power to solve a single large problem in the shortest 
amount of time. Often a capability system is able to solve a problem of a size 
or complexity that no other computer can, e.g. a very complex weather 
simulation application.

Capacity computing in contrast is typically thought of as using efficient 
cost-effective computing power to solve a small number of somewhat large 
problems or a large number of small problems, e.g. many user access requests to 
a database or a web site. Architectures that lend themselves to supporting many 
users for routine everyday tasks may have a lot of capacity but are not 
typically considered supercomputers, given that they do not solve a single very 
complex problem.

### Performance metrics

In general, the speed of supercomputers is measured and benchmarked in "FLOPS" 
(FLoating Point Operations Per Second), and not in terms of MIPS, i.e. as 
"instructions per second", as is the case with general purpose computers. These 
measurements are commonly used with an SI prefix such as tera-, combined into 
the shorthand "TFLOPS" (10<sup>12</sup> FLOPS, pronounced teraflops), or peta-, 
combined into the shorthand "PFLOPS" (10<sup>15</sup> FLOPS, pronounced 
petaflops.) "Petascale" supercomputers can process one quadrillion 
(10<sup>15</sup>) (1000 trillion) FLOPS. Exascale is computing performance in 
the exaflops range. An exaflop is one quintillion (10<sup>18</sup>) FLOPS (one 
million teraflops).

No single number can reflect the overall performance of a computer system, yet 
the goal of the Linpack benchmark is to approximate how fast the computer 
solves numerical problems and it is widely used in the industry. The FLOPS 
measurement is either quoted based on the theoretical floating point 
performance of a processor (derived from manufacturer's processor 
specifications and shown as *Rpeak* in the TOP500 lists) which is generally 
unachievable when running real workloads, or the achievable throughput, derived 
from the LINPACK benchmarks and shown as *Rmax* in the TOP500 list. The LINPACK 
benchmark typically performs LU decomposition of a large matrix. The LINPACK 
performance gives some indication of performance for some real-world problems, 
but does not necessarily match the processing requirements of many other 
supercomputer workloads, which for example may require more memory bandwidth, 
or may require better integer computing performance, or may need a high 
performance I/O system to achieve high levels of performance.

### The TOP500 list


![Pie chart showing share of supercomputers by countries from top 500 
supercomputers as of November 2013](top500_countries.png)

Since 1993, the fastest supercomputers have been ranked on the [TOP500 list](http://top500.org) 
according to their LINPACK benchmark results. The list does not claim to be 
unbiased or definitive, but it is a widely cited current definition of the 
"fastest" supercomputer available at any given time.

This is a recent list of the computers which appeared at the top of the TOP500 
list, and the "Peak speed" is given as the "Rmax" rating.


Year | Supercomputer | Peak speed (Rmax) | Location
-----|---------------|-------------------|---------
2013 | NUDT Tianhe-2 | 33.86 PFLOPS | Guangzhou, China
2012 | Cray Titan | 17.59 PFLOPS | Oak Ridge, USA
2012 | IBM Sequoia | 17.17 PFLOPS | Livermore, USA
2011 | Fujitsu K computer | 10.51 PFLOPS | Kobe, Japan
2010 | Tianhe-IA | 2.566 PFLOPS | Tianjin, China
2009 | Cray Jaguar | 1.759 PFLOPS | Oak Ridge, USA
2008 | IBM Roadrunner | 1.026 PFLOPS | Los Alamos, USA
2013 | IIoTM Prithvi | 0.790 PFLOPS | Pune, India

