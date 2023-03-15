# 2.E Max

## The problem
Given a number N, and N numbers, find maximum number in these N numbers.

### *input*
First line contains a number N (1 ≤ N ≤ 10^3).
### *output*
Second line contains N numbers Xi (0 ≤ Xi ≤ 10^9).

## Solution

```C++
#include <iostream>
 
using namespace std;
 
int main()
{
    int max;
    short int array_length;
    cin >> array_length;
    int arr[array_length];
    for(int i = 0; i < array_length; i++){
        cin >> arr[i];
    }
    for(int i = 0; i < array_length; i++){
        if(arr[i] >= max){
            max = arr[i];
        }else{
            continue;
        }
    }
    cout << max;
    return 0;
}
```

tags: `C++`  `CPP`  `problem-solving`  `programming`  `coding-challenge`  `interview`
`learn-C++`  `C++-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`
`programming-contest`  `python-coding-challenges`  `python-problem-solving`
