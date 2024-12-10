//In any lang program, mostly syntax error occurs due to unbalancing delimiter such as (),{},[]. Write CPP program using stack to check whether given expression is well parenthesized.

#include <iostream>
using namespace std;
#define size 5

class stackexp{
public:
	int top;
	char stk[size];
	stackexp(){
		top = -1;
	}
	bool overflow();
	bool underflow();
	void push(char);
	char pop();
	bool isMatching(char, char);
};

bool stackexp::overflow(){
	if (top == (size - 1)){
		return true;
	}else{
		return false;
	}
}

bool stackexp::underflow(){
	if (top == -1){
		return true;
	}else{
		return false;
	}
}

void stackexp::push(char a){
	if (!overflow()){
		top += 1;
		stk[top] = a;
	}else{
		cout << "Overflow!" << endl;
	}
}

char stackexp::pop(){
	if (!underflow()){
		char s;
		s = stk[top];
		top -= 1;
		return s;
	}else{
		cout << "Underflow!" << endl;
		return '\0';
	}
}


bool stackexp::isMatching(char a, char b){
	if (a == '(' && b == ')'){
		return true;
	}
	else if (a == '{' && b == '}'){
		return true;
	}
	else if (a == '[' && b == ']'){
		return true;
	}
	else{return false;}
}

int main(){
	stackexp s;
	string exp;
	
	cout << "Enter the string: ";
	cin >> exp;
	
	int flag = 0;
	
	for (int i = 0; exp[i] != '\0'; i++){
		if (exp[i] == '(' || exp[i] == '{' || exp[i] == '['){
			s.push(exp[i]);
		}
		else if (exp[i] == ')' || exp[i] == '}' || exp[i] == ']'){
			if (s.underflow()){
				flag = 1;
				break;
			}
			else if (s.isMatching(s.stk[s.top],exp[i])){
				s.pop();
			}
			else{
				flag = 1;
				break;
			}
		}
	}
	if (flag == 1 || !s.underflow()){
		cout << "Invalid parantheses" << endl;
	}
	else if (s.underflow()){
		cout << "Valid parantheses" << endl;
	}
	return 0;
}

	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
