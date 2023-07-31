```c
int main() {
	FILE* fp = NULL;

	fopen_s(&fp, "test.txt", "r+");

	char data[100];
	
	if (fp == NULL) {
		return 0;
	}

	fgets(data, 100, fp);
	printf("%s", data);

	fclose(fp);

	return 0;
}
```


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
