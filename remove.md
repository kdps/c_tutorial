#include <stdio.h>

int main() {
	char strPath[] = { "D:\\Text2.txt" };
	
	int success = remove( strPath );

	if (success == 0) {
   printf("파일 삭제 성공");
	} else if(success == -1) {
		perror("파일 삭제 실패");
	}
 
  return 0;
}
