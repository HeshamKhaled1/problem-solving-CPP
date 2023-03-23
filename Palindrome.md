# 2.I Palindrome

## The problem
Given a number N. Print 2 lines that contain the following respectively:

1. Print N in a reversed order and not leading zeroes.

2. If N is a palindrome number print "YES" otherwise, print "NO.

Note:

A palindrome number is a number that reads the same forward or backward.

For example: 12321, 101 are palindrome numbers, while 1201, 221 are not.

A leading zero is any 0 digit that comes before the first nonzero digit in a number for example : numbers (005 , 01 , 0123 , 02 , 000250 ) are leading zeroes but ( 5 , 123 , 20 ,2500 ) not leading zeroes numbers .

### *input*
Only one line containing a number N (1≤N≤10^7).
### *output*
Print the answer required above.

## Solution

```C++
#include <iostream>
using namespace std;
 
int main()
{
    int num;
    int res;
    int final_res = 0;
    cin >> num;
    int test = num;
    while(test != 0){
        res = test % 10;
        final_res *= 10;
        final_res += res;
        if(res == 0){
            test /= 10;
            continue;
        }else{
            test /= 10;
        }
    }
    cout << final_res << endl;
    if(num == final_res){
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
