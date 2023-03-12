/* Ria Labbe | IT312 | 03/12/23 | 2-1 Using Operators to Calculate GPA and Honors
* GPAnHonoursCalculator.cpp : This file contains the 'main' function. Program execution begins and ends there.
* 
* This app is broken down into two portions, one which evaluates the input grade chars into doubles, and the main function which utilises the new doubles
* in order to calculate the GPA for the student, this is calculated through the totalGradePoints divided by 4. This is then tested against a system of booleans 
*which outputs which level of honours or lack thereof which the student resides in.
*/

#include <iostream>
using namespace std;

//Function which converts Letter grade into double format for GPA calculations
double gpaLetterToDouble(char gradeInput) {
    if (gradeInput == 'A' || gradeInput == 'a') {
        return 4.0;
    }
    else if (gradeInput == 'B' || gradeInput == 'b') {
        return 3.0;
    }
    else if (gradeInput == 'C' || gradeInput == 'c') {
        return 2.0;
    }
    else if (gradeInput == 'D' || gradeInput == 'd') {
        return 1.0;
    }
    else { //Encompasses F Grade
        return 0.0;
    }
}
    //arg count and arg vector allow for command line input
int main(int argc, char* arg[])
{
    //Initalise Variables, setting Variables to 0.0 where appropriate
    double totalGradePoints = 0.0, 
        studentOverallGPA = 0.0;
    char inputGrade1, inputGrade2, inputGrade3, inputGrade4;

    cout << "Input your first grade (A,B,C,D, or F):" << endl;
    cin >> inputGrade1;
    totalGradePoints += gpaLetterToDouble(inputGrade1);

    cout << "Input your second grade (A,B,C,D, or F):" << endl;
    cin >> inputGrade2;
    totalGradePoints += gpaLetterToDouble(inputGrade2);

    cout << "Input your third grade (A,B,C,D, or F):" << endl;
    cin >> inputGrade3;
    totalGradePoints += gpaLetterToDouble(inputGrade3);

    cout << "Input your fourth grade (A,B,C,D, or F):" << endl;
    cin >> inputGrade4;
    totalGradePoints += gpaLetterToDouble(inputGrade4);

    //Calcluates the GPA for the student which can be used to check against Honours system
    studentOverallGPA = totalGradePoints / 4.0;
    cout << "Student GPA is: " << studentOverallGPA << endl;

    //Boolean set which allows for Honours system output

    bool summaCumLaude = studentOverallGPA >= 4.0;
    bool magnaCumLaude = studentOverallGPA >= 3.8 && studentOverallGPA < 3.9;
    bool cumLaude = studentOverallGPA >= 3.65 && studentOverallGPA < 3.8;
    bool withoutHonours = studentOverallGPA < 3.65;

    //Utilising documentation, the use of Bool Alpha allows me to print true/false based on bool system above

    cout << "Graduating Summa Cum Laude is:" << boolalpha << summaCumLaude << endl;
    cout << "Graduating Magna Cum Laude is:" << boolalpha << magnaCumLaude << endl;
    cout << "Graduating Cum Laude is:" << boolalpha << cumLaude << endl;
    cout << "Graduating without Honours is:" << boolalpha << withoutHonours << endl;

    return 0;

}


