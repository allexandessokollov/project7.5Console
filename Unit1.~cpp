#pragma hdrstop
//--------------------------------------------------------------------------

#include <iostream.h>
#include <stdio.h>
#include <conio.h>
#pragma argsused

const int MAX_STRING_SIZE = 512;


int findAmount(char chArr[]);
bool isOdd(int num);

int findQuantOfSequences(char chArr[]);

int main()
{
    int answer;
    char chArr[MAX_STRING_SIZE];

    printf("Enter your string\n");

    gets(chArr);

    answer = findAmount(chArr);

    printf("\nAnswer is: %d ", answer);

    puts("\n\n\nPress any key ... ");
    getch();
    getch();

    return 0;
}
int findAmount(char chArr[])
{
    int arrSize = strlen(chArr);
    int tempSumm = 0;
    int answer = 0;
    int counter = 0;

    for(int i = 0; i < arrSize; i++)
    {
        if(chArr[i] == '1' || chArr[i] == '0'){
            counter++;
            if(chArr[i] == '1'){
                  tempSumm++;
            }

            if(i == arrSize - 1 && isOdd(counter))
            {
                answer +=  tempSumm;
            }
        }
        else{
            if(isOdd(counter)){
                answer +=  tempSumm;
            }

            tempSumm = 0;
            counter = 0;
        }




    }

    return answer;
}

bool isOdd(int num)
{
    num %= 2;

    if(num == 0){
        return false;
    }
    else {
        return true;
    }
}

