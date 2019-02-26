# ice_cream
Calculate the how much ice cream you sold and how much you made selling them
// computes the number of each cone type sold that day, and then computes and displays a daily sales  
// Celestino Martinez
// INCLUDE ANY NEEDED FILES HERE.
using namespace std;

#include <iostream>
#include <string>
#include <iomanip>

int main()
{  
   // DEFINE NAMED CONSTANTS HERE TO HOLD THE PRICES OF THE 3 
   // SIZES OF ICE CREAM CONES. GIVE EACH ONE A DESCRIPTIVE
   // NAME AND AN APPROPRIATE DATA TYPE. 
	double DeLIGHTful = 1.49,
		   double_DeLIGHTful = 2.49,
		   triple_DeLIGHTful = 3.49;

   // DECLARE ALL NEEDED VARIABLES HERE. GIVE EACH ONE A DESCRIPTIVE
   // NAME AND AN APPROPRIATE DATA TYPE. 
	int total_scoop,
		number_of_single_scoop,
		number_of_double_scoop,
		number_of_triple_scoop;

	double pause,
		   total_price,
		   DeLightful_single_price,
		   DeLightful_double_price,
		   DeLightful_triple_price;
   
   // WRITE STATEMENTS HERE TO PROMPT FOR AND INPUT THE INFORMATION
   // THE PROGRAM NEEDS TO GET FROM THE USER.
	cout << "Number of single scoop cones sold: ";
	cin >> number_of_single_scoop;
	cout << "Number of double scoop cones sold: ";
	cin >> number_of_double_scoop;
	cout << "Number of triple scoop cones sold: " ;
	cin >> number_of_triple_scoop;
	cout << endl;

   
   // WRITE STATEMENTS HERE TO PERFORM ALL NEEDED COMPUTATIONS  
   // AND ASSIGN THE RESULTS TO VARIABLES.
	total_scoop = number_of_single_scoop + number_of_double_scoop + number_of_triple_scoop;
	DeLightful_single_price = static_cast<double> (number_of_single_scoop) * DeLIGHTful; 
	DeLightful_double_price = static_cast<double>(number_of_double_scoop) * double_DeLIGHTful; 
	DeLightful_triple_price = static_cast<double>(number_of_triple_scoop) * triple_DeLIGHTful;
	total_price = DeLightful_single_price + DeLightful_double_price + DeLightful_triple_price;
   
   // WRITE STATEMENTS HERE TO DISPLAY THE REQUESTED INFORMATION.
	cout<< setprecision(7);
    cout<<"DeLIGHTful cones " << setw(10) << number_of_single_scoop << " " << "$ " << setw(7) <<DeLightful_single_price << endl;
    cout<<"doube DeLIGHTful cones " << setw(4) << number_of_double_scoop << " " << "$ " << setw(7) <<DeLightful_double_price << endl;
    cout<<"triple DeLIGHTful cones " << setw(3) << number_of_triple_scoop << " " << "$ " << setw(7) <<DeLightful_triple_price << endl;
    cout<<"Total " << setw(21) << total_scoop << " "<< "$ "<< setw(7) <<total_price << endl;

    cout << "Pause " << endl;
    cin >> pause;



   return 0;
}
