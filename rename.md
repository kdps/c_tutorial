#include <stdio.h>
#include <direct.h>

int main() {
	char strOldFolder[] = "C:\\OldFolder";
	char strNewFolder[] = "C:\\NewFolder";

	mkdir(strOldFolder);
	
	int success = rename(strOldFolder, strNewFolder);

	if (success == 0) {
		printf("이름 변경 성공");
	} else if( success == -1 ) {
		perror("이름 변경 실패");
	}

	return 0;
}
