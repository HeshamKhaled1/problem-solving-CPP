# 2.N Numbers Histogram

## The problem
Given 3 lines of input described as follow:

1. First line contains a symbol *S*

2. Second line contains a number *N*

3. Third line contains *N* numbers
For each number *Xi* in the *N* numbers print a new line that contains the symbol *S* repeated *Xi* time.

### *input*
The first line contains a symbol *S* can be (+,−,∗,/)

The second line an number *N* (1≤*N*≤50)

The third line contains *N* numbers (1≤*Xi*≤100)
### *output*
Print the answer required above.

## Solution

```C++
#include <iostream>
 
using namespace std;
 
int main()
{
    char s;
    int tc;
    int num;
    cin >> s;
    cin >> tc;
    switch(s){
        case '+' :
            while(tc--){
                cin >> num;
                for(int i = 0; i < num; i++){
                    cout << '+';
                }
                cout << endl;
            }
            break;
        case '-' :
            while(tc--){
                cin >> num;
                for(int i = 0; i < num; i++){
                    cout << '-';
                }
            cout << endl;
            }
            break;
        case '*' :
            while(tc--){
                cin >> num;
                for(int i = 0; i < num; i++){
                    cout << '*';
                }
            cout << endl;
            }
            break;
        case '/' :
            while(tc--){
                cin >> num;
                for(int i = 0; i < num; i++){
                    cout << '/';
                }
            cout << endl;
            }
            break;
    }
    return 0;
}
```

tags: `C++`  `CPP`  `problem-solving`  `programming`  `coding-challenge`  `interview`
`learn-C++`  `C++-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`
`programming-contest`  `python-coding-challenges`  `python-problem-solving`
