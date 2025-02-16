using namespace std;
#include <iostream>
int main() {
    int t;
    cin >> t;
    int* arr = new int[t * 2];
    for (int i = 0; i < t * 2; i+=2) {        
        cin >> arr[i];
        cin >> arr[i+1];
    }
    cout << endl;
    for (int i = 0; i < t * 2; i += 2) {
        cout << 1 << " ";
        if (arr[i] >= 3 || arr[i+1] % 3 == 0)
            cout << 3 << " ";
        if (arr[i+1] == 5)
            cout << 5 << " ";
        if (arr[i] >= 3 || arr[i+1] == 7)
            cout << 7 << " ";
        if ((arr[i] >= 3 && arr[i+1] % 3 == 0) || arr[i] >= 6)
            cout << 9;
        cout << endl;
    }
}
