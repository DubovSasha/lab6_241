# lab6_241
// task2
#include <locale.h>
#include <stdio.h>
#include <math.h>
#define _USE_MATH_DEFINES

int main()
{
	setlocale(LC_ALL, "RUS");
	float res;
	int x;
	// res = 1/(pow(x,2)+1)
	puts("Введите значение x");
	scanf("%x", &x);
	res = x <= -3 ? 9 : (1 / (pow(x, 2) + 1));
	printf("Вы ввели значение x: %x \n Ответ на задачу: %.3f ", x, res);
	

}
// task3
