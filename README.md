#  ***PROGRAMMING FOR PROBLEM SOLVING ESC-18105***
## ***NAME:- GURINDER SINGH***
## ***ROLL NO.:- 1915024***
## ***BRANCH:- CSE***
## ***SECTION:- A1***
![LOGO](https://camo.githubusercontent.com/4659980dc21fcc7231390ce3a2ea8b724c3b9058/68747470733a2f2f626c6f672e636f616368696e676b61726f2e6f72672f77702d636f6e74656e742f75706c6f6164732f323031392f30372f6c6f676f2e6a7067)
## *1. Program to print Welcome to budding   Engineers*
``` 
#include<stdio.h>
int main()
{
    puts("Welcome to Budding Engineers");
    return 0;
}
```
## *Output of the program*
```
Welcome to Budding Engineers
```
## *2. Program to print Address using puts*
```
#include<stdio.h>
int main()
{
        puts("Address: H.No.:7111/1A,  St.No.:14/2, Durga Nagar, Waheguru Road, Near Kartar Chowk, Ludhiana(Punjab)-141 003");
        return 0;
}
```
## *Output of the program*
```
Address: H.No.:7111/1A, St.No.:14/2, Durga Nagar, Waheguru Road, Near Kartar Chowk, Ludhiana(Punjab)-141 003
```
## *3. Program to find the sum of two numbers*
```
#include<stdio.h>
int addnum(int a,int b);
void main()
{
        int a,b;
        printf("Enter two numbers:\n ");
        scanf("%d",&a);
        scanf("%d",&b);
        int s=addnum(a,b);
        printf("Sum= %d\n",s);
}
int addnum(int a,int b)
{
        int s=a+b;
        return s;
}
```
## *Output of the program*
```
Enter two numbers:
5
8
Sum= 13
```
## *4. Program to Convert Celsius temperature to Fahrenheit temperature*
```
#include<stdio.h>
int main()
{
        float f,c;
        printf("Enter the temperature in Celsius= ");
        scanf("%f",&c);
        f=(c*9/5)+32;
        printf("Temperature in Fahrenheit= %.2f\n",f);
        return 0;
}
```
## *Output of the program*
```
Enter the temperature in Celsius= 37
Temperature in Fahrenheit= 98.60
```
## *5. Program to find Area and Perimeter of circle*
```
#include<stdio.h>
int main()
{
        float r,area,perimeter;
        printf("Enter the radius of circle: ");
        scanf("%f",&r);
        area=3.14*r*r;
        perimeter=2*3.14*r;
        printf("Area of the circle: %.2f\n",area);
        printf("Perimeter of the circle: %.2f\n",perimeter);
        return 0;
}
```
## *Output of the program*
```
Enter the radius of circle: 5
Area of the circle: 78.50
Perimeter of the circle: 31.40
```
## *6. Program to swap two numbers without using a third variable*
```
#include <stdio.h>
int main()
{
        int a,b;
        printf("Enter the value of a and b: ");
        scanf("%d%d",&a,&b);
        a=a+b;
        b=a-b;
        a=a-b;
        printf("Value of a is %d and b is %d\n",a,b);
}
```
## *Output of the program*
```
Enter the value of a and b: 5 10
Value of a is 10 and b is 5
```
## *7. Program to find whether the number is even or odd*
```
#include<stdio.h>
int check(int a);
int main()
{
        int num;
        printf("Enter the number: ");
        scanf("%d",&num);
        int s=check(num);
        return 0;
}
int check(int a)
{
        int s1=a%2;
        if(s1==0)
        printf("Number is even\n");
        else
        printf("Number is odd\n");
        return s1;
}
```
## *Output of the program*
```
Enter the number: 5
Number is odd
```
## *8. Program to find the Factorial of an number*
```
#include<stdio.h>
int main()
{
        int n,i,p=1;
        printf("Enter the number: ");
        scanf("%d",&n);
        for(i=1;i<=n;i++)
        {
                p=p*i;
        }
        printf("Factorial of %d is %d\n",n,p);
        return 0;
}
```
## *Output of the Program*
```
Enter the number: 5
Factorial of 5 is 120
```
## *9. Program to Reverse a number*
```
#include<stdio.h>
int main()
{
        int a,t,b,c;
        printf("Enter the number: ");
        scanf("%d",&a);
        t=a;
        while(a!=0)
        {
                b=a%10;
                c=c*10+b;
                a=a/10;
        }
        printf("Reverse of %d is %d\n",t,c);
        return 0;
}
```
## *Output of the Program*
```
Enter the number: 586
Reverse of 586 is 685
```
## *10. Program to play Fizzbuzz*
```
#include<stdio.h>
void main()
{
        int a,i;
        printf("Enter the limit: ");
        scanf("%d",&a);
        for(i=1;i<=a;i++)
        {
                if(i%3==0&&i%5!=0)
                printf("fizz\n");
                if(i%5==0&&i%3!=0)
                printf("buzz\n");
                if(i%3==0&&i%5==0)
                printf("fizzbuzz\n");
                if(i%3!=0&&i%5!=0)
                printf("%d\n",i);
        }
        return 0;
}
```
## *Output of the program*
```
Enter the limit: 15
1
2
fizz
4
buzz
fizz
7
8
fizz
buzz
11
fizz
13
14
fizzbuzz
```
## *11. Program to find the days of week using Switch Case*
```
#include<stdio.h>
int main()
{
    int number;
    printf("Enter an number to print days of the week  (1, 2, 3, 4, 5, 6, 7): ");
    scanf("%d", &number);
    switch(number)
    {
        case 1:
            puts("Monday");
            break;
        case 2:
            puts("Tuesday");
            break;
        case 3:
            puts("Wednesday");
            break;
        case 4:
            puts("Thursday");
            break;
        case 5:
            puts("Friday");
            break;
        case 6:
            puts("Saturday");
            break;
        case 7:
            puts("Sunday");
            break;
        default:
            printf("Error! keyword is not correct\n");
    }

    return 0;
}
```
## *Output of a program*
```
Enter an number to print days of the week  (1, 2, 3, 4, 5, 6, 7): 5
Friday
```
## *12. Program to make a simple calculator using Switch case*
```
# include <stdio.h>
int main() {
    char operator;
    double a,b;
    printf("Enter an operator (+, -, *,/): ");
    scanf("%c", &operator);
    printf("Enter two operands: \n");
    scanf("%lf %lf",&a, &b);
    switch(operator)
    {
        case '+':
            printf("%.2f + %.2f = %.2f\n",a, b, a + b);
            break;
        case '-':
            printf("%.2f - %.2f = %.2f\n",a, b, a - b);
            break;
        case '*':
            printf("%.2f * %.2f = %.2f\n",a, b, a * b);
            break;
        case '/':
            printf("%.2f / %.2f = %2f\n",a, b, a / b);
            break;
        default:
            printf("Error! operator is not correct\n");
    }

    return 0;
}
```
## *Output of the Program*
```
Enter an operator (+, -, *,/): *
Enter two operands:
5
7
5.00 * 7.00 = 35.00
```
## *13. Program to check Leap year*
```
#include<stdio.h>
int main()
{
        int y;
        printf("Enter the year= ");
        scanf("%d",&y);
        if(y%4==0)
        printf("It is a leap year\n");
        else
        printf("It is not a leap year\n");
        return 0;
}
```
## *Output of the program*
```
Enter the year= 2000
It is a leap year
```
## *14. Program to check Prime number*
```
#include<stdio.h>
int main()
{
        int a,i,c=0;
        printf("Enter the number\n");
        scanf("%d",&a);
        for(i=1;i<=a;i++)
        {
                if(a%i==0)
                c++;
        }
        if(c==2)
        printf("Number is prime\n");
        else
        printf("Number is not prime\n");
        return 0;
}
```
## *Output of the program*
```
Enter the number
5
Number is prime
```
## *15. Program to check Palindrome number*
```
#include<stdio.h>
int main()
{
        int n,t,a,b=0;
        printf("Enter the number\n");
        scanf("%d",&n);
        t=n;
        while(n!=0)
        {
                a=n%10;
                b=b*10+a;
                n=n/10;
        }
        if(b==t)
        printf("Number is palindrome\n");
        else
        printf("Number is not palindrome\n");
        return 0;
}
```
## *Output of the Program*
```
Enter the number
121
Number is palindrome
```
## *16. Program to check Palindrome word*
```
#include<stdio.h>
#include<string.h>
int main()
{
        char a[100],b[100],c[100];
        printf("Enter the word: ");
        scanf("%s",a);
        strcpy(c,a);
        int l=strlen(a);
        for(int i=1;i<=l;i++)
        b[i]=a[l-i];
        if(strcmp(b,c)==0)
        printf("Word is Palindrome\n");
        else
        printf("Word is not Palindrome\n");
}
```
## *Output of the program*
```
Enter the word: madam
Word is Palindrome
```
## *17. Program to print Fibonnacci Series*
```
#include <stdio.h>
int main()
{
        int n,a=0,b=1,c=0,i;
        printf("Enter ther limit of series ");
        scanf("%d",&n);
        printf("%d %d ",a,b);
        for(i=2;i<=n;i++)
        {
                c=a+b;
                printf("%d ",c);
                a=b;
                b=c;
        }
        printf("\n");
        return 0;
}
```
## *Output of the program*
```
Enter ther limit of series 15
0 1 1 2 3 5 8 13 21 34 55 89 144 233 377 610
```
## *18. Program to enter elements and display a 1D array*
```
#include<stdio.h>
int main()
{
        int a[100],n;
        printf("Enter the limit of array: ");
        scanf("%d",&n);
        printf("Enter the elements for array:\n");
        for(int i=1;i<=n;i++)
        scanf("%d",&a[i]);
        printf("Array\n");
        for(int i=1;i<=n;i++)
        printf("%d ",a[i]);
        printf("\n");
        return 0;
}
```
## *Output of the program*
```
Enter the limit of array: 5
Enter the elements for array:
2
2
4
5
7
Array
2 2 4 5 7
```
## *19. Program to enter elements and display a 2D array*
```
#include<stdio.h>
int main()
{
        int a[3][3];
        printf("Enter the value for 3*3 matrix\n");
        for(int i=1;i<=3;i++)
        {
                for(int j=1;j<=3;j++)
                scanf("%d",&a[i][j]);
        }
        printf("Matrix A\n");
        for(int i=1;i<=3;i++)
        {
                for(int j=1;j<=3;j++)
                printf("%d\t",a[i][j]);
                printf("\n");
        }
}
```
## *Output of the program*
```
Enter the value for 3*3 matrix
5
2
1
4
5
7
5
8
9
Matrix A
5       2       1
4       5       7
5       8       3
```
## *20. Program to Add two matrices*
```
#include <stdio.h>
int main()
{
        int a[3][3],b[3][3],c[3][3];
        printf("Enter the value for first matrix\n");
        for(int i=1;i<=3;i++)
        {
                for(int j=1;j<=3;j++)
                scanf("%d",&a[i][j]);
        }
        printf("Enter the value for second matrix\n");
        for(int i=1;i<=3;i++)
        {
                for(int j=1;j<=3;j++)
                scanf("%d",&b[i][j]);
        }
        for(int i=1;i<=3;i++)
        {
                for(int j=1;j<=3;j++)
                c[i][j]=a[i][j]+b[i][j];
        }
        printf("First Matrix\n");
        for(int i=1;i<=3;i++)
        {
                for(int j=1;j<=3;j++)
                printf("%d\t",a[i][j]);
                printf("\n");
        }
        printf("Second Matrix\n");
        for(int i=1;i<=3;i++)
        {
                for(int j=1;j<=3;j++)
                printf("%d\t",b[i][j]);
                printf("\n");
        }
        printf("Result of Addition of Two Matrix\n");
        for(int i=1;i<=3;i++)
        {
                for(int j=1;j<=3;j++)
                printf("%d\t",c[i][j]);
                printf("\n");
        }
}
```
## *Output of the program*
```
Enter the value for first matrix
5
2
3
6
4
1
2
5
7
Enter the value for second matrix
4
5
1
7
8
6
5
1
2
First Matrix
5       2       3
6       4       1
2       5       7
Second Matrix
4       5       1
7       8       6
5       1       2
Result of Addition of Two Matrix
9       7       4
13      12      7
7       6       9
```
## *21. Program to find Transpose of a matrix*
```
#include <stdio.h>
int main()
{
        int a[3][3],b[3][3],c[3][3];
        printf("Enter the value for matrix\n");
        for(int i=1;i<=3;i++)
        {
                for(int j=1;j<=3;j++)
                scanf("%d",&a[i][j]);
        }
        for(int i=1;i<=3;i++)
        {
                for(int j=1;j<=3;j++)
                c[j][i]=a[i][j];
        }
        printf("First Matrix\n");
        for(int i=1;i<=3;i++)
        {
                for(int j=1;j<=3;j++)
                printf("%d\t",a[i][j]);
                printf("\n");
        }
        printf("Result of Transpose of Matrix\n");
        for(int i=1;i<=3;i++)
        {
                for(int j=1;j<=3;j++)
                printf("%d\t",c[i][j]);
                printf("\n");
        }
}
```
## *Output of the program*
```
Enter the value for matrix
2
5
4
7
8
9
6
4
5
Matrix
2       5       4
7       8       9
6       4       5
Result of Transpose of Matrix
2       7       6
5       8       4
4       9       5
```
## *22. Program to find Substraction of two matrices*
```
#include <stdio.h>
int main()
{
        int a[3][3],b[3][3],c[3][3];
        printf("Enter the value for first matrix\n");
        for(int i=1;i<=3;i++)
        {
                for(int j=1;j<=3;j++)
                scanf("%d",&a[i][j]);
        }
        printf("Enter the value for second matrix\n");
        for(int i=1;i<=3;i++)
        {
                for(int j=1;j<=3;j++)
                scanf("%d",&b[i][j]);
        }
        for(int i=1;i<=3;i++)
        {
                for(int j=1;j<=3;j++)
                c[i][j]=a[i][j]-b[i][j];
        }
        printf("First Matrix\n");
        for(int i=1;i<=3;i++)
        {
                for(int j=1;j<=3;j++)
                printf("%d\t",a[i][j]);
                printf("\n");
        }
        printf("Second Matrix\n");
        for(int i=1;i<=3;i++)
        {
                for(int j=1;j<=3;j++)
                printf("%d\t",b[i][j]);
                printf("\n");
        }
        printf("Result of Subtraction of Two Matrix\n");
        for(int i=1;i<=3;i++)
        {
                for(int j=1;j<=3;j++)
                printf("%d\t",c[i][j]);
                printf("\n");
        }
}
```
## *Output of the program*
```
Enter the value for first matrix
5
2
1
4
7
8
6
5
4
Enter the value for second matrix
2
1
7
5
4
7
6
3
1
First Matrix
5       2       1
4       7       8
6       5       4
Second Matrix
2       1       7
5       4       7
6       3       1
Result of Subtraction of Two Matrix
3       1       -6
-1      3       1
0       2       3
```
## *23. Program to find multiplication of two matrices*
```
#include <stdio.h>
int main()
{
        int a[3][3],b[3][3],c[3][3],sum;
        printf("Enter the value for first matrix\n");
        for(int i=1;i<=3;i++)
        {
                for(int j=1;j<=3;j++)
                scanf("%d",&a[i][j]);
        }
        printf("Enter the value for second matrix\n");
        for(int i=1;i<=3;i++)
        {
                for(int j=1;j<=3;j++)
                scanf("%d",&b[i][j]);
        }
        for(int i=1;i<=3;i++)
        {
                for(int j=1;j<=3;j++)
                {
                        sum=0;
                        for(int k=1;k<=3;k++)
                        sum=sum+a[i][k]*b[k][j];
                        c[i][j]=sum;
                }
        }
        printf("First Matrix\n");
        for(int i=1;i<=3;i++)
        {
                for(int j=1;j<=3;j++)
                printf("%d\t",a[i][j]);
                printf("\n");
        }
        printf("Second Matrix\n");
        for(int i=1;i<=3;i++)
        {
                for(int j=1;j<=3;j++)
                printf("%d\t",b[i][j]);
                printf("\n");
        }
        printf("Result of Multiplication of Two Matrix\n");
        for(int i=1;i<=3;i++)
        {
                for(int j=1;j<=3;j++)
                printf("%d\t",c[i][j]);
                printf("\n");
        }
}                
```
## *Output of the program*
```
Enter the value for first matrix
2
3
4
5
1
4
7
2
3
Enter the value for second matrix
2
3
1
4
5
2
3
4
5
First Matrix
2       3       4
5       1       4
7       2       3
Second Matrix
2       3       1
4       5       2
3       4       5
Result of Multiplication of Two Matrix
28      37      28
26      36      27
31      43      26
```
## *24. Program  to find square of a number using function*
```
#include<stdio.h>
int square(int x);
int main()
{
        int n,s;
        printf("Enter the number: ");
        scanf("%d",&n);
        s=square(n);
        printf("Square of %d= %d\n",n,s);
}
int square(int x)
{
        int s=x*x;
        return s;
}
```
## *Output of the program*
```
Enter the number: 5
Square of 5= 25
```
## *25. Program to swap two numbers using call by value*
```
#include <stdio.h>
void swap(int, int);
int main()
{
        int x, y;
        printf("Enter the value of x and y\n");
        scanf("%d%d",&x,&y);
        printf("Before Swapping\nx = %d\ny = %d\n", x, y);
        swap(x, y);
        printf("After Swapping\nx = %d\ny = %d\n", x, y);
        return 0;
}
void swap(int a, int b)
{
        int temp;
        temp = b;
        b = a;
        a = temp;
}
```
## *Output of the program*
```
Enter the value of x and y
5
3
Before Swapping
x = 5
y = 3
After Swapping
x = 5
y = 3
```
## *26. Program to swap two numbers using call by reference*
```
#include <stdio.h>
void swap(int * num1, int * num2);
int main()
{
        int num1, num2;
        printf("Enter two numbers: ");
        scanf("%d%d", &num1, &num2);
        printf("Before swapping in main n");
        printf("Value of num1 = %d \n", num1);
        printf("Value of num2 = %d \n\n", num2);
        swap(&num1, &num2);
        printf("After swapping in main n");
        printf("Value of num1 = %d \n", num1);
        printf("Value of num2 = %d \n\n", num2);
        return 0;
}
void swap(int * num1, int * num2)
{
        int temp;
        temp = *num1;
        *num1= *num2;
        *num2= temp;
}
```
## *Output of the program*
```
Enter two numbers: 5
3
Before swapping in main nValue of num1 = 5
Value of num2 = 3

After swapping in main nValue of num1 = 3
Value of num2 = 5
```
## *27. Program to find Factorial of a number using recursion*
```
#include <stdio.h>
int factorial(int n);
int main()
{
        int n;
        printf("Enter the number: ");
        scanf("%d", &n);
        printf("Factorial of %d = %ld\n", n,factorial(n));
        return 0;
}
int factorial(int n)
{
        if (n>=1)
        return n*factorial(n-1);
        else
        return 1;
}
```
## *Output of the program*
```
Enter the number: 5
Factorial of 5 = 120
```
## *28. Program to print Fibonnicci Series using recursion*
```
#include<stdio.h>
int Fibonacci(int);
int main()
{
        int n,i=0;
        printf("Enter the limit: ");
        scanf("%d",&n);
        printf("Fibonacci series\n");
        for(int j=0;j<=n;j++)
        {
                printf("%d ",Fibonacci(i));
                i++;
        }
        printf("\n");
        return 0;
}
int Fibonacci(int n)
{
        if(n==0)
        return 0;
        else if(n==1)
        return 1;
        else
        return ( Fibonacci(n-1) + Fibonacci(n-2) );
}
```
## *Output of the program*
```
Enter the limit: 15
Fibonacci series
0 1 1 2 3 5 8 13 21 34 55 89 144 233 377 610
```
## *29. Program to enter elements in a structure and display them*
```
#include <stdio.h>
struct patient
{
        char name[10];
        float age;
        char gender;
};
int main()
{
        struct patient p;
        printf("Enter the name: ");
        scanf("%s",p.name);
        printf("Enter the age: ");
        scanf("%f",&p.age);
        printf("Enter the gender: ");
        scanf(" %c",&p.gender);
        printf("%s of age %.2f of gender %c is having liver disease\n",p.name,p.age,p.gender);
        return 0;
}
```
## *Output of the program*
```
Enter the name: Anshik
Enter the age: 17
Enter the gender: M
Anshik of age 17.00 of gender M is having liver disease
```
## *30. Program to enter elements in array using structure and display them*
```
#include <stdio.h>
struct student
{
        char name[10];
        int rollno;
        char branch[10];
        int maths;
        int chemistry;
};
int main()
{
        int n;
        printf("Enter the number of students: ");
        scanf("%d",&n);
        struct student p[n];
        for(int i=0;i<n;i++)
        {
                printf("Enter the name of the student: ");
                scanf("%s",p[i].name);
                printf("Enter the roll number of the student: ");
                scanf("%d",&p[i].rollno);
                printf("Enter the branch of the student: ");
                scanf("%s",p[i].branch);
                printf("Enter the marks of mathematics of the student: ");
                scanf("%d",&p[i].maths);
                printf("Enter the marks of chemistry of the student: ");
                scanf("%d",&p[i].chemistry);
        }
        for(int i=0;i<n;i++)
        {
                printf("%s of branch %s and roll number %d has scored %d and %d marks in mathematics and chemistry\n",p[i].name,p[i].branch$
        }
}
```
## *Output of the program*
```
Enter the number of students: 2
Enter the name of the student: Anshik
Enter the roll number of the student: 1915009
Enter the branch of the student: CSE
Enter the marks of mathematics of the student: 100
Enter the marks of chemistry of the student: 98
Enter the name of the student: Bhavneet
Enter the roll number of the student: 1915015
Enter the branch of the student: CSE
Enter the marks of mathematics of the student: 97
Enter the marks of chemistry of the student: 98
Anshik of branch CSE and roll number 1915009 has scored 100 and 98 marks in mathematics and chemistry
Bhavneet of branch CSE and roll number 1915015 has scored 97 and 98 marks in mathematics and chemistry
```
## *31. Program to use pointer variable*
```
#include<stdio.h>
int main()
{
        int n,*p;
        printf("Enter the value ");
        scanf("%d",&n);
        p=&n;
        printf("Value of n is %d and %d\n",n,&n);
        printf("Value of p is %d and %d\n",*p,p);
}
```
## *Output of the program*
```
Enter the value 16
Value and address of n is 16 and 799370564
Value and address of p is 16 and 799370564
```

