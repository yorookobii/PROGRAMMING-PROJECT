#include <iostream>
#include <Windows.h>
#include <fstream>
#include <string>

using namespace std;
void login();
void add();
void forgot();
void voucher();
void help();


void gotoxy(int x, int y) {
	COORD coord;
	coord.X = x;
	coord.Y = y;
	SetConsoleCursorPosition(GetStdHandle(STD_OUTPUT_HANDLE), coord);
}



int main()
{
	Sleep(300);
	cout << "888888888888888888888  88888888888888888888   88888888888888888888   888888888888888888888  888888888888888888888888   " << endl;
	Sleep(300);
	cout << "8888            88888  8888            8888   88888888888888888888   8888            88888    88888            88888" << endl;
	Sleep(300);
	cout << "8888          88888    8888           8888    8888            8888   8888          88888       888888           888" << endl;
	Sleep(300);
	cout << "8888        88888      8888          8888     8888            8888   8888        88888           88888           88" << endl;
	Sleep(300);
	cout << "8888     88888         8888        8888       8888            8888   8888     88888               88888           8" << endl;
	Sleep(300);
	cout << "8888 88888             8888       88          8888            8888   8888 88888                     888888" << endl;
	Sleep(300);
	cout << "888888888              8888888888888          8888            8888   888888888                          888888" << endl;
	Sleep(500);
	cout << "8888                   888888   8888          8888            8888   8888                                    88888" << endl;
	Sleep(300);
	cout << "8888                   8888      8888         8888            8888   8888    ------------       888          8888" << endl;
	Sleep(300);
	cout << "8888                   8888        888        8888            8888   8888    -----------         8888            8888" << endl;
	Sleep(300);
	cout << "8888                   8888         888       88888888888888888888   8888    -------                888888       88888" << endl;
	Sleep(300);
	cout << "8888                   8888          8888     88888888888888888888   8888    ----                      888888888888888" << endl;

	cout << "                 ------R          E          S          E          R          V          E------                       " << endl;

	system("pause");
	int  choice;

	system("cls");
	Sleep(300);
	gotoxy(20, 3);
	cout << "---------------------------------------------------------------------------" << endl;
	gotoxy(35, 4);
	cout << " | Press  [1]  to  LOGIN:                       |" << endl;
	gotoxy(35, 5);
	cout << " | Press  [2]  to  ADD:                         |" << endl;
	gotoxy(35, 6);
	cout << " | Press  [3]  to  HELP:                        |" << endl;
	gotoxy(35, 7);
	cout << " | Press  [4]  to  EXIT:                        |" << endl;
	gotoxy(20, 8);
	cout << "---------------------------------------------------------------------------" << endl;
	gotoxy(35, 10);
	cout << "ENTER YOUR CHOICE HERE: " << endl;
	gotoxy(70, 10);
	cin >> choice;
	cout << endl;

	switch (choice)
	{
	case 1:
	{
		 login();

		break;
	}
	case 2:
	{
		 add();

		break;
	}
	case 3:
	{
		help();
		break;
	}
	case 4:
	{
		cout << "Thank you!" << endl;
		break;
	}

	default:
		system("cls");
		cout << "Please Press a valid Number: " << endl;
		break;
	}

	system("pause");
}

void voucher () 
{

	string voucher;

again:
	system("cls");

	gotoxy(22, 5);
	cout << "Please Type -MABUHAY- to claim your 20% off voucher for first time users." << endl;
	gotoxy(40, 7);
	cout << "------------------------------------" << endl;
	gotoxy(40, 8);
	cout << "|                                   |" << endl;
	gotoxy(40, 9);
	cout << "------------------------------------" << endl;
	gotoxy(55, 8);
	cin >> voucher;
	if (voucher == "MABUHAY")
	{

		gotoxy(45, 12);
		cout << "!!! CONGRATULATIONS !!!" << endl;
		Sleep(1000);
		login();
	}
	else
	{
		system("cls");
		gotoxy(16, 5);
		cout << "Please Type -MABUHAY- to claim your FREE VOUCHER " << endl;
		system("pause");
		goto again;

	}

	


}
void add()
{

	string username, pass, address;
	string acc, password;
	int age;
	string claim;

	system("cls");
	gotoxy(16, 5);
	cout << ":ENTER USERNAME:" << endl;
	gotoxy(10, 7);
	cout << "------------------------------------" << endl;
	gotoxy(10, 8);
	cout << "|                                   |" << endl;
	gotoxy(10, 9);
	cout << "------------------------------------" << endl;


	gotoxy(16, 12);
	cout << ":ENTER YOUR PASSWORD:" << endl;
	gotoxy(10, 14);
	cout << "------------------------------------" << endl;
	gotoxy(10, 15);
	cout << "|                                   |" << endl;
	gotoxy(10, 16);
	cout << "------------------------------------" << endl;

	gotoxy(14, 8);
	cin >> username;

	gotoxy(14, 15);
	cin >> pass;

	system("cls");

	gotoxy(15, 5);
	cout << ":ENTER YOUR FULL ADDRESS: " << endl;
	gotoxy(10, 7);
	cout << "------------------------------------" << endl;
	gotoxy(10, 8);
	cout << "|                                   |" << endl;
	gotoxy(10, 9);
	cout << "------------------------------------" << endl;


	gotoxy(17, 12);
	cout << ":ENTER YOUR AGE: " << endl;
	gotoxy(10, 14);
	cout << "------------------------------------" << endl;
	gotoxy(10, 15);
	cout << "|                                   |" << endl;
	gotoxy(10, 16);
	cout << "------------------------------------" << endl;



	gotoxy(12, 8);
	cin >> address;
	gotoxy(12, 15);
	cin >> age;





	system("cls");

again:
	gotoxy(16, 3);
	cout << "LOG IN YOUR ACCOUNT" << endl;
	gotoxy(16, 5);
	cout << "ENTER YOUR USERAME" << endl;
	gotoxy(10, 7);
	cout << "------------------------------------" << endl;
	gotoxy(10, 8);
	cout << "|                                   |" << endl;
	gotoxy(10, 9);
	cout << "------------------------------------" << endl;


	gotoxy(16, 12);
	cout << "ENTER YOUR PASSWORD" << endl;
	gotoxy(10, 14);
	cout << "------------------------------------" << endl;
	gotoxy(10, 15);
	cout << "|                                   |" << endl;
	gotoxy(10, 16);
	cout << "------------------------------------" << endl;


	gotoxy(14, 8);
	cin >> acc;
	gotoxy(14, 15);
	cin >> password;

	cout << endl;

	if (acc != username)
	{
		system("cls");
		gotoxy(16, 12);
		cout << "!!! ERROR !!! " << endl;
		Sleep(1000);
		goto again;

	}
	else if (pass != password)
	{
		system("cls");
		gotoxy(16, 12);
		cout << "!!! ERROR !!! " << endl;
		Sleep(1000);
		goto again;

	}

	else {
		Sleep(1000);
		voucher();
	}



}

void help()
{
	system("cls");


	int help, help1;
	cout << "[1] ABOUT THE PROGRAM:      " << endl;	
	cout << "[3] ABOUT THE AUTHOR        " << endl;
	cout << "[3] HOW TO USE THE PROGRAM: " << endl;

	cin >> help;

	if (help == 1)
	{
		system("cls");
		
		cout << "----------------------------------------------------------------------------------------------------------------------" << endl;
		cout << "|                                                                                                                    |" << endl;
		cout << "|                                                                                                                    |" << endl;
		cout << "|                                                                                                                    |" << endl;
		cout << "|                                                                                                                    |" << endl;
		cout << "|                                                                                                                    |" << endl;
		cout << "|                                                                                                                    |" << endl;
		cout << "|                                                                                                                    |" << endl;
		cout << "|                                                                                                                    |" << endl;
		cout << "|                                                                                                                    |" << endl;
		cout << "|                                                                                                                    |" << endl;
		cout << "|                                                                                                                    |" << endl;
		cout << "|                                                                                                                    |" << endl;
		cout << "----------------------------------------------------------------------------------------------------------------------" << endl;

		gotoxy(22, 5);
		cout << "The purpose of our innovative prop reservation program is to seamlessly bridge" << endl;
		gotoxy(22, 6);
		cout << "the rich traditions of folkdance with the fast - paced world of technology." << endl;
		gotoxy(22, 7);
		cout << "By offering an efficient and user-friendly platform. We aim to empower dancers " << endl;
		gotoxy(22, 8);
		cout << "and event organizers to effortlessly preserve and share cultural heritage" << endl;
		gotoxy(22, 9);
		cout << "              	    with PROPS - RESERVE. " << endl;

		cout << endl;
	again:

		cout << "[1] MAIN MENU :" << endl;
		cout << "[2] EXIT      :" << endl;
		cin >> help1;


		if (help1 == 1)
		{
			system("cls");
			main();
		}


		else if (help1 == 2)
		{
			int exit;
			cout << "ARE YOU SURE YOU WANT TO EXIT" << endl;
			cout << "[1] YES  ||  [2] NO " << endl;

			cin >> exit;

			if (exit == 1)
			{
				cout << "Thank you" << endl;
			}
			else if (exit == 2)
			{
				goto again;
			}



		}



	}
	else if (help == 2)
	{
		system("cls");
		cout << "The Author of this program is Mr. John Jesrylle C. Balatbat                                                                                        " << endl;
		cout << "His undying passion about Folk Dance led him in making an innovative program like this                                                             " << endl;
		cout << "He is a BSIT studen in Bulacan State University Hagonoy Campus and an Active Folk dancer for almost 5 years                                        " << endl;
		cout << "He is the past president of Hiyas ng Hagonoy Folkloric Group and Currently member of Lahing Kayumanggi Dance Troupe In Bulacan State University.   " << endl;


	}

	else if (help == 3)
	{
		system("cls");
		cout << "If using SPACE try using DASH (-) instead to avoid erorr." << endl;
	}

}

	
void forgot() {
	cout << "stoopid ass brain";
}


void login() {

	system("cls");

	Sleep(300);
	cout << "888888888888888888888  88888888888888888888   88888888888888888888   888888888888888888888  888888888888888888888888   " << endl;
	Sleep(300);
	cout << "8888            88888  8888            8888   88888888888888888888   8888            88888    88888            88888" << endl;
	Sleep(300);
	cout << "8888          88888    8888           8888    8888            8888   8888          88888       888888           888" << endl;
	Sleep(300);
	cout << "8888        88888      8888          8888     8888            8888   8888        88888           88888           88" << endl;
	Sleep(300);
	cout << "8888     88888         8888        8888       8888            8888   8888     88888               88888           8" << endl;
	Sleep(300);
	cout << "8888 88888             8888       88          8888            8888   8888 88888                     888888" << endl;
	Sleep(300);
	cout << "888888888              8888888888888          8888            8888   888888888                          888888" << endl;
	Sleep(500);
	cout << "8888                   888888   8888          8888            8888   8888                                    88888" << endl;
	Sleep(300);
	cout << "8888                   8888      8888         8888            8888   8888    ------------       888          8888" << endl;
	Sleep(300);
	cout << "8888                   8888        888        8888            8888   8888    -----------         8888            8888" << endl;
	Sleep(300);
	cout << "8888                   8888         888       88888888888888888888   8888    -------                888888       88888" << endl;
	Sleep(300);
	cout << "8888                   8888          8888     88888888888888888888   8888    ----                      888888888888888" << endl;

	cout << "                 ------R          E          S          E          R          V          E------                       " << endl;

	cout << "\t\t\t\t\t----WELCOME TO PROPS-RESERVE----" << endl;
	cout << "\t\t\t\tTraditions Unveiled: Folkdance Prop Reservations" << endl;

	int choice2;

again:
	Sleep(2000);
	system("cls");
	cout << "SET = 2 PIECES     ||     PIECE = 1 PIECE " << endl;
	gotoxy(55, 4);
	cout << "AVAILABLE PROPS: " << endl;

	gotoxy(35, 6);
	cout << "[1] TINIKLING BAMBOO : 150 Pesos Per Set   : " << endl;
	gotoxy(35, 7);
	cout << "[2] SUBLI HAT        : 30  Pesos Per Piece : " << endl;
	gotoxy(35, 8);
	cout << "[3] CASTANETS        : 30  Pesos Per Set   : " << endl;
	gotoxy(35, 9);
	cout << "[4] KALATONG STICKS  : 50  Pesos Per Set   : " << endl;
	gotoxy(35, 10);
	cout << "[5] FESTIVAL FLAGS   : 20  Pesos Per Piece : " << endl;
	gotoxy(35, 11);
	cout << "[6] E     X    I    T                        " << endl;

	gotoxy(37, 14);
	cout << "------------------------------------" << endl;
	gotoxy(37, 15);
	cout << "|                                   |" << endl;
	gotoxy(37, 16);
	cout << "------------------------------------" << endl;
	gotoxy(40, 15);
	cin >> choice2;	



	switch (choice2)
	{
	case 1: 

	{	
		double total, sub, quantity, subtotal;
		int vouch; // used choice in voucher.

		gotoxy(37, 22);
		cout << "PLEASE ENTER THE QUANTITY OF SET:    ";
		cin >> quantity;
		
		total = quantity * 150;
		gotoxy(37, 24);
		cout << "THE TOTAL AMOUNT IS: " << total << endl;

		Sleep(1000);
		gotoxy(37, 22);
		cout << "DO YOU WANT TO USE YOUR VOUCHER? " << endl;
		gotoxy(37, 23);
		cout << "PRESS THE NUMBER OF YOUR CHOICE " << endl;
		gotoxy(37, 24);
		cout << "[1] YES || [2] NO     ";
		cin >> vouch;

		if (vouch == 1)
		{
		sub = (20 * total) / 100;
		subtotal = total- sub;

			cout << "THE DISCOUNTED PRICE OF YOUR ORDER IS: " << subtotal << endl;
			break;
		}

		
		
	}

	case 2:
	{
	
		double total, sub, quantity, subtotal;
		int vouch; // used choice in voucher.
		gotoxy(37, 22);
		cout << "PLEASE ENTER THE QUANTITY OF SET: " << endl;
		cin >> quantity;


		total = quantity * 30;
		gotoxy(37, 24);
		cout << "THE TOTAL AMOUNT IS: " << total << endl;
		Sleep(1000);
		gotoxy(37, 22);
		cout << "DO YOU WANT TO USE YOUR VOUCHER? " << endl;
		gotoxy(37, 23);
		cout << "PRESS THE NUMBER OF YOUR CHOICE " << endl;
		gotoxy(37, 24);
		cout << "[1] YES || [2] NO     ";
		cin >> vouch;					

		if (vouch == 1)
		{
			sub = (20 * total) / 100;
			subtotal = total - sub;

			cout << "THE DISCOUNTED PRICE OF YOUR ORDER IS: " << subtotal << endl;
			break;
		}
	
	}
	case 3:
	{
		double total, sub, quantity, subtotal;
		int vouch; // used choice in voucher.

		gotoxy(37, 22);
		cout << "PLEASE ENTER THE QUANTITY OF SET: " << endl;
		cin >> quantity;


		total = quantity * 30;
		gotoxy(37, 24);
		cout << "THE TOTAL AMOUNT IS: " << total << endl;

		Sleep(1000);
		gotoxy(37, 22);
		cout << "DO YOU WANT TO USE YOUR VOUCHER? " << endl;
		gotoxy(37, 23);
		cout << "PRESS THE NUMBER OF YOUR CHOICE " << endl;
		gotoxy(37, 24);
		cout << "[1] YES || [2] NO     ";
		cin >> vouch;

		if (vouch == 1)
		{
			sub = (20 * total) / 100;
			subtotal = total - sub;

			cout << "THE DISCOUNTED PRICE OF YOUR ORDER IS: " << subtotal << endl;
			break;
		}
	}
	case 4:
	{
		double total, sub, quantity, subtotal;
		int vouch; // used choice in voucher.

		gotoxy(37, 24);
		cout << "PLEASE ENTER THE QUANTITY OF SET: " << endl;
		cin >> quantity;
		gotoxy(45, 24);

		total = quantity * 40;
		gotoxy(37, 22);
		cout << "THE TOTAL AMOUNT IS: " << total << endl;

		Sleep(1000);
		gotoxy(37, 22);
		cout << "DO YOU WANT TO USE YOUR VOUCHER? " << endl;
		gotoxy(37, 23);
		cout << "PRESS THE NUMBER OF YOUR CHOICE " << endl;
		gotoxy(37, 24);
		cout << "[1] YES || [2] NO     ";
		cin >> vouch;


		if (vouch == 1)
		{
			sub = (20 * total) / 100;
			subtotal = total - sub;

			cout << "THE DISCOUNTED PRICE OF YOUR ORDER IS: " << subtotal << endl;
			break;
		}
	}

	case 5:
	{
		double total, sub, quantity, subtotal;
		int vouch; // used choice in voucher.
		gotoxy(37, 22);
		cout << "PLEASE ENTER THE QUANTITY OF SET: " << endl;
		cin >> quantity;

	

		total = quantity * 20;

		cout << "THE TOTAL AMOUNT IS: " << total << endl;

		Sleep(1000);
		gotoxy(37, 22);
		cout << "DO YOU WANT TO USE YOUR VOUCHER? " << endl;
		gotoxy(37, 23);
		cout << "PRESS THE NUMBER OF YOUR CHOICE " << endl;
		gotoxy(37, 24);
		cout << "[1] YES || [2] NO     ";
		cin >> vouch;

		if (vouch == 1)
		{
			sub = (20 * total) / 100;
			subtotal = total - sub;

			cout << "THE DISCOUNTED PRICE OF YOUR ORDER IS: " << subtotal << endl;
			break;
		}
	}
	default:
		break;
	}

}

