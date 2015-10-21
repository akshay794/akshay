#include<iostream.h>
#include<conio.h>
class personaldetail
{
		private: char name[20],add[20];
		  	int roll,zip;
		public: personaldetail ( );//Constructor
			~stu( );//Destructor
			void read( );
			void disp( );			// display funtion
};
personaldetail :: personaldetail( )
{
	cout<<”This is personal Details”<<endl;
}
void stu :: read( )
{
	cout<<”Enter the  name”;
	cin>>name;
	cout<<”Enter the Id_No “;
	cin>>Id_No;
	cout<<”Enter the address”;
	cin>>address;
	cout<<”Enter the Zipcode”;
	cin>>zipcode;
}
void personaldetail :: disp( )
{
	cout<<”Student Name :”<<name<<endl;
	cout<<”Roll no   is       :”<<Id_No<<endl;
	cout<<”Address is       :”<<address<<endl;
	cout<<”Zipcode is       :”<<zip;
}
personaldetail : : ~personaldetail( )
{
	cout<<”details is Closed”;
}
 
void main( )
{
	personaldetail s;
	clrscr( );
s.read ( );
s.disp ( );
getch( );
}
