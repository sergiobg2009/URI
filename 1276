# URI
UriOnlineJudge

#include<stdio.h>
#include<stdlib.h>
 
int main(){
    int i,j,*alfabeto,inicio,fim,flag;
    char s[100];
 
    while(gets(s)){
        i=flag=0;
        alfabeto = (int*)calloc(26,sizeof(int));
        while(s[i] != '\0'){
            alfabeto[ s[i] - 97 ] = 1;
            i++;
        }
        inicio=fim=j=0;
        while(j < 26){
            if(alfabeto[j] == 1){
                inicio = j;
                while(alfabeto[j] == 1 && j < 26){
                    j++;
                }
                if(flag == 0){
                    printf("%c:%c",inicio+97, j+97-1);
                    flag=1;
                }else{
                    printf(", %c:%c",inicio+97, j+97-1);
                }
            }else{
                j++;
            }
        }
        puts("");
    }
    return 0;
}
