#include "main.h"

/**
 * main - tests function that prints if integer is positive or negative
 * Return: 0
 */

int main(void)
{
 	int i;
{
	i = 0;
	positive_or_negative(i);

	return (0);
}

#include <stdio.h>

/**
 * main - causes an infinite loop
 * Return: 0
 */

int main(void)
{
	int i;

	printf("Infinite loop incoming :(\n");

	i = 0;

	/*while (i < 10)*/
	/*{*/
	/*putchar(i);*/
	/*}*/

	printf("Infinite loop avoided! \\o/\n");

	return (0);
}

#include "main.h"

/**
 * largest_number - returns the largest of 3 numbers 
 * @a: first integer
 * @b: second interger
 * @c: third interger
 * Return: largest number
 */

int largest_number(int a, int b, int c)
{
	int largest;

	if (a >= b && a >= c)

	{
		largest = a;
	} 
	else if (b >= a && b >= c)
	{
		largest = b;
	}
	else
	{
		largest = c;
	}

	return (largest);
}

#include <stdio.h>
#include "main.h"

/**
 * print_remaining_days - takes a date and prints how many days are 
 * left in the year, taking leap years into account
 * @month: month in number format
 * @day: day of month
 * @year: year
 * Return: void
 */

void print_remaining_days(int month, int day, int year)
{
	if (year % 4 == 0 || ((year % 100 == 0) && (year % 400 == 0))) 
	{
		day++;
	}

	printf("Day of the year: %d\n", day);
	printf("Remaining days: %d\n", 366 - day);
	}
	else
	{
		if (month == 2 && day == 60)
		{
			printf("Invalid date: %02d/%02d/%04d\n", month, day - 31, year);
		}
		else
		{
			printf("Day of the year: %d\n", day);
			printf("Remaining days: %d\n", 365 - day);
		}
	}
}


