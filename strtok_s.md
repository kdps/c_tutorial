```c
#include <stdio.h>
#include <string.h>
#include <stdlib.h>

int main() {
	char str[] = "there#is#no#sponnn";
	char delim[] = "#";
	char* token, * context;

	token = strtok_s(str, delim, &context);

	while (token != NULL) {
		printf("%s : %d\n", token, strlen(token));
		token = strtok_s(NULL, delim, &context);
	}

	return 0;
}
```
