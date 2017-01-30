#include<stdio.h>
#include<conio.h>
void showMenu();
float avgGDP();
float findMin();
float findDiff();
float highIn();
float find2Max();
float inpercent();
void main(void)
{
	char userinput;
	do {
		showMenu();
		userinput = _getch();
		switch (userinput)
		{
		case'a':
		case'A':
			avgGDP();
			break;
		case'b':
		case'B':
			findMin();
			break;
		case'c':
		case'C':
			findDiff();
			break;
		case'd':
		case'D':
			highIn();
			break;
		case 'e':
		case'E':
			find2Max();
			break;
		/*case 'f':
		case'F':
			F();
			break;*/
		case'q':
		case'Q':
			userinput = 'Q';
			break;
		default:
			printf("You have entered an invaild entry. Please try again");

		}

	} while (userinput != 'Q');
}
