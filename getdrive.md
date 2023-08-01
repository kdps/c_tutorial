```c
#include <stdio.h>
#include <direct.h>

int main() {
	int drive = 0;

	drive = _getdrive();

	printf("%c", char(drive)+96);

	return 0;
}
```
