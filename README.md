## Assembly Stack Frame

A simple javascript snippet that illustrates the stack frame during a C function call.

The frame sequences are screenshoots from the [GDB](https://www.gnu.org/software/gdb/) debugger.

### The complete C source

```c
#include <stdio.h>

int add(int a, int b) {
	int c;
	c = a + b;
	return c;
}

int main(int argc, char argv**) {
	int a = 1;
	int b = 2;
	int usm = add(a + b);
	return 0;
}
```

### Run the project
[https://wiredolphin.github.io/app/assembly_stack_frame/index.html](https://wiredolphin.github.io/app/assembly_stack_frame/index.html)
