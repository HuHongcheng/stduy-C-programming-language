# stduy-C-programming-language


#define _CRT_SECURE_NO_WARNINGS 1


#include<stdio.h>
#include<string.h>

//结构体和指针--------------
int x = 0;
struct Book
{
	char name[30];
	short price;
	short number;
};
int main()
{
	struct Book A1 = { "大学英语",100,23 };
	printf("书名:%s\n", A1.name);
	printf("价格:%d\n", A1.price);
	printf("编号%d\n", A1.number);
	struct Book*pb=&A1;
	printf("%p\n", pb);//指针
	A1.price = 50;
	printf("打折后的价钱:%d\n", A1.price);
	strcpy(A1.name, "修改后的名字");
	printf("修改后的名字:%s\n", A1.name);
	return 0;
}
