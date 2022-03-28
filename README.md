
#include <stdlib.h>
#include <stdio.h>
#define row 10
#define colume 10
#define row2 5
#define colume2 5
#define _CRT_SECURE_NO_WARNINGS

int main()
{
	int x = 0, y = 0, a = 0, b = 0, trigger = 0;
	int mtrx[row][colume] = { {1,2,3,4,5,0,0,0,0,0}, {6,7,8,9,10,0,0,0,0,0}, { 11,12,13,14,15,0,0,0,0,0}, {16,17,18,19,20,0,0,0,0,0}, {21,22,23,24,25,0,0,0,0,0}, {0,0,0,0,0,0,0,0,0,0}, {0,0,0,0,0,0,0,0,0,0}, {0,0,0,0,0,0,0,0,0,0}, {0,0,0,0,0,0,0,0,0,0}, {0,0,0,0,0,0,0,0,0,0} };
	int mtrx2[row2][colume2] = { { 1,2,3,4,5 },{ 6,7,8,9,10 },{ 11,12,13,14,15 },{ 16,17,18,19,20},{ 21,22,23,24,25} };

	for (x = 0; x < colume; x++)
	{
		for (y = 0; y < row; y++)
		{
			for (a = 0; a < colume; a++)
			{
				for (b = 0; b < row; b++)
				{

					if (mtrx2[a][b] == mtrx[x][y])
					{
					
						trigger++;
						
						
					}
				}
			}
		}
	}

	printf("%d", trigger);
	

	system("pause");
}


//יש לקלוט מטריצה בגודל 10 על 10
//ויש לקלוט מטריצה בגודל 5 על 5
//יש להדפיס האם המטריצה 5 על 5 נמצאת בתוך המטריצה של 10 על 10 
