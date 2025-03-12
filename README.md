# c-8
Program to reverse a string
#include<stdio.h>
#include<string.h>
int main()
{
    char str[30],temp;
    int i,length;
    printf("enter the name");
    scanf("%s",str);
    length=strlen(str);
    for(i=0;i<length/2;i++)
    {
        temp=str[i];
        str[i]=str[length-i-1];
        str[length-i-1]=temp;
    }
    printf("reversed string %s",str);
     return 0;
}
