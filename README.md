# design-table-using-c-
how to create  table in c++  using 2 dimensional  array which help to analysis of  datato 
here i will show the code of c++ language which help you to design table.For this use turbo c++ compiler and dev c++ etc'.

To install dev c++ [click here]( https://sourceforge.net/projects/orwelldevcpp/files/latest/downloadI)

If we have question such as

An election is contested by four candidates C1,C2,C3 and C4 for the president post of stock trading companies located at different four places P1,P2,P3 and P4 in Mumbai. The result have been reported by each place is as follows. 


Write a C++ program to do the following:

a. Read the votes from above data table that contains one row for each place. 
b. Display the table content along with total votes given at each place.
c. Compute and display the total number of votes received by each candidate. 

**Table is given below:**

Place No.                         Candidates  
                          C1   C2   C3   C4
               
P1               156 137 166 214 



P2               132 183 234 226


P3               135 256 259 169


P4              134 248 123 243 



**To create and show all the answer just look at my given code:**


#include <iostream>
using namespace std;



class election 

{
	
  
  int arr[10][10];
  
  
	int r,c;
	
  
  public:
  
  
		void getdata()
		{
			cout<<"Enter rows and columns :"<<endl;
			cin>>r>>c;
			for(int i=0;i<c;i++)
			{
				for(int j=0;j<r;j++)
				{
					cin>>arr[i][j];
				}
				cout<<"\n";
			}
		}

		void showdata()
		{
			for(int i=0;i<c;i++)
			{
				for(int j=0;j<r;j++)
				{
					cout<<arr[i][j]<<"  ";
				}
				cout<<"\n";
			}
		}

		void total_votes_at_Place()
		{}
			int total_votes=0;
			cout<<"Counting total_votes of each place"<<endl;
			for(int i=0;i<r;i++)
			{
				cout<<"For P"<<i+1<<endl;
				for(int j=0;j<c;j++)
				{
					total_votes+=arr[i][j];
				}
				cout<<"total_votes:"<<total_votes<<endl;
				total_votes=0;
			}
		}

		void total_votes_of_candidate()
		{
			int total_votes=0
			cout<<"Counting total_votes of each candidate:"<<endl;
			for(int i=0;i<c;i++)
			{
				cout<<"For C"<<i+1<<endl;
				for(int j=0;j<r;j++)
				{
					total_votes+=arr[i][j];
				}
				cout<<"total_votes:"<<total_votes<<endl;
				total_votes=0;
			}
		}
};

int main()



{



	election E;
  
	E.getdata();
  
	E.showdata();
  
	E.total_votes_at_Place();
  
	E.total_votes_of_candidate();
  
	return 0;
}



In above code there using class we defined three member fuction
1. getdata-- to take data from user

2.show data-- to design table and show to user

3.total_votes_at_place --to compute votes at each place and display

4. total_votes_of_candidates--to compute votest of each candidates and display



**thank you**




