# 2.S Sum of Consecutive Odd Numbers

## The problem
Given two numbers *X* and *Y*. Print the sum of all odd numbers between them, excluding *X* and *Y*.

### *input*
First line contains a number *T* (1 ≤ *T* ≤ 10) number of test cases.

Next *T* lines will contain two numbers *X* and *Y* (0 ≤ *X*, *Y* ≤ 10^4).
### *output*
Print the sum of all odd numbers between *X* and *Y* (excluding *X* and *Y*).

## Solution

```C++
#include <iostream>
 
using namespace std;
 
int main()
{
    short tc; //it's not exceeds 10
    int num1;
    int num2;
    cin >> tc;
    while(tc--){
        cin >> num1 >> num2;
        int result =0;
        if(num1 < num2){
            for(int i = num1+1; i < num2; i++){
                if(i%2 == 0){
                    continue;
                }else{
                    result += i;
                }
            }
            cout << result;
        }else{
            for(int i = num2+1; i < num1; i++){
                if(i%2 == 0){
                    continue;
                }else{
                    result += i;
                }
            }
            cout << result;
        }
        cout << endl;
    }
    return 0;
}
```

tags: `C++`  `CPP`  `problem-solving`  `programming`  `coding-challenge`  `interview`
`learn-C++`  `C++-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`
`programming-contest`  `python-coding-challenges`  `python-problem-solving`
