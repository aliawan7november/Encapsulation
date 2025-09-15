#include <iostream>
using namespace std;

// Encapsulation Example
class Student {
private:
    string name;   // private variable
    int age;       // private variable

public:
    // Setter for name
    void setName(string n) {
        name = n;
    }

    // Getter for name
    string getName() {
        return name;
    }

    // Setter for age
    void setAge(int a) {
        if (a > 0)   // validation example
            age = a;
        else
            cout << "Age must be positive!" << endl;
    }

    // Getter for age
    int getAge() {
        return age;
    }
};

int main() {
    Student s1;

    // setting values using setters
    s1.setName("Ali");
    s1.setAge(20);

    // accessing values using getters
    cout << "Name: " << s1.getName() << endl;
    cout << "Age: " << s1.getAge() << endl;

    return 0;
}
