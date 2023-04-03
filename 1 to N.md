# 2.A 1 to N

## The problem
Given a number *N*. Print numbers from 1 to *N* in separate lines.

### *input*
Only one line containing a number N (1 ≤ *N* ≤ 10^3).
### *output*
Print *N* lines according to the required above.

## Solution

```C++
#include <iostream>

using namespace std;

int main()
{
    int num;
    cin >> num;
    for(int i = 1; i <= num; i++){
        cout << i << endl;
    }
    return 0;
}
```

tags: `C++`  `CPP`  `problem-solving`  `programming`  `coding-challenge`  `interview`
`learn-C++`  `C++-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`
`programming-contest`  `python-coding-challenges`  `python-problem-solving`
