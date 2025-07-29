//  There are two types of header files
// 1 System header files --> it comes with the compailer
#include <iostream>
#include <iomanip>
// 2 User difined header files --> It is written by the programmer
// #include "this.h" // This will produce an error if this.h is not precent in current direcry
// for header files --> en.cpprefrence.com

using namespace std;
   int num1=7;
   int e=100;//i write it as globel variable
   int sum(int a ,int b);
   void swappointer(int* a, int* b);
   void swapReferenceVer(int &a, int &b);
   void sum(){
       float A= 34.56,y = 56.99, u = 23.98, s = 12.23 , h = 87.23, i = 89.12;
       cout<<A*y*u*s*h*i;

   }
   void G();
 
  int main(){
    int s = 19;

    /* this (int) is a variable (Bulid-in Type)
    we have 5 types of it 
    int - 1,-2 ,0
    float - 1.45,2.46
    char - 'a','b','c',
    double - 1.4465755756565656 
    bool - true or false, male or female ,*/


    cout<<" hello word. \n here sum ="<<s<<"\n";
    cout<<"Aayushi = ";
    sum();
    cout<<endl;
 
    /* this is lec 5 */
     
    double a,b,e;
    cout<<"\nEnter the values of a ="; /* '<<' is called insertion operater*/
    cin>>a;/* '>>' is called Extraction operater*/

    cout<<"Enter the values of b ="; /* '<<' is called insertion operater*/
    cin>>b;/* '>>' is called Extraction operater*/
    
    e = a + b;
    cout<<"the sum is e="<<e; // use of Arithmetic opreters
    cout<<"The sum is ="<<a+b<<endl; 
    cout<<endl;

 // this is lec 6
  cout<<"Opreters in c++"<<endl;
  cout<<"Follwing tyeps of opreters"<<endl;// endl =\n
  // Arithmetic Opreters
     
     cout<<"1. Arithmetic opreter."<<"\n";
     cout<<"The value of a + b ="<<a+b<<endl;
 
     cout<<"The value of a - b ="<<a-b<<endl;
     cout<<"The value of a * b ="<<a*b<<endl;
     cout<<"The value of a / b ="<<a/b<<endl;
     cout<<"The value of a % b ="<<int(a)%int(b)<<endl;// --> it's work for int value not for double so --> use typecasting
     cout<<"The value of a++ ="<<a++<<endl;
     cout<<"The value of a-- ="<<a--<<endl;
     cout<<"The value of ++a ="<<++a<<endl;
     cout<<"The value of --a ="<<--a<<endl;
     cout<<"The value of b++ ="<<b++<<endl;
     cout<<"The value of b-- ="<<b--<<endl;
     cout<<"The value of ++b ="<<++b<<endl;
     cout<<"The value of --b ="<<--b<<endl;
     cout<<endl;

  // Assigment Opreters --> use to assing values to variables
    
    char c='d';
    cout<<"2. Assigment Opreters"<<endl;
    cout<<"ex \nint a=7, b=9;\n char c='d';"<<endl;
    cout<<endl;

 // Comparison Opreters
    cout<<"3.Comparison Opreters "<<endl;
    cout<<"The value of a == b is"<<(a==b)<<endl;
    cout<<"The value of a != b is"<<(a!=b)<<endl;
    cout<<"The value of a < b is"<<(a<b)<<endl;
    cout<<"The value of a > b is"<<(a>b)<<endl;
    cout<<"The value of a <= b is"<<(a<=b)<<endl;
    cout<<"The value of a >= b is"<<(a>=b)<<endl;
    cout<<endl;

 // Logical Opreters
     cout<<"4. Logical Opreters"<<endl;
     cout<<"Following are the logical opreters in c++"<<endl;
     cout<<"THe value of the logical and Opreter ((a==b) && (a<b)) is:"<<((a==b) && (a<b))<<endl;
     cout<<"THe value of the logical or Opreter ((a==b) || (a<b)) is:"<<((a==b) || (a<b))<<endl;
cout<<endl;

// this is lec 7
// **********************Build in Data Types************************

   /* if we have both globle and local variable so the campiler's first choice is local variable <-- this is for interview  */
   /* but if i want write value of globel varible so i add (::)--> scope resolution opreter*/
    cout<<"**********************Build in Data Types************************"<<"\n";
    cout<<endl;
   e = a + b;
    cout<<"the sum is e="<<e<<endl; // use of Arithmetic opreters
    cout<<"the globel variable is e="<<::e<<endl; // use of Arithmetic opreters
cout<<endl;

// **********************float,double and long double Literals in Data Types************************

cout<<"**********************float,double and long double Literals in Data Types************************"<<"\n";
cout<<endl;
float d=34.4f; // in this (f and l)--> type of number float or long double,etc..... 
long double E=34.4l; // if we don't use it so compailer by default declared it as a double 

// (sizeof() opreter)--> size of desimal munbers
cout<<"the size of 34.4="<<sizeof(34.4)<<endl; 
cout<<"the size of 34.4f="<<sizeof(34.4f)<<endl; 
cout<<"the size of 34.4F="<<sizeof(34.4F)<<endl; 
cout<<"the size of 34.4l="<<sizeof(34.4l)<<endl; 
cout<<"the size of 34.4L="<<sizeof(34.4L)<<endl; 
cout<<endl;
// **********************Reference Variables************************

cout<<"**********************Reference Variables************************"<<"\n";
cout<<endl;
int g;
float h;
cout<<"Put the value of int g=";
cin>>g;

cout<<"Put the value of Float h=";
cin>>h;

cout<<"the vlue of g="<<float(g)<<endl;
cout<<"the vlue of g="<<(float)g<<endl;

cout<<"the vlue of h="<<int(h)<<endl;
cout<<"the vlue of h="<<(int)h<<endl;

cout<<"The Expression of g+h ="<<g+h<<endl;
cout<<"The Expression of g+int(h) ="<<g+int(h)<<endl;
cout<<"The Expression of g+(int)h ="<<g+(int)h<<endl;

// this is lec 8

cout<<"constants"<<endl;
const int j = 200;
cout<<"j="<<j;
cout<<endl;
cout<<endl;
// const --> if you don't want to change values of any variable

// **********************************Manipulators************************************

cout<<"// **********************************Manipulators************************************"<<endl;
cout<<endl;
// it's help for data display formeting 
// iostream --> endl ; iomanip --> setw(it's for fild width)
int x=1,y=34,z=12345;
cout<<"the value of x without setw = "<<x<<endl;
cout<<"the value of y without setw = "<<y<<endl;
cout<<"the value of z without setw = "<<z<<endl;

cout<<"the value of x = "<<setw(5)<<x<<endl;
cout<<"the value of y = "<<setw(5)<<y<<endl;
cout<<"the value of z = "<<setw(5)<<z<<endl;

// ***************************Opretor Precedence**********************************

cout<<"Opretor Precedence"<<endl;
float X=(((x*y)+45)/5);
// check is opretors from chart and if it's in same place so see the Associativity
// (Associativity)--> sum solve kervanu kyarthi chalu karvu aa [left to Right] or [Right to left]
// firstly make () on first opretor in chart
// (en.cpprefrence.com)
cout<<"(((x*y)+45)/5)= "<<X<<endl;

// this is lec 9
// ***************************Control structures**********************************
      cout<<"***************************Control structures**********************************"<<endl;
      cout<<endl;
// working : give a flow and logic of programme 

// types;  basic control structure
// 1--> sequence structure
// 2--> selection structure
// 3--> loop structure

// until now,this entire proggrame was the part of the sequesce structure
      cout<<"until now,this entire proggrame was the part of the sequesce structure"<<endl;
      cout<<endl;

// 2--> ------------------------------selection stucture-----------------------------------------
   //  if-else , else-if ladder
 cout<<" 2-->------------------------------------- selection stucture ------------------------------------- "<<endl; 
       cout<<endl;

 cout<<" if-else , else-if ladder "<<endl; 
  int standerd;
  cout<<"Tell me our standerd"<<endl;
  cin>>standerd;
  cout<<endl;
  if ((standerd<5) && (standerd>0)){
   cout<<" you are a kid now. \n";
  }
   //   using logical oppreters((standerd<5) && (standerd>0))
   /*  if we are not use (standerd>0) so we can get output of 
 else if (standerd == 0){
   cout<<"you are not born yet."<<endl;
   }*/

  else if (standerd == 5){

   cout<<"you are at middel"<<endl;
  }

  //   we can use number of else if b/w if and else 
  else if (standerd == 0){
   cout<<"you are not born yet."<<endl;
  }

  else{
   cout<<"you have to star focuse on your study."<<endl;
  }

  cout<<endl;
// another way of selection structure

// switch case
cout<<"another way of selection structure"<<endl;
cout<<"switch case"<<endl;


switch (standerd)
{
case 10:
   cout<<"focuse on your boards."<<endl;
   break;
case 5:
   cout<<"enjoy your school life."<<endl;
   break;
case 12:
   cout<<"your 100 persant focuse on your career and board exam."<<endl;
   break;

default:
cout<<"enjoy your school life."<<endl;
   break;
}
cout<<endl;
cout<<"free advice hee leni ho to lo verna jane do."<<endl;
cout<<endl;


// this is lec 10

// 3--> ----------------------------------- loop structure ------------------------------------

/* types
   1. for loop
   2. while loop
   3. do-while loop
*/   
cout<<"3--> ------------------------------ loop stucture -------------------------------------"<<endl;
cout<<"for loop stucture"<<endl;

// syntax for for loop
/* for(initialization; condition; updation)
{
 loop body(c++ code);
}*/ 

// for (size_t i = 0; i < count; i++)
// {
//    /* code */
// }


// intialization --> itput run only one time and shift to conditional
// condition --> if it's true so so go for updation pr false so break the loop
// updation--> it's update and give output and continue this loop untile it's not be false
for (int i =0; i<20;i++){
   cout<<i<<endl;
}
cout<<endl;


// -------------------------------------while loop stucture-------------------------------------
/*
cout<<"while loop stucture"<<endl;
syntex for while loop stucture
while(condition)
{
   loop body(c++ code);
}
*/
cout<<"-------------------------------------while loop stucture-------------------------------------"<<endl;
int Y=0;
while (Y<2)
{
   cout<<Y<<endl;
   Y++;
}
cout<<endl;
         // it's output bing a veriable for next loop
// ------------------------------------- do-while loop stucture -------------------------------------
 
cout<<"------------------------------------- do-while loop stucture-------------------------------------"<<endl;

 do
 {
   cout<<Y<<endl;
   Y++;
 } while (Y<10);
 
//  in all three types of loop , infinity codition is posibal...........
cout<<endl;

// exercise :------
cout<<"exercise :------"<<endl;

int Z=1;
while (Z<11)
{
   cout<<6*Z<<endl; 
   Z++; 
}

// this is lec 11

// ---------------break and continue---------------
cout<<"---------------break and continue---------------"<<endl;
cout<<endl;
cout<<"break---------------"<<endl;

for (int B = 0; B < 4; B++)
{
   cout<<B<<endl;
   if(B==2)
   break;
}
cout<<endl;
cout<<"continue---------------"<<endl;

for (int B = 0; B < 10; B++)
{
   
   if(B==2)
   continue;
   cout<<B<<endl;
}
cout<<endl;

// break--> at point break the loop and exitty
// continue--> at point skip it and continue the loop

// this is lec 12

   //   what is pointer? ----> data type which holds address of other data types.

   int m=143;
   int* M = &m;        // in pointer we have to add * and &

   // & ---> (Address of) operator 
   cout<<"The Address of m is "<<&m<<endl;
   cout<<"The Address of m is "<<M<<endl;


   // * -----> (value at ) Dereference operator
      cout<<"The value at Address M is "<<*M<<endl;

   // pointer to pointer ------> which is continue ,just add *
      int** N=&M;
         cout<<"The Address of N is "<<&M<<endl;
         cout<<"The Address of N is "<<N<<endl;
         cout<<"The value at Address N is "<<*N<<endl;
         cout<<"The value at Address N is "<<**N<<endl;
         cout<<endl;

// this is lec 13

//  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ Arrays ~~~~~~~~~~~~~~~~~~~~~~~ 

cout<<" ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ Arrays ~~~~~~~~~~~~~~~~~~~~~~~ "<<endl;
cout<<endl;

int marks[] = {34,56,7,8,89,3,35,4,56,4,56,56};

// in normal form ----------------

cout<<"in normal form ----------------"<<endl;

cout<<marks[0]<<endl;
cout<<marks[1]<<endl;
cout<<marks[2]<<endl;
cout<<marks[3]<<endl;
cout<<marks[4]<<endl;
cout<<marks[5]<<endl;
cout<<marks[6]<<endl;
cout<<marks[7]<<endl;
cout<<marks[8]<<endl;
cout<<marks[9]<<endl;
cout<<marks[10]<<endl;
cout<<marks[11]<<endl;

   //   change the value as you do in normal variables  
   marks[5] = 00;

// in form of loop ----------------- (for loop) 
cout<<"in normal for loop ----------------"<<endl;
cout<<endl;

for(int C = 0; C <12 ; C++){
   cout<<"the value of "<<C<<" is "<<setw(2)<<marks[C]<<endl;
}

// in form of loop ------------------ (while loop)
cout<<"in normal while loop ----------------"<<endl;
cout<<endl;

int D = 0 ; 
while (D<12)
{
      cout<<"the value of "<<D<<" is "<<setw(2)<<marks[D]<<endl; 
      D++;
}

// in form of loop ------------------ (Do-while loop)
cout<<"in normal Do-while loop ----------------"<<endl;
cout<<endl;

do{
   cout<<"the value of "<<D<<" is "<<setw(2)<<marks[D]<<endl; 
      D++;
}while(D<12);

// ##################################### pointer and Arrays ########################################################

cout<<"##################################### pointer and Arrays ########################################################"<<endl;

/*------------- pointer and arrays -------------
we can use pointer for a normal variables and 
array for normal variables 

so now we can use pointers for arrays*/

// in arrays we can't write like &a but write simlpy a-----

int* B = marks;  
cout<<"This is the address of marks[0] array "<<B<<endl;
cout<<"This is the address of marks[1] array "<<++B<<endl;
cout<<"This is the address of marks[6] array "<<(B+5)<<endl;
cout<<"This is the value of marks[0] array "<<*(B-1)<<endl;
cout<<"This is the address of marks[1] array "<<*B<<endl;
cout<<"This is the address of marks[2] array "<<*(B+1)<<endl;
// ?????????? point arithmetic ??????? for i
 
    /* address now = address current + i * size of data type*/

// this is lec 14
// ######################################### Structures, Unions , Enums ########################################
cout<<"######################################### Structures, Unions , Enums ########################################"<<endl;

// structures ---> are used to combine diff types of data types, just like arrays but arrays stored same type of data types 
cout<<"structers"<<endl;
typedef struct studentdata
{
   /* data */
   float inrollmentno;
   char Div;
   float SPI;
}sd;

   //   typedef---> it's use for convert in short form of long variable's name

   struct studentdata Ayushi;
   struct studentdata Honee;
   struct studentdata Prachi;

   Ayushi.Div = 'A';
   Ayushi.inrollmentno = 241250131034;
   Ayushi.SPI = 9.5;

   cout<<"information of Ayushi is :"<<endl;
   cout<<"Inrollment No.:-"<<Ayushi.inrollmentno<<endl;
   cout<<"Div.:-"<<Ayushi.Div<<endl;
   cout<<"SPI.:-"<<Ayushi.SPI<<endl;

// union ---> it's same as structer but.....
/*diff:---> structer -- we can opret all deta 
                      it's take large no of memory
            union -- we can opret only one 
                   it's take small no of memory*/

cout<<"Union"<<endl;
  union student
  {
   /* data */
   int rice;
   char car;
   float pounds;
  };
           union student s1;
           s1.rice = 34;
           cout<<s1.rice<<endl;       

// Enums---> are user-defined types which consist of named constant.
   //   enums are used to make program more readable   

cout<<"Enums"<<endl;

enum meal{ breakfast, lunch, dinner};
meal m1 = lunch;
cout<<m1;

// this is lec 15 

// function
// top down structure programming ---> functions are the imp part of it  
// what is function--> divide in parts and do work for each part  
//   "do ones and use forever"

// int main(){} ; int sum(){} ; void main (){} ; etc.... it's all are the functions
// return 0; ----> means your programming exicut succesfuly 
// if you give some o/p in return like (return c;) so at the end of this program thi fun give you this o/p
// we already use int main() so now we use int sum()

cout<<"functions"<<endl;
int no1,no2;
cout<<"enter the value of no1 = "<<endl;
cin>>no1;
cout<<"enter the value of no2 = "<<endl;
cin>>no2;
cout<<"the sum is = "<<sum(no1,no2)<<endl;
G(); // so return value is mendetri
cout<<endl;

// ########################## function prototype ############################ 
// syntext--> type function-name (arguments)
// int sum(int a, int b); --> Acceptable
// int sum(int a,  b); --> not Acceptable
// int sum(int, int); --> Acceptable

// Actual parameters-->the valus which is pass to a function --> no1 & no2

// this is lec 16
// call by value & call by reference
cout<<"call by value & call by reference"<<endl;
cout<<endl;
    int H =4, F=5;
    cout<<"The value of x is "<<H<<" and the value of y is "<<F<<endl;
    swap(H, F); 
    cout<<"The value of x is "<<H<<" and the value of y is "<<F<<endl; 
    swappointer(&H, &F);
    cout<<"The value of x is "<<H<<" and the value of y is "<<F<<endl; 
    swapReferenceVer(H, F);
    cout<<"The value of x is "<<H<<" and the value of y is "<<F<<endl; 

// this is lec 17
   //   continue.........................

return 0;
}   // it's give error bcz progamm has no idea about sum function that we apply it after main function that's why we use fnction prototype 

//  call by reference using c++ reference Variable
void swapReferenceVer(int &a, int &b){ //temp a b
    int temp = a;        //4   4  5   
    a = b;              //4   5  5
    b = temp;            //4   5  4        // Reference Variable---> x = &Y
}
//  call by reference using  pointer
void swappointer(int* a, int* b){ //temp a b
    int temp = *a;        //4   4  5   
    *a = *b;              //4   5  5
    *b = temp;            //4   5  4 
}

void swap(int a, int b){ //temp a b
    int temp = a;        //4   4  5   
    a = b;               //4   5  5
    b = temp;            //4   5  4 
}

int sum (int a, int b){
   int C= a+b;
   // Formal parameters--> which is declered by function like a & b 
   return C;
}

void G(){
   cout<<"\n Hello Good morning"<<endl;
}
// ########################## function prototype ############################ 
// syntext--> type function-name (arguments)
// int main() {
//    cout<<"########################## function prototype ############################ "<<endl;
//   return 0;
// }

