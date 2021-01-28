# Car-Parking-Program

#include<stdio.h>
#include<conio.h>
int Menu();
void Bus();
void Cycle();
void Riksha();
void Delete();
void ShowDelete();
int nor=0,nob=0,noc=0,amount=0,count=0;
void main()
{
	clrscr();
	switch(Menu())
	{
	 case 1:
	 	Bus();
	 	break;
	 case 2:
	 	Cycle();
	 	break;
	 case 3:
	    Riksha();
	 	break;	
	 case 4:
	    Showdetail();
	 	break;	
	 case 5:
	 	Delete();
	 	break;
	 default:
	 	printf("\n Invalid choice :");	
	}
	
	getch();
	
}
int Menu()
{
	int ch;
	printf("\n 1, Enter bus : ");
	printf("\n 2, Enter cucle : ");
	printf("\n 3, Enter riksha : ");
	printf("\n 4, Show status : ");
	printf("\n 5, Delete data : ");
	printf("\n 6, Enter your choice : \n");
	scanf("%d",&ch);
	return(ch);
	
}
void Delete()
{
	nob=0;
	noc=0;
	nor=0;
	amount=0;
	count=0;
	 
void ShowDetail()
{
	printf("\n Number of bus=%d",nob);
	printf("\n Number of cycle=%d",noc);
	printf("\n Number of riksha=%d",nor);
	printf("\n Total no of vehicle=%d",count);
	printf("\n Total gain amount=%d",amount);
	
}
void Riksha()
{
	nor++;
	amount=amount+50;
	
	
}
void Cycle()
{
	noc++;
	amount=amount+20;
	count++;
	
}
void Bus()
{
	nob++;
	amount=amount+100;
	count++;
	
}
