#include <stdio.h>
#include <stdlib.h>
#include <time.h>
void grid(void) 
{
    int cell[6][6], row, col, s, i, j;
    char in = 'A';
    srand(time(NULL));

    for (row = 0; row <= 5; row++) 
    {
        printf("\t\t\t[ |");
        for (col = 0; col <= 5; col++) 
        {
            s = rand() % 6 + 1;
            if (s % 2 == 0)
            {
                cell[row][col] = rand() % 6 + 1;
                for (j = 0; j<col; j++) 
                {
                    if (cell[row][j] == cell[row][col]) 
                    {
                        col--;
                        continue;
                    }
                }
            }
            else { 
                printf("   | ", in++); continue; 
                }
            printf(" %d | ", cell[row][col]);
        }
        printf("]\n\n");
    }
}

int main()
{
    grid();
}
