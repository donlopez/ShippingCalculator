#include <iostream>
#include <iomanip>

using namespace std;

int milesToSegment(int a);

double twopounds(int b, double c);

double twoToSixpounds(int d, double e);

double sixToTenpounds(int f, double g);

int main()
{
    int miles = 0, quit = 1, multiple, remainder;
     
    double weight = 0.0, cost = 0.0;

    cout << fixed << showpoint << setprecision(2);

    while (quit == 1)
    {
        do
        {

        cout << "Enter the number of Miles as a whole number: ";
        cin >> miles;
        cout << endl;

        milesToSegment(miles);

        }

        while (miles <= 0);

        while (weight <= 0)
        {
            cout << "Enter the Weight of the package in pounds: ";
            cin >> weight;
            cout << endl;

            if (weight <= 0)
            {
                cout << "Error: Weight must be greater than zero!\n" << endl;
            }
            
            else if (weight > 10)
            {
                cout << "Error: We don't ship packages over 10 pounds!\n" << endl;
                weight = 0.0;
            }

        }

        if (weight <= 2)
        {
            cost = twopounds(miles, weight);
            cout << "The cost to ship your package is: $" << cost << endl;
        }

        else if (weight > 2 && weight <= 6)
        {
            cost = twoToSixpounds(miles, weight);
            cout << "The cost to ship your package is: $" << cost << endl;
        }

        else
        {
            cost = sixToTenpounds(miles, weight);
            cout << "The cost to ship your package is: $" << cost << endl;
        }

        cout << "\nEnter 1 to continue or 0 to quit: ";
		cin >> quit;
        cout << endl;

		if (quit == 0) 
            {
				cout << "Good-bye!\n" << endl;
            }
           
        weight = 0.0;
		miles = 0;
		multiple = 0;
		remainder = 0;

    }

    return 0;
}

double sixToTenpounds(int f, double g)
{
    double price3;
    int multiple3, remainder3;
    
    multiple3 = f / 500;
    remainder3 = f % 500;

    if (remainder3 > 0)
		remainder3 = 1;

	if (g > 6 && g <=10)
    {
        price3 = 5.25 * (multiple3 + remainder3);
    }
    return price3; 
}

double twoToSixpounds(int d, double e)
{
    double price2;
    int multiple2, remainder2;
    
    multiple2 = d / 500;
    remainder2 = d % 500;

    if (remainder2 > 0)
		remainder2 = 1;

	if (e > 2 && e <= 6)
    {
        price2 = 3.70 * (multiple2 + remainder2);
    }
    return price2; 
    
}

double twopounds(int b, double c)
{
    double price1;
    int multiple1, remainder1;
    
    multiple1 = b / 500;
    remainder1 = b % 500;

    if (remainder1 > 0)
		remainder1 = 1;

	if (c <= 2) 
    {
        price1 = 1.50 * (multiple1 + remainder1);
    }

    return price1;
}

int milesToSegment(int a)
{
    int miles;

    while (a <= 0)
    {
        cout << "Error: Miles must be greater than zero!\n" << endl;
        return a;
    }
    
    return miles;
    
}
