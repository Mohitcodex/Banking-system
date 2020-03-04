#include<iostream>
#include<conio.h>

using namespace std;

class bank
{ 
public:

char name[10],add[10],y;
int balance,a;
 float amount;
 
	public:
		void open_account();
		void deposite_money();
		void withdraw_money();
		void display_account();
		
};

void bank::open_account()
{   cout<<"\t\t******************************************************************************************\n";
	cout<<"\t\t*******************************[WELCOME TO MOHIT BANK]************************************\n"; 
	cout<<"\t\t******************************************************************************************\n";
	cout<<endl<<endl;
	cout<<"\t\t\t\t\t\tENTER YOUR FULL NAME = ";
	cin>>name;
	cout<<endl<<endl;
	cout<<"\t\t\t\t\t\tENTER YOUR ADDRESS= ";
	cin>>add;
	cout<<endl<<endl;
	cout<<"\t\t\t\t\t\t PRESS (S)=SAVING && (C)=CURRENT ";
	cin>>y;
	cout<<endl<<endl;
	cout<<"\t\t\t\t\t\tENTER THE AMOUNT TO DEPOSITE=";
	cin>>balance;
	cout<<endl<<endl<<endl<<endl<<endl;
	cout<<"\t\t\t\t\t\t A C O U N T   C R E A T E D \n\n\n";
	
	
}

void bank::deposite_money()
{   
cout<<endl<<endl;
	cout<<"\t\t\t\t\t\tENTER DEPOSITE AMOUNT =";
	cin>>a;
	balance=balance+a;
	cout<<endl<<endl;
	cout<<"\t\t\t\t\t\tTOTAL BALANCE AVALIABLE="<<balance;
	
}

void bank::display_account()
{
	
	cout<<"\t\t\t\t\t\tYOUR FULL NAME ="<<name;
	cout<<endl<<endl;
	cout<<"\t\t\t\t\t\tYOUR ADDRESS ="<<add;
	cout<<endl<<endl;
    cout<<"\t\t\t\t\t\tTYPE OF ACCOUNT THAT YOU OPPET ="<<y;
	cout<<endl<<endl;
	cout<<"\t\t\t\t\t\tTOTAL AMOUNT  YOU DEPOSITE ="<<balance;
	cout<<endl<<endl;
	

}

void bank::withdraw_money()
{   

	cout<<"\t\t\t\t\t\tWITHDRAW = \n";
	cout<<"\t\t\t\t\t\tENTER AMOUNT TO WITHDRAW =";
	cin>>amount;
	balance=balance-amount;
	
	cout<<endl<<endl<<endl;
	cout<<"\t\t\t\t\t\tTOTAL AMOUNT LEFT = "<<balance;
	
}

int main()

{
	 
	 
	 bank obj;
int ch,x;
 
 
 do
 {  cout<<endl<<endl<<endl;
    cout<<"\t\t ___________W E L C O M E    T O   M O H I T    B A N K    O F    B A R O D A _____________\n\n\n";
	cout<<"\t\t*******************************************************************************************\n";
    cout<<"\t\t*******************************************************************************************\n\n\n";

    
    cout<<"\t\t  1-> OPEN YOUR ACCOUT\n";
    cout<<"\t\t     *****************\n\n";
	cout<<"\t\t  2-> DEPOSITE MONEY    \n";
	cout<<"\t\t     *****************\n\n";
	cout<<"\t\t  3-> WITHDRAW AMOUNT \n";
	cout<<"\t\t     *****************\n\n";
	cout<<"\t\t  4-> DISPLAY ACCOUNT   \n";
	cout<<"\t\t     *****************\n\n";
	cout<<"\t\t  5->EXIT \n";
	cout<<"\t\t     *****************\n\n\n";
	cout<<"\t\t  *->SELECT A OPTION =";
	cin>>ch;
	cout<<endl;
	cout<<"\t\t ___________ C R E A T E D   B Y   M O H I T   S I N G H   C H A U H A N ___________________\n\n\n\n\n";
	
	switch(ch)
	{
		case 1:cout<<"\t\t\t\t\t\t N E W   A C C O U N T \n\n";
		
		obj.open_account();
		break;
		
		case 2:cout<<"\t\t\t\t\t\t D E P O S I T E  M O N E Y \n\n";                    
		obj.deposite_money();
		break;
		
		case 3:cout<<"\t\t\t\t\t\t W I T H D R A W  M O N E Y \n\n";
		obj.withdraw_money();
		break;
		
		case 4:cout<<"\t\t\t\t\t\t D I S P L A Y  M O N E Y \n\n";
		obj.display_account();
		break;
		
		case 5:
			
		if(ch==5)
		{
			exit(1);
		}
	
default:

cout<<"THIS IS NO EXIST TRY AGAIN \n";
}

cout<<endl<<endl<<endl;

cout<<"\t\t\t\t\t\t DO TO SELECT NEXT OPPTIN THEN PRESS (Y) \n\n";
cout<<"\t\t\t\t\t\t IF YOU WANT TO EXIT THEN PRESS (N) \n\n";
x=getch();
cout<<endl<<endl<<endl<<endl;
if(x=='n'||x=='N')
{

cout<<"\t\t\t\t\t  T H A N K Y O U    V I S I T   A G A I N \n\n";
exit(0);
}
}


while(x=='y'|| x=='Y');
getch();
return 0;


}

	
		
	
						
