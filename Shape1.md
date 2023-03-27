# 2.P Shape1

## The problem
Given a number *N*. Print a face down right angled triangle that has *N* rows.

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
    int num;
    cin >> num;
    for(int i = num; i >= 1; i--){
        for(int j = 1; j <= i; j++){
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
