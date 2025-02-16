# konstructivno-laba1
using namespace std;
#include <iostream>
#include <windows.h>
int main(){
    SetConsoleCP(1251);
    SetConsoleOutputCP(1251);
    int n,d,t;
    cout << "Введите кол-во проверок: "; cin >> t;
     for (int i = 0; i < t; i++) {    //проверка
       //код
        cout << "Введите факториал: "; cin >> n;
        cout << "Введите цифру: "; cin >> d;
        cout << 1 << " ";
        if (n >= 3  d % 3 == 0)
            cout << 3 << " ";        
        if (d == 5) 
            cout << 5 << " ";        
        if (n >= 3  d == 7) 
            cout << 7 << " ";
        if ((n >= 3 && d % 3 == 0) || n >= 6) 
            cout << 9;
        cout << endl;
     }
}
