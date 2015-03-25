# Developer's Guide #

`C2CUDATranslator` is very easy to work with. Developers are required to know `C`, `CUDA C` in detail in advance before using <span><code>C2CUDATranslator</code></span>. Additionally they are required to know `ANTLR` compulsory.

## C.1 Getting Started ##

C2CUDATranslaor is like a framework to develop and test various code analysis algorithms in the field of source code to source code translation.

### C.1.1 C2CUDATranslator Project Structure ###

The design of the project is shown below. Developers can see the Visual Studio 2008 Solution project as given design on project website.

http://sites.google.com/a/nirmauni.ac.in/a/nirmauni.ac.in/cudacodes

## C.2 C2CUDATranslator development Details ##

### C.2.1 Analysis Framework ###

In C2CUDATranslator there is a file "Analysis.cs" which contains analysis algorithms. One can write his/her own algorithm in this file as a class or new function and can call in the parser. But the namespace must be C2CUDAranslator.Analysis.

### C.2.2 Translation Framework ###

Similarly, `C2CUDATranslator.Translation` is the framework that contains classes and codes for translation. Developers will find `FOR`, `BLOCK` etc. classes. They may contain properties like `LOOP.index`, `LOOP.IsNestLoop` etc.

### C.2.3 Use framework ###

Developers can use collections those contains read-only, write-only variables and can use them in conditions in making analysis algorithms.



## See Also ##

[User's Guide](http://code.google.com/p/c2cudatranslator/wiki/UsersGuide)

[Abstract](http://code.google.com/p/c2cudatranslator/wiki/Abstract)

[Thesis Site](https://sites.google.com/a/nirmauni.ac.in/cudacodes/)

[Converted Programs](https://sites.google.com/a/nirmauni.ac.in/cudacodes/ongoing-projects/automatic-conversion-of-source-code-for-c-to-cuda-c/converted-programs)