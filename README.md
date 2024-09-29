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
#include <locale.h>
#include <stdio.h>
#include <math.h>
#include <stdlib.h>
#define _USE_MATH_DEFINES

int main()
{
	/*Дано число N (N<1000). Написать программу, которая по запросу
    пользователя выведет последнюю или первую цифру введенного числа.*/
	setlocale(LC_ALL, "RUS");
	
	float reg,res,x;
	int a, b;
	puts("Введите значение от 0  до  1000");
	scanf("%f", &x);
	system("pause");


	if (x >  1000) puts("Ошибка! Вы ввели значение от 1000");
	else
	{
		if (x < 10)
		{
			printf("Вы ввели однозначное число %i ",(int)x);
		}
			else
			{
				if ((x >= 10 ) && (x < 100))
				{
					puts("Если хотите вывести первую цифру введите - 1 , а если последнюю - 0");
					scanf("%i", &a);
					res = a == 1 ? ((int)x / 10) : (((int)x) % 10);
					printf(" Ваша выбранная цифра: %i", (int)res);
				}
					else
					{
						
						puts("Если хотите вывести первую цифру введите - 2 , а если последнюю - 3");
						scanf("%i", &b);
						reg = b == 2 ? ((int)x / 100) : ((int)x % 10);
						printf(" Ваша выбранная цифра: %i", (int)reg);
					}
			}
	}
		
	

}
