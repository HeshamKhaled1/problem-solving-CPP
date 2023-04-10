# 2.T Shape2

## The problem
Given a number N. Print a pyramid that has N rows.

For more clarification see the example below.

### *input*
Only one line containing a number N (1 ≤ N ≤ 99).
### *output*
Print the answer according to the required above.

## Solution

```C++
#include <iostream>
 
using namespace std;
 
int main()
{
    int tc;
    cin >> tc;
 
    for(int i = 1; i <= tc; i++){
        for(int j = 1; j <= tc-i; j++){
            cout << " ";
        }
        for(int k = 0; k < (i*2-1); k++){
                    cout << '*';
        }
        cout << endl;
    }
    return 0;
}
```

tags: `C++`  `CPP`  `problem-solving`  `programming`  `coding-challenge`  `interview`
`learn-C++`  `C++-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`
`programming-contest`  `python-coding-challenges`  `python-problem-solving`
