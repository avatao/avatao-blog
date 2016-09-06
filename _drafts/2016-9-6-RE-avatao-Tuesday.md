---
layout: post
title: RCE avatao Tuesday
author: gabor
author_name: "Gabor Pek"
author_web: "http://www.crysys.hu/~pek/"
---
So here we are again with your next avatao Tuesday challenge. Today, we are delving a bit into reverse engineering by providing a small tutorial and a challenge to solve. 


<!--excerpt-->

A decent definition for reverse engineering comes from Eldad Eilam from  his [Reversing: Secrets of Reverse Engineering](http://eu.wiley.com/WileyCDA/WileyTitle/productCd-0764574817.html) book: "In the software world reverse engineering boils down to taking an existing program for which source-code or proper documentation is not available and attempting to recover details regarding its’ design and implementation." 

You can easily grasp the idea behind this definition if you write a simple C program, compile and disassemble it. For simplicity, we are going to create a simple Linux [ELF](https://en.wikipedia.org/wiki/Executable_and_Linkable_Format) binary with [GCC](https://gcc.gnu.org/)

So here is your first source code:

```c
#include <stdio.h>

int main()
{
    printf("Hello avatao Tudesday\n");
    return 0;
}

```

Let's create a 32-bit binary from this source code:

```
gcc -m32 -o re_challenge re_challenge.c
```

If you prefer 64 bit simply use `-m64`
```
gcc -m64 -o re_challenge re_challenge.c
```

There are various disassemblers available online in demo version (e.g., [IDA](https://www.hex-rays.com/products/ida/), [Binary Ninja](https://binary.ninja/demo.html)) or entirely free (e.g., [radare2](https://github.com/radare/radare2))


In this tutorial, we are going to use IDA to dissect our [32-bit binary](../downloads/re_tuesday).

If we simply open the binary in IDA you will see something similar:


[re_challenge](../images/re_challenge.png)

The compiled binary contains instructions that can be executed by the CPU directly. The language which makes these machine instructions readable for humans is called [Assembly](https://en.wikipedia.org/wiki/Assembly_language). That is what we generally work with during reverse engineering. 


For more information a really nice beginner's guide from Dennis Yurichev is available [online](https://github.com/dennis714/RE-for-beginners)


**All right, lhere is yout [second avatao Tuesday challenge](https://platform.avatao.com/challenges/82aced6a-baa8-4380-a553-a14ca304283d)**