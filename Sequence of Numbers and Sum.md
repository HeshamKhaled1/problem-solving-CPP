# 2.R Sequence of Numbers and Sum

## The problem
Given multiple lines each line contains two numbers *N* and *M*.

For each line print a single line contains:

* The numbers between *N* and *M* inclusive separated by single space.
* The message " sum =".
* The summation of all numbers between *N* and *M* inclusive.
Note: The program should be TERMINATED as soon as any of these two numbers is less than or equal to zero and don't print any thing.

### *input*
The input contains multiple line.

Each line contains two numbers *N* and *M* (-100 ≤ *N*, *M* ≤ 100).

It's guaranteed that the last line of the input will contain a number that is less than or equal to zero.
### *output*
For each line print the answer according to the required above in a single line.

## Solution

```C++
#include <iostream>
 
using namespace std;
 
int main()
{
    int num1;
    int num2;
    int tc = 100;
    while(tc != 0){
        cin >> num1 >> num2;
        if(num1 < num2){
            int i;
            int res = 0;
            for(i = num1; i <= num2; i++){
            if((num1 <= 0) || (num2 <= 0)){
                return 0;
            }
            res += i;
            cout << i << " ";
            }
            cout << "sum =" << res;
        }else{
            int i;
            int res = 0;
            for(i = num2; i <= num1; i++){
            if((num1 <= 0) || (num2 <= 0)){
                return 0;
            }
            res += i;
            cout << i << " ";
            }
            cout << "sum =" << res;
        }
 
        cout << endl;
        tc--;
    }
    return 0;
}
```

tags: `C++`  `CPP`  `problem-solving`  `programming`  `coding-challenge`  `interview`
`learn-C++`  `C++-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`
`programming-contest`  `python-coding-challenges`  `python-problem-solving`
