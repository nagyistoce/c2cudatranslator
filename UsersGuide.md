# User's Guide #

`C2CUDATranslator` is very easy to use. Users are required to know `C` in advance before using `C2CUDATranslator`.

## B.1 Getting Started ##

### B.1.1 Input and Output of `C2CUDATranslator` ###

```

Input.file - input to translator (C File)
Output.file - output of the translator (CUDA File)
```

First, copy `C` program to `input.file` and run the translator. After running the translator copy `CUDA` code that has been converted or copy content of `output.file`. Put them in `CUDA` project. Run the project.

## B.2 C2CUDATranslator input Details ##

### B.2.1 Kernel Outlining ###

The kernel is the code to be ported on the `GPU`. So, First identify the code you want to run on `GPU`. It may be some computation code such as loops. Now, write `"#pragma kernel_start"` before that code and at the end of the code write `"#pragma kernel_end"`.

**Example**
```

#pragma kernel_start
for (i = 1; i <= 100; ++i)
{
for (j = 0; j < 100; ++j)
{
a [i ] [j ] = b[i ] [j ] + c[i ] [j ];
}
}
#pragma kernel_end
```

### B.2.2 Kernel Variables ###

`Kernel` variables are the variables which are copied to/from  host/devices. User can specify them in their code by writing `"kernel"` in the declaration of that variable.

**Example**
```

int a [100 ] [100 ];
int b [100 ] [100 ];
int c [100 ] [100 ];
```

a,b & c arrays are used in kernel. So, we will write them as
```

kernel int a[100 ] [100 ];
kernel int b[100 ] [100 ];
kernel int c[100 ] [100 ];
```

### B.2.3 Kernel local Variables ###

If there are some local variables in the kernel code, they does not need to be copied to/from host/device. They can be initialized in `GPU`. We can write `"local kernel"` before the declaration statements of them.

**Example**

```

int n=3;
int P=100;
```

n & P are local variables used in kernel region. So, we will write them as
```

local kernel int n=3;
local kernel int P=100;
```



## See Also ##

[Developer's Guide](http://code.google.com/p/c2cudatranslator/wiki/DeveloperGuide)

[Abstract](http://code.google.com/p/c2cudatranslator/wiki/Abstract)

[Thesis Site](https://sites.google.com/a/nirmauni.ac.in/cudacodes/)

[Converted Programs](https://sites.google.com/a/nirmauni.ac.in/cudacodes/ongoing-projects/automatic-conversion-of-source-code-for-c-to-cuda-c/converted-programs)