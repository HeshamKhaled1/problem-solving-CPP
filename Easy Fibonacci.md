# 2.Y Easy Fibonacci

## The problem
Given a number *N*. Print first *N* numbers of the Fibonacci sequence.

Note: In order to create the Fibonacci sequence use the following function:

* fib(1) = 0.
* fib(2) = 1.
* fib(n) = fib(n - 1) + fib(n - 2).

### *input*
Only one line containing a number *N* (1 ≤ *N* ≤ 45).
### *output*
Print the first *N* numbers from the Fibonacci Sequence .

## Solution

```C++
#include <iostream>
 
using namespace std;
 
int main()
{
    int num;
    cin >> num;
    int first_term = 0;
    int second_term = 1;
    int next_term;
    for(int i = 1; i <= num; i++){
        if(i == 1){
            cout << first_term << " ";
            continue;
        }else if(i == 2){
            cout << second_term << " ";
            continue;
        }
        next_term = first_term + second_term;
        first_term = second_term;
        second_term = next_term;
        cout << next_term << " ";
    }
    return 0;
}
```

tags: `C++`  `CPP`  `problem-solving`  `programming`  `coding-challenge`  `interview`
`learn-C++`  `C++-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`
`programming-contest`  `python-coding-challenges`  `python-problem-solving`
