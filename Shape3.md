# 2.W Shape3

## The problem
Given a number *N*. Print a diamond that has 2*N* rows.

### *input*
Only one line containing number N (1 ≤ N ≤ 99).
### *output*
Print the answer according to the required above.

## Solution

```C++
#include <iostream>
 
using namespace std;
 
int main()
{
    short rows;
    cin >> rows;
    int test = 1;
    for(int i = 1; i <= rows; i++){
        for(int k = 1; k <= rows-i; k++){
            cout << " ";
        }
        for(int cols = 0; cols < (i * 2)-1; cols++){
            cout << "*";
        }
        cout << endl;
    }
    for(int i = rows; i >= 1; i--){
        for(int k = rows - i; k > 0; k--){
            cout << " ";
        }
        for(int cols = 0; cols < (i * 2)-1; cols++){
            cout << "*";
        }
        cout << endl;
    }
    return 0;
}
```

tags: `C++`  `CPP`  `problem-solving`  `programming`  `coding-challenge`  `interview`
`learn-C++`  `C++-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`
`programming-contest`  `python-coding-challenges`  `python-problem-solving`
