
def add(mat1,mat2):
	mat3=[]
	for i in range(0,r):
		a=[]
		for j in range(0,c):
			ele=mat1[i][j]+mat2[i][j]
			a.append(ele)
		mat3.append(a)
	return mat3	

#Substraction of matrices	
def sub(mat1,mat2):
	mat3=[]
	for i in range(0,r):
		a=[]
		for j in range(0,c):
			ele=mat1[i][j]-mat2[i][j]
			a.append(ele)
		mat3.append(a)
	return mat3
	
def mult(mat1,mat2):
	result=[[0,0],[0,0]]
	for i in range(len(mat1)):
		for j in range(len(mat2[0])):
			for k in range(len(mat2)):
           			result[i][j] += mat1[i][k] * mat2[k][j]
	return result

#Transpose of matrices	
def trans(mat):
	mat3=[]
	for i in range(0,r):
		a=[]
		for j in range(0,c):
			mat3[i][j]=mat[j][i]
	return mat3

matA=[]
matB=[]
r=int(input("Enter number of rows: "))
c=int(input("Enter number of columns: "))

for i in range(0,r):
	a=[]
	for j in range(0,c):
		val=int(input("Enter the value of A["+str(i)+","+str(j)+"] : "))
		a.append(val)
	matA.append(a)
	
for i in range(0,r):
	a=[]
	for j in range(0,c):
		val=int(input("Enter the value of B["+str(i)+","+str(j)+"] : "))
		a.append(val)
	matB.append(a)

print("Matrix A is: ")
print(matA)
print("Matrix B is: ")
print(matB)	
		
flag=1

while flag==1:
	print("MENU")
	print("1. Addition of matrices. ")
	print("2. Substraction of matrices. ")
	print("3. Multiplication of matrices. ")
	print("4. Transpose of matrices. ")
	print("5. Exit")
	ch=int(input("Enter your choice : "))
	
	if ch==1:
		print("Addition of the matrices is: ",add(matA,matB))
		a=input("Do you want to continue (yes/no): ")
		if a == "yes":
			flag=1
		else:
			flag=0
		
	elif ch==2:
		print("Substraction of the matrices is: ",sub(matA,matB))
		a=input("Do you want to continue (yes/no): ")
		if a == "yes":
			flag=1
		else:
			flag=0
	elif ch==3:
		print("Multiplication of the matrices is : ",mult(matA,matB))
		a=input("Do you want to continue (yes/no): ")
		if a == "yes":
			flag=1
		else:
			flag=0
	elif ch==4:
		print("Transpose of matrix A is: ",trans(matA))
		print("Transpose of matrix B is: ",trans(matB))
		a=input("Do you want to continue (yes/no): ")
		if a == "yes":
			flag=1
		else:
			flag=0
	elif ch==5:
		flag=0
		
	else:
		print("Error Select valid choice.")



if flag==0:
	print("Thanks! for using the program")
