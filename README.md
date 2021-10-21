#include <iostream>
using namespace std;
int main()
{
    char name[50];
    int mark;
    cout << "Enter the full name of the Student: ";
    cin.getline(name, 50);
    cout << "Enter the marks (between 0 - 100): ";
    cin >> mark;
    if (mark > 100 || mark < 0) mark = -10;
    switch (mark / 10) {
    case 10:;
    case 9:;
    case 8:cout << "Name: " << name << "\nGrade A\n"; break;
    case 7:cout << "Name: " << name << "\nGrade B\n"; break;
    case 6:cout << "Name: " << name << "\nGrade C\n"; break;
    case 5:cout << "Name: " << name << "\nGrade D\n"; break;
    case 4:cout << "Name: " << name << "\nGrade E\n"; break;
    case 3:;
    case 2:;
    case 1:;
    case 0:cout << "Name: " << name << "\nGrade F\n"; break;
    default: cout << "Invalid marks\n";
    }
    return 0;
}
