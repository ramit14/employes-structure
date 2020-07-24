# employes-structure
Develooed by Ramit Bhanawat.
#include <iostream> 

using namespace std; 

  

struct employee { 

    string ename; 

    int age, phn_no; 

    int salary; 
}; 

void display(struct employee emp[], int n) 
{ 

    cout << "Name\tAge\tPhone Number\tSalary\n"; 

    for (int i = 0; i < n; i++) { 

        cout << emp[i].ename << "\t" << emp[i].age << "\t"

             << emp[i].phn_no << "\t" << emp[i].salary << "\n"; 

    } 
}

int main() 
{ 

    int n = 3; 

    // Array of structure objects 

    struct employee emp[n]; 

  

    // Details of employee 1 

    emp[0].ename = "ramit"; 

    emp[0].age = 18; 

    emp[0].phn_no = 1234567788; 

    emp[0].salary = 2000000; 

  

    // Details of employee 2 

    emp[1].ename = "rachit"; 

    emp[1].age = 21; 

    emp[1].phn_no = 1234567891; 

    emp[1].salary = 5600000; 

  

    // Details of employee 3 

    emp[2].ename = "renit"; 

    emp[2].age = 12; 

    emp[2].phn_no = 1100661111; 

    emp[2].salary = 3050000; 

  

    display(emp, n); 

  

    return 0; 
} 
