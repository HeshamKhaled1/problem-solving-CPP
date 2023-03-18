# 2.H One Prime

## The problem
Given a number X. Determine if the number is prime or not

Note:

A prime number is a number that is greater than 1 and has only two factors which are 1 and itself.

In other words : prime number divisible only by 1 and itself.

Be careful that 1 is not prime .

### *input*
Only one line containing a number X (2 ≤ X ≤ 10^5).
### *output*
print "YES" if the number is prime and "NO" otherwise.

## Solution

```C++
#include <iostream>
 
using namespace std;
 
int main()
{
    int num;
    cin >> num;
    bool isPrime = true;
    for(int i = 2; i <= num/2; i++){
        if(num % i == 0){
            isPrime = false;
        }
    }
    if(isPrime == true){
        cout << "YES";
    }else{
        cout << "NO";
    }
    return 0;
}
```

tags: `C++`  `CPP`  `problem-solving`  `programming`  `coding-challenge`  `interview`
`learn-C++`  `C++-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`
`programming-contest`  `python-coding-challenges`  `python-problem-solving`
