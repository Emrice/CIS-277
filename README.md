# CIS - 277
/*
Class: CIS-277-001
Professor: Alan Eliscu
Date: 9/17/2018
Name: Marlen Herrera
*/

#include <iostream>
#include <stdlib.h>
#include <string>
using namespace std;

//Structure for flight passenger.
struct flyer{
		string name;
		int ticket;
		int flyer;
		double price;
		char flightNumber[6];
		char seat[6];
		int month;
		int date;
		int year;
		};

int main ()
{
	//struct variable
	flyer passenger;

	//user inputting passenger information
	cout << "Enter passenger name (Format: First, Last): ";
	getline(cin, (passenger.name));

	cout << "Enter ticket number (Format: 123456): ";
	cin >> passenger.ticket;

	cout << "Enter frequent flyer number (Format: 1234): ";
	cin >> passenger.flyer;

	cout << "Enter ticket price (Format: 100.00): ";
	cin >> passenger.price;

	cout << "Enter flight number (Format: AH123): ";
	cin >> passenger.flightNumber;

	cout << "Enter seat number (Format: A1): ";
	cin >> passenger.seat;

	cout << "Enter flight date (Format: 01 01 2001): ";
	cin >> passenger.month >> passenger.date >> passenger.year;

	cout << endl << endl << endl;

	//Outputting information that was entered
	cout << "Passenger Name: " << passenger.name << endl;
	cout << "Ticket Number: " << passenger.ticket << endl;
	cout << "Frequent Flyer: " << passenger.flyer << endl;
	cout << "Ticket Price: $" << passenger.price << endl;
	cout << "Flight Number: " << passenger.flightNumber << endl;
	cout << "Seat Number: " << passenger.seat << endl;
	cout << "Flight Date: " << passenger.month << "/" << passenger.date << "/" << passenger.year << endl;


	system("pause");
    return 0;
}
