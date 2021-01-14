# alphabets-only
Write a function which accepts a string as an argument and returns  a modified string containing only the English alphabets from the  string. 


#include <iostream>
#include <string>
using namespace std;

string stringchecker(string a){
    int length = a.length();
    string n;
    for(int i=0; i<length; i++){
        int c = a[i];
        if(c>=65 && c<=90 || c>= 97 && c<= 122){
            n += a[i];
        }
    }
    return n;
}

int main(){

    string s;
    cout<< "Enter your string: ";
    getline(cin,s);
    cout << stringchecker(s);
    return 0;
}
