# 2.V PUM

## The problem
Given a number N. Print N lines that describes PUM game.

### *input*
Only one line containing a number *N* (1 ≤ *N* ≤ 20).
### *output*
Print the answer according to the required above.

## Solution

```C++
#include <iostream>
 
using namespace std;
 
int main()
{
    short num;
    cin >> num;
    int test = 1;
    for(int i = 0; i < num; i++){
        for(int j = 1; j <= 4; j++){
            if(j == 4){
                cout << "PUM";
                test++;
                break;
            }
            cout << test << " ";
            test++;
        }
        cout << endl;
    }
    return 0;
}
```

tags: `C++`  `CPP`  `problem-solving`  `programming`  `coding-challenge`  `interview`
`learn-C++`  `C++-tutorial`  `programming-exercises`  `programming-challenges`  `programming-fundamentals`
`programming-contest`  `python-coding-challenges`  `python-problem-solving`
