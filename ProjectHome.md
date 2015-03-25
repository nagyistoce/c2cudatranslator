# Automatic conversion of source code for C to CUDA C #
**Project Type  :** [M.Tech. `Thesis`](https://sites.google.com/a/nirmauni.ac.in/cudacodes/)<br />
**Student Name  :** Parth R.Trivedi<br />
**Guide Name    :** Dr. S. N. Pradhan<br />
**Roll No       :** 10MCEC25<br />
**College       :** Institute of Technology<br />
**University    :** [Nirma University](http://www.nirmauni.ac.in/), _INDIA_<br />

## _Abstract_ ##
**As today in so many fields, computation is the main part of the algorithm and takes too much time in execution of the algorithm, it is necessary to parallelize the computation or reduce execution time. **`GPU`**s are widely used in **`(HPC) High Performance Computing`**.
To achieve speedup, either we can increase clock frequency or multiple computation cores on the same chip. The clock speeds have reached the physical limit, so the use of many cores is the only way left to achieve speedup. As the **`GPU`** is growing demand of the Game Industry and large scientific computations, efforts have been made to take advantages to gain maximum utilization of the **GPU\*s in computation. Though**`GPU`**s are widely used in**Supercomputers**today, they are not code transparent because one has to sit and code the algorithms in**`CUDA C`**to run them on**`GPU`**. So if we can have some**middle ware**that converts the**`C`**programs to**`CUDA`**, the end user gets**transparency_._

I tried to develop a prototype compiler using**`ANTLR`**in visual studio that converts the**`C`**programs in**`CUDA C`**language. The thesis describes the literature survey in**`CUDA`**, different performance optimization strategies to reduce execution time, the Pattern approach to develop a translator for source code to source code translation on the basis of selection of codes using patterns, platforms to code such translator and platform comparison and choice and algorithm of translation. The Compiler Architecture and its implementation details are widely described in thesis. The thesis describes implementation of the complete**`C2CUDATranslator`**, testing and analysis of the developed compiler. The compiler takes input of**`C`**program and generates**`CUDA`**program. The thesis demonstrates the pattern approach for language to language translation and the compiler flow architecture.**`C2CUDAranslator`**covers a new way or a framework to implement new analysis algorithms to detect dependencies in the code. The thesis also covers neural network design for compiler learning and optimization of the translated code. The Neural Network helps compiler to take decision for selection of transformation and translation.
Finally, the thesis covers outcome of the compiler, converted programs list, evaluation using parboil benchmark suite, performance graph of converted programs. It is concluded that** the `C2CUDATranslator` saves 95% of the development time in selected cases._`C2CUDATranslator` converts `C` code to `CUDA`. It is also a framework to develop analysis and dependency checking algorithms for other developers._




## See Also ##

[Abstract](http://code.google.com/p/c2cudatranslator/wiki/Abstract)

[Developer's Guide](http://code.google.com/p/c2cudatranslator/wiki/DeveloperGuide)

[User's Guide](http://code.google.com/p/c2cudatranslator/wiki/UsersGuide)

[Thesis Site](https://sites.google.com/a/nirmauni.ac.in/cudacodes/)

[Converted Programs](https://sites.google.com/a/nirmauni.ac.in/cudacodes/ongoing-projects/automatic-conversion-of-source-code-for-c-to-cuda-c/converted-programs)