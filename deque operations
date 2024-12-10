//Program to implement deque using array
#include<iostream>
using namespace std;

class Deque
{	
	int f = -1;
	int r = -1;
	int max = 10;
	int deque[10];
	public:
	
	void insert_front(int val)
	{		
		if(f == 0 && r == max -1 || f == r + 1)
			cout << "Queue Overflow " << endl;
		else if(f == -1 && r == -1)
		{
			f = r = 0;
			deque[f] = val;
		}
		else if(f == 0)
		{
			f = max - 1;
			deque[f] = val;
		}
		else
		{
			f--;
			deque[f] = val;
		}
	}
	
	void insert_rear(int val)
	{
		if(f == 0 && r == max -1 || f == r + 1)
			cout << "Queue Overflow " << endl;
		else if(f == -1 && r == -1)
		{
			f = r = 0;
			deque[f] = val;
		}
		else if(r == max - 1)
		{
			r = 0;
			deque[r] = val;
		}
		else
		{
			r++;
			deque[r] = val;
		}
	}
	
	void delete_front()
	{
		if(f == -1 && r == -1)
			cout << "Queue Underflow " << endl;
		else if(f == max - 1 )
		{
			cout << "Element to be deleted " << deque[f]<<endl;
			f = 0;
		}
		else if(f == r)
		{
			cout << "Element to be deleted " << deque[f]<<endl;
			f = r = -1;
		}
		else
		{
			cout << "Element to be deleted " << deque[f]<<endl;
			f++;
		}
	}
	
	void delete_rear()
	{
		if(f == -1 && r == -1)
			cout << "Queue Underflow " << endl;
		else if(r == 0 )
		{
			cout << "Element to be deleted " << deque[r]<<endl;
			r = max - 1;
		}
		else if(f == r)
		{
			cout << "Element to be deleted " << deque[r]<<endl;
			f = r = -1;
		}
		else
		{
			cout << "Element to be deleted " << deque[r]<<endl;
			r--;
		}
	}
	void display()
	{	
			
		if(r != max - 1 && !(f < r))
		{
			for(int i=f;i<=max-1;i++)
			{
				cout << deque[i] << " ";
			}
			for(int i=0;i<=r;i++)
			{
				cout << deque[i] << " ";
			}
			cout << endl;
		}
		else
		{
			for(int i=f;i<=r;i++)
			{
				cout << deque[i] << " ";
			}
		}
	}
};

int main()
{
	Deque d1;
	int num,ch,flag = 1;
	while(flag)
	{
		cout << "Enter 1 - Insert at the front " << endl;
		cout << "Enter 2 - Insert at the rear " << endl;
		cout << "Enter 3 - Delete from front " << endl;
		cout << "Enter 4 - Delete from rear "<< endl;
		cout << "Enter 5 - Display "<< endl;
		cout << "Enter any other number to EXIT"<< endl;
		cout << "Enter your choice : ";
		cin>>ch;
		switch(ch)
		{
			case 1:
				cout << "Enter the number to be inserted : ";
				cin>>num;
				d1.insert_front(num);
				break;
			case 2:
				cout << "Enter the number to be inserted : ";
				cin>>num;
				d1.insert_rear(num);
				break;
			case 3:
				d1.delete_front();
				break;
			case 4:
				d1.delete_rear();
				break;
			case 5:
				d1.display();
				break;
			default:
				flag = 0;
				break;
		}
	}		
	return 0;
}
