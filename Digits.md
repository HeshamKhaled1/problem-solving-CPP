# 2.Q Digits

## The problem
Given a number *N*. Print the digits of that number from right to left separated by space.

### *input*
First line contains a number *T* (1 ≤ *T* ≤ 10) number of test cases.

Next *T* lines will contain a number *N* (0 ≤ *N* ≤ 10^9)
### *output*
For each test case print a single line contains the digits of the number separated by space.

## Solution

```C++
#include <iostream>
 
using namespace std;
 
int main()
{
    int tc;
    long long num;
    cin >> tc;
    while(tc--){
        cin >> num;
        if(num == 0){
            cout << 0;
        }
        while(num != 0){
            cout << num % 10 << " ";
            num /= 10;
        }
        cout << endl;
    }
    return 0;
}
```

tags: `C++`  `CPP`  `problem-solving`  `programming`  `coding-challenge`  `interview`
`learn-C++`  `C++-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`
`programming-contest`  `python-coding-challenges`  `python-problem-solving`
