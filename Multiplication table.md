# 2.F Multiplication table

## The problem
Given a number N. Print the maltiplication table of the number from 1 to 12

### *input*
Only one line containing a number N (1 ≤ N ≤ 50).
### *output*
Print 12 lines according to the required above.

## Solution

```C++
#include <iostream>
 
using namespace std;
 
int main()
{
    short int num;
    cin >> num;
    for(int i = 1; i <= 12; i++){
        cout << num << " * "<< i << " = " << (num * i) << endl;
    }
    return 0;
}
```

tags: `C++`  `CPP`  `problem-solving`  `programming`  `coding-challenge`  `interview`
`learn-C++`  `C++-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`
`programming-contest`  `python-coding-challenges`  `python-problem-solving`
