# food-ordering-system
#include <iostream>

using namespace std;
class price{
    
  public :
    int small=150;
    int regular=250;
    int large=900;
};
class pizza :public price{
    int amount;
    string choice;
   
    public :
    void choices(int a){
  switch(a){
      case 1:
      choice="chicken fazita pizza";
      
      break;
      case 2:
      choice="creamy max pizza";
      
      break;
      case 3:
      choice="peri peri pizza";
     
      break;
      case 4:
      choice="chicken bar pizza";
      default :
      cout<<"enter correct choice"<<endl;
      
      break;
  }
    }
    
 
    void bill(int x,int q){
        switch(x){
        
            case 1:
            amount=small*q;
            break;
            case 2:
            amount=regular*q;
            break;
            case 3:
            amount=large*q;
            break;
            
            default :
            cout<<"enter correct choice"<<endl;
            break;
        }
    }
    void show(){
        cout<<"***************************THANK YOU****************************"<<endl;
       cout<<"your choice is : "<<choice<<endl; 
        cout<<"your bill amount : "<<amount<<endl;
        cout<<"*********you will get your order with in 40 minutes*********"<<endl;
        
    }
  
};

class sandwich :public price{
    int amount;
    string choice;
   
    public :
    void choices(int a){
  switch(a){
      case 1:
      choice="club sandwich";
      
      break;
      case 2:
      choice="chicken crispy sandwich";
      
      break;
      case 3:
      choice="extreme vef sandwich";
     
      break;
     
      default :
      cout<<"enter correct choice"<<endl;
      
      break;
  }
    }
    
 
    void bill(int x,int q){
        switch(x){
        
            case 1:
            amount=small*q;
            break;
            case 2:
            amount=regular*q;
            break;
            case 3:
            amount=large*q;
            break;
            
            default :
            cout<<"enter correct choice"<<endl;
            break;
        }
    }
    void show(){
        cout<<"***************************THANK YOU****************************"<<endl;
       cout<<"your choice is : "<<choice<<endl; 
        cout<<"your bill amount : "<<amount<<endl;
        cout<<"*********you will get your order with in 40 minutes*********"<<endl;
        
    }
  
};

class biryani :public price{
    int amount;
    string choice;
   
    public :
    void choices(int a){
  switch(a){
      case 1:
      choice="chicken biryani";
      
      break;
      case 2:
      choice="pawn biryani";
      
      break;
      case 3:
      choice="beef biryani";
     
      break;
     
      default :
      cout<<"enter correct choice"<<endl;
      
      break;
  }
    }
    
 
    void bill(int x,int q){
        switch(x){
        
            case 1:
            amount=small*q;
            break;
            case 2:
            amount=regular*q;
            break;
            case 3:
            amount=large*q;
            break;
            
            default :
            cout<<"enter correct choice"<<endl;
            break;
        }
    }
    void show(){
        cout<<"***************************THANK YOU****************************"<<endl;
       cout<<"your choice is : "<<choice<<endl; 
        cout<<"your bill amount : "<<amount<<endl;
        cout<<"*********you will get your order with in 40 minutes*********"<<endl;
        
    }
  
};


int main()
{
    
 string name;
 cout<<"**********************CARL RESTAURANT*****************"<<endl;
 cout<<"please enter your name"<<endl;
 cin>>name;
 cout<<"HELLO "<<name<<endl;
 begin :
 cout<<"**********Menu of the Restaurant***********"<<endl;
 cout<<"1) Pizza"<<endl<<"2) sandwich"<<endl<<"3) biryani"<<endl;
    cout<<"please enter your choice"<<endl;
    int x;
    cin>>x;
    if(x==1){
        
    
    pizza pi;
  
    cout<< "1) chicken fazita pizza"<<endl;
 
  cout<<"2) creamy max pizza"<<endl;
  cout<<"3) peri peri pizza"<<endl;
   cout<<"4) chiken bar pizza"<<endl;
  cout<<" choice your flavour"<<endl;
 // cout<<" enter your flavour"<<endl;
  int k;
  cin>>k;
  if(k>4 ||k<1){
      cout<<"please enter correct choice"<<endl;
      goto begin;
  }
    pi.choices(k);
    
    cout<<"*****************we have three types of plates****************"<<endl;
    cout<<"1) small=150"<<endl;
    cout<<"2) regular=250"<<endl;
    cout<<"3) large=900"<<endl;
    
    cout<<"please enter your choice"<<endl;
  
    int a;
    cin>>a;
    if(a<1 ||a>3){
    cout<<"please enter correct choice"<<endl;
    goto begin;
}
    cout<<"enter the quantity of order"<<endl;
    int q;
    cin>>q;

pi.bill(a,q);
pi.show();
cout<<"******* if want to order more thing enter Y/y"<<endl;
char c;
cin>>c;
if(c=='Y'||c=='y') goto begin;
//break;

}else{
    
if(x==2){
sandwich s;
    cout<< "1) club sandwich"<<endl;
 
  cout<<"2)chicken crispy sandwich"<<endl;
  cout<<"3) veg sandwich"<<endl;
  
  cout<<" choice your flavour"<<endl;
 // cout<<" enter your flavour"<<endl;
  int d;
  cin>>d;
  if(d>3 ||d<1){
      cout<<"please enter correct choice"<<endl;
      goto begin;
  }
    s.choices(d);
    
    cout<<"*****************we have three types of plates****************"<<endl;
    cout<<"1) small=150"<<endl;
    cout<<"2) regular=250"<<endl;
    cout<<"3) large=900"<<endl;
    
    cout<<"please enter your choice"<<endl;
  
    int e;
    cin>>e;
    if(e<1 ||e>3){
    cout<<"please enter correct choice"<<endl;
    goto begin;
}
    cout<<"enter the quantity of order"<<endl;
    int f;
    cin>>f;

s.bill(e,f);
s.show();
cout<<"******* if want to order more thing enter Y/y"<<endl;
char g;
cin>>g;
if(g=='Y'||g=='y') goto begin;

}
else{
    if(x==3){
   biryani b;
    cout<< "1) chicken biryani"<<endl;
 
  cout<<"2)pawn biryani"<<endl;
  cout<<"3) beef biryani"<<endl;
  
  cout<<" choice your flavour"<<endl;
 // cout<<" enter your flavour"<<endl;
  int h;
  cin>>h;
  if(h>3 ||h<1){
      cout<<"please enter correct choice"<<endl;
      goto begin;
  }
    b.choices(h);
    
    cout<<"*****************we have three types of plates****************"<<endl;
    cout<<"1) small=150"<<endl;
    cout<<"2) regular=250"<<endl;
    cout<<"3) large=900"<<endl;
    
    cout<<"please enter your choice"<<endl;
  
    int i;
    cin>>i;
    if(i<1 ||i>3){
    cout<<"please enter correct choice"<<endl;
    goto begin;
}
    cout<<"enter the quantity of order"<<endl;
    int j;
    cin>>j;

b.bill(i,j);
b.show();
cout<<"******* if want to order more thing enter Y/y"<<endl;
char k;
cin>>k;
if(k=='Y'||k=='y') goto begin;
 
}
else
cout<<"please enter correct choice"<<endl;
goto begin;
}

}
    return 0;
}

