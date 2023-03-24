# 2.L GCD

## The problem
Given two numbers *A* and *B*. Print the greatest common divisor between (*A*, *B*).

Note: The greatest common divisor (GCD) of two or more integers, which are not all zeroes, is the largest positive integer that divides each of the integers.

For example:

the GCD of 8 and 12 is 4.

because the numbers that divides both 8 and 12 are (1,2,4) and 4 is the largest one .

### *input*
Only one line containing two numbers *A* and *B* (1 ≤ *A*, *B* ≤ 10^3).
### *output*
Print the GCD of *A* and *B*.

## Solution

```C++
#include <iostream>
 
using namespace std;
 
int main()
{
        int num1;
        int num2;
        int max;
        int test;
        cin >> num1 >> num2;
        if(num1 == 0){
            cout << num2;
            return 0;
        }else if(num2 == 0){
            cout << num1;
            return 0;
        }else if(num1 == num2){
            cout << num1;
            return 0;
        }
        if(num1 >= num2){
            test = num1;
        }else{
            test = num2;
        }
        for(int i = 1; i < test; i++){
            if((num1 % i == 0) && (num2 % i == 0)){
                if(i >= max){
                    max = i;
                }
            }
        }
        cout << max;
        return 0;
}
```

tags: `C++`  `CPP`  `problem-solving`  `programming`  `coding-challenge`  `interview`
`learn-C++`  `C++-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`
`programming-contest`  `python-coding-challenges`  `python-problem-solving`
