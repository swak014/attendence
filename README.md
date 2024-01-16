#include<iostream>
using namespace std;

int main()
{
    int totalClasses, attendedClasses;

    cout << "Enter the total number of classes: ";
    cin >> totalClasses;

    cout << "Enter the number of classes attended: ";
    cin >> attendedClasses;

    if (attendedClasses > totalClasses)
        {

        cout << "Error: Number of attended classes cannot be greater than total classes." << endl;
        return 1;

       }

    // Calculate attendance percentage
    double attendancePercentage = (static_cast<double>(attendedClasses) / totalClasses) * 100;

    // Display the attendance percentage
    cout << "Attendance Percentage: " << attendancePercentage << "%" << endl;

    return 0;
}
