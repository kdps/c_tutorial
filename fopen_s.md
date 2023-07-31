```c
#include <stdio.h>

int main() {
	FILE* fp = NULL;

	fopen_s(&fp, "test.txt", "w");

	if (fp != NULL) {
		fputs("TEST", fp);
		fclose(fp);
	}

	return 0;
}
```
