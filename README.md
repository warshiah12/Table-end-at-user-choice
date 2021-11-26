# Table-end-at-user-choice
#For loop
#include<iostream>
#include<conio.h>
using namespace std;
int main()
{
	int table, e;     //declaring variables with datatype integer
	cout << "Table of and should end at: "<<endl;    
	cin >> table >> e;

	while (cin.fail() != 0)  
	{
		cin.clear();
		cin.ignore(1000, '\n');
		cout << "Incorrect command. First enter the number you want the table of and then enter the number where it should end:  "<<endl;
		cin >> table>>e;
	}
	cout << "Table of " << table << endl;
	for (int k = 1; k <= e; k++)  //using for loop
	{
		cout << "\n" << table << " X " << k << " = " << table * k << endl;  //displaying the table on the console screen
	}
	return 0;
}
