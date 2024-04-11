# C++ PROGRAMS
***************************************************************All Programs of C++ WHICH ARE done in training classes ****************************************************
                                                                    Program 1- power of (x^n)
                                                                    -------------------------
a. Through procedural approach
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
//power of x to the n(x^n) program by procedural approach in c++
#include<stdio.h>
#include<math.h>
int main()
{
	int x,n ,res;
	printf("Enter value of x : ");
	scanf("%d",&x);
	printf("\nEnter power of x :");
	scanf("%d",&n);
	res=pow(x,n);
	printf("result is : %d",res);
	return 0;
	
}
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

Method 2 of program 1 - b. Through object based approach
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
//power of x to the n(x^n) program by object based approach in c++
#include<iostream>
#include<cmath>
using namespace std;
int main()
{
	int x,n ,res;
	cout<<"Enter value of x : "<<endl;
	cin>>x;
	cout<<"Enter power of x"<<endl;
	cin>>n;
	res=pow(x,n);
	cout<<"result is :  "<<res;
	return 0;
	
}
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%



Method 3 of program 1 - b. Through object oriented approach
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
//power of x to the n(x^n) program by object oriented  approach in c++
#include<iostream>
#include<cmath>
using namespace std;
class power
{
	int x,n, res;
	public:
	void input()
	{
		cout<<"Enter value of x : "<<endl;
		cin>>x;
		cout<<"Enter power of x: "<<endl;
		cin>>n;
		
	}
	void process()
	{
		res=pow(x,n);
	}
	void output()
	{
		cout<<"Result is : "<<res;
	}
};
int main()
{
	power obj;
	obj.input();
	obj.process();
	obj.output();
	return 0;
}
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
                                                                                PROGRAM 2 :  FACTORIAL OF A NUMBER
                                                                              --------------------------------------------
a. Through procedural approach
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
//FACTORIAL  of a number (n) by procedural approach in c++
#include<stdio.h>
int main()
{
	int f=1,n,i;
	printf("Enter value of a number :\n");
	scanf("%d",&n);
	for(i=1;i<=n;i++)
	{
		f=f*i;
	}
	printf("\nFactorial of number is %d ",f);
	return 0;
}
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

Method 2 of program 2 - b. Through object based approach
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
//FACTORIAL  of a number (n) by object based approach in c++
#include<iostream>
using namespace std;
int main()
{
	int f=1,n,i;
	cout<<"Enter value of a number: "<<endl;
	cin>>n;
	for(i=1;i<=n;i++)
	{
		f=f*i;
	}
	cout<<"Factorial  of a number is: "<<f<<endl;
	return 0;
}
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

Method 3 of program 2 - b. Through object oriented approach
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
//FACTORIAL  of a number (n) by object oriented approach in c++
#include<iostream>
using namespace std;
class factorial
{
	int f=1,n,i;
	public:
		void input()
		{
			  cout<<"Enter value of a number: "<<endl;
        cin>>n;	
		}
		void process()
		{
				for(i=1;i<=n;i++)
     	{
	     	f=f*i;
      }
		}
		void output()
		{
			  cout<<"Factorial of a number is: "<<f;	
		}
	};
int main()
{
    factorial obj;
    obj.input();
    obj.process();
    obj.output();
	  return 0;
}
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

                                  PROGRAM 3- Access the information of two students by main function through making class data is public through oo aproach.
                                  ---------------------------------------------------------------------------------------------------------------------------
//access the information of two students by main function through making class data is public through oo aproach
#include<iostream>
using namespace std;
class student
{
	public:
		int roll;
		string name;
		float marks;
};
int main()
{
	student s1,s2;
	s1.roll=11;
	s1.name="Tulsi";
	s1.marks=50;
	s2.roll=22;
	s2.name="Komal";
	s2.marks=90;
	cout<<"Data of student 1: "<<endl<<"Name:  ";
	cout<<s1.name<<"  "<<"Roll no. : "<<s1.roll<<"  "<<"Marks :  " <<s1.marks<<endl;
	cout<<"Data of Student 2: "<<endl<<"Name:  ";
	cout<<s2.name<<"  "<<"Roll no. : "<<s2.roll<<"  "<<"Marks : "<<s2.marks<<endl;
	return 0;
}
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
                          PROGRAM 4-Access the information of two students by main function throgh set and get method in class making public by oo approach
                        ------------------------------------------------------------------------------------------------------------------------------------
//Access the information of two students by main function throgh set and get method in class making public by oo approach
#include<iostream>
using namespace std;
class stu
{
		int roll;
		string name;
		float marks;
		public:
			void set(int r,string n,float m)
			{
				      roll=r;
             	name=n;
            	marks=m;
			}
      void get()
	    {
			   cout<<"ROLL: "<<roll<<"  "<<"Name : "<<name<<"  "<<"Marks: "<<marks<<endl;
      }
};
int main()
{
	stu s1,s2;
	s1.set(11,"Tulsi",85);
	s1.get();
	s2.set(22,"Komal",80);
	s2.get();
  return 0;
}
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

    PROGRAM 5-Access the information of one students in two times by class through set and get method by putting constant info and making object in main function through oo aproach. 
  -----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
//Access the information of two students by class through set and get method by putting constant info and making object in main function through oo aproach.
#include<iostream>
using namespace std;           //But here only access one student information not of two student due to no object making 
class student
{
	
		int roll;
		string name;
		float marks;
		public:
			void set()
			{
			   
	           roll=22;
	           name="Tulsi";
	           marks=90;
	           roll=33;
	           name="Komal";
	           marks=90;
			}
	    void get()
	    {
			     cout<<"ROLL: "<<roll<<"  "<<"Name : "<<name<<"  "<<"Marks: "<<marks<<endl;
     	}
};
int main()
{
   	student s1,s2;
	s1.set();
	s1.get();
	s2.set();
	s2.get();
    return 0;
}    
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%


