# Practical-4-4-2-
#include <iostream>
#include <string>
using namespace std;

string max(string a, string z) {
    return (a > z) ? a : z;
}
string max(string a, string z, string b) {
    return max(max(a, z), b);
}
int main() {
    string str1, str2, str3;
    cout << "Enter Three strings: ";
    cin >> str1 >> str2 >> str3;
    cout << "Maximum string is: " << max(str1, str2, str3) << endl;
    return 0;
}
