# malloc-trace
A very library that replaces malloc/calloc/free with trace functions


# Usage
```c
// main.c
#include "malloc_trace.h"   // replace malloc/free/calloc with trace functions
                            // from here on these functions are logged to stdout
                            // NOTE: additionally you must include "malloc_trace.c" to your compile step

int main() {
    int* x = malloc(sizeof(*x));
    free(x);
    return 0
}
```
