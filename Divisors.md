# 2.K Divisors

## The problem
Given a number N. Print all the divisors of N in ascending order.

### *input*
Only one line containing a number N (1 ≤ N ≤ 10^4).
### *output*
Print all positive divisors of N, one number per line.

## Solution

```C++
#include <iostream>
 
using namespace std;
 
int main()
{
    int num;
    cin >> num;
    for(int i = 1; i <= num; i++){
        if(num % i == 0){
            cout << i << endl;
        }
    }
    return 0;
}
```

tags: `C++`  `CPP`  `problem-solving`  `programming`  `coding-challenge`  `interview`
`learn-C++`  `C++-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`
`programming-contest`  `python-coding-challenges`  `python-problem-solving`
