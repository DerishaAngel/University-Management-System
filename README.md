# University-Management-System
To design and implement a simple University Management System using a C++ class with encapsulation, constructors, and destructors, and to demonstrate the object lifecycle. 

program 
#include <iostream>
using namespace std;

class Student
{
private:
    int rollNo;
    string name;

public:
    Student(int r, string n)
    {
        rollNo = r;
        name = n;
        cout << "Student object created" << endl;
    }

    void display()
    {
        cout << "Roll Number: " << rollNo << endl;
        cout << "Name: " << name << endl;
    }

    ~Student()
    {
        cout << "Student object destroyed" << endl;
    }
};

int main()
{
    Student s1(101, "Arun");
    s1.display();
    return 0;
}