# Lab-8
#include <iostream>

using namespace std;

void LinearIndx(int i , int j)

{	
	int B[10];
	int I;
	//An array with 8 rows and 8 columns
	int A[i][j]= {{0,0},{1,0},{2,0},{2,1},{2,2},{3,0},{3,1},{3,2}};
	
	//Output each array element's value
	for (int i = 0; i < 10; i++)
	{
		for (int j=0; j<10;j++)
		{
			// An if else statment to assgin the values to 0 when i < j
			if (i < j)
			{
				cout<< "0"<< " ";
			}
			else
			//prints the lower triangular matrix
			cout<< A[i][j]<< "  ";
			
			//Stores the array into a one dimensianal array.
			B[I]=A[i][j];
			//prints the !D array that stores the 2D array values	
			//cout<< B[i]<< endl;
		}
		cout<< endl;
	}
}

void Inverse(int i,int j)
{
	int B[8];
	int I;
	//An array with 8 rows and 8 columns
	int A[i][j]= {{0,0},{1,0},{2,0},{2,1},{2,2},{3,0},{3,1},{3,2}};
	
	//Output each array element's value
	for (int i = 0; i < 10; i++)
	{
		for (int j=0; j<10;j++)
		{
			//cout<< A [i][j]<<endl;
			
			B[I]=A[i][j];
			//swapping i and j
			while (i < j)
			{
				int temp = B[i];
				B[i]=B[j];
				B[j]= temp;
				i++;
				j--;
			}
			//prints the array after
			for (int i=0; i<8;i++){
				for(int j=0; j<8;j++){
					cout<<A[i][j]<< endl;
					if (i < j)
			{
				cout<< "0"<< " ";
			}
			else
			//prints the lower triangular matrix
			cout<< A[i][j]<< "  ";
			
			//prints the !D array that stores the 2D array values	
			
				}
			} 	
	
			
		}
	}
}
class message{
	public:
	void messages()
{
	cout<<"Here are the results: "<< endl;
}
};

int main()
{
	message mess;
	mess.messages();
	//LinearIndx(8,8);
//	LinearIndx(8,8);
	LinearIndx(32,32);
}
