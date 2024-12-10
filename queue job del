/*
Queue Implementation for job with delete and insert functions
*/

#include <iostream>
#define MAX 10
using namespace std;

struct queue{
	int q[MAX];
	int front, rear;
};

class Queue{
public:
	queue a;
	void set_values(int q[MAX], int n){
		for (int i = 0; i < MAX; i++){
			a.q[i] = q[i];
		}
		a.front = 0;
		a.rear = n - 1;
	}
	bool Overflow(){
		if (a.rear >= (MAX)){
			return true;
		}else{
			return false;
		}
	}
	bool Underflow(){
		if (a.rear == -1){
			return true;
		}else{
			return false;
		}
	}
	
	void Enqueue(int ele){
		if (!Overflow()){
			a.rear += 1;
			a.q[a.rear] = ele;
			cout << "Element added: " << ele << endl;
		}else{cout<<"Overflow!";}
	}
	
	void Dequeue(){
		if (!Underflow()){
			cout << "Element dequeued: " << a.q[a.front] << endl;
			a.front+=1;
		}else{cout<<"Underflow!";}
	}
	
	void Display(){
		cout<<"\nQueue: ";
		for (int i = a.front; i < (a.rear + 1); i++){cout << a.q[i] << " ";}
		cout << "\nFront: " << a.front << endl;
		cout << "Rear: " << a.rear << endl;
	}
};

int main(){
	Queue a;
	int b[] = {1,2,3,4,5,6,7,8};
	int size = sizeof(b)/sizeof(b[0]);
	a.set_values(b,size);
	a.Display();
	
	int ch;
	bool str = true;
	while (str){
		cout << "1. Enqueue\n2. Dequeue\n3. Display\n4. Exit" << endl;
		cin >> ch;
		switch (ch){
			case 1:
				int c;
				cout << "Enter element to enqueue: ";
				cin >> c;
				a.Enqueue(c);
				break;
			case 2:
				a.Dequeue();
				break;
			case 3:
				a.Display();
				break;
			case 4:
				str = false;
				break;
		}
	}
		 
	/*
	a.Enqueue(5);
	a.Display();
	
	a.Dequeue();
	a.Display();
	*/
}
			
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
