#include<iostream>
#include<cstdlib>
#include<ctime>
using namespace std;
int main()
{   int num;
    srand(static_cast<unsigned int>(time(nullptr)));
    int secretNumber=rand()%100+1;
    for(int i=1;i<=5;i++) {
     cout<<"You has 5 tries"<<endl;
     cout<<"guess a number (between 1-100)"<<endl;
    cin>>num;
    if(num>secretNumber)
    cout<<"It's too High"<<endl;
   else if(num<secretNumber)
    cout<<"It's too low"<<endl;
    else if(num<0&&num>100)
    {
        cout<<"Please Enter a number between 1-100";
    }
    else 
    {
    cout<<"Congratulations!You guessed the correct number";
    exit(0);
    }
    }
    return 0;
    

}
