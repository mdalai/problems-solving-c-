## Basic syntax
```c++
#include <iostream>
int main() {
  std::cout << "Hello World!!!" << "\n";
  return 0;
}
```
## Control Flow
### If else statement
```c++
#include<iostream>

int main()
{
   char location; 
   
   std::cout<<"Would you like an animal that lives in water(w), land(l), or both(b)?";
   std::cin>>location;
   std::cout<<location<<"\n";
   
   //Use if-else statements to control program flow
   if (location=='w'){
       std::cout<<"Get a fish"<<"\n";  
   } else if(location=='l'){
       std::cout<<"Get a gecko"<<"\n";
   } else{
       std::cout<<"Get a frog"<<"\n";
   }
      
   return 0;
}
```
### Switch statement
```c++
#include <iostream>

int main()
{
    int menuItem = 1;
    
    std::cout<<"What is your favorite winter sport?: \n";
    std::cout<<"1.Skiing\n2: Sledding\n3: Sitting by the fire";
    std::cout<<"\n4.Drinking hot chocolate\n";
    std::cout<<"\n\n";
    
    switch(menuItem)
    {
        case(1): std::cout<<"Skiing?! Sounds dangerous!\n";
                 break;
        case(2): std::cout<<"Sledding?! Sounds like work!\n";
                 break; 
        case(3): std::cout<<"Sitting by the fire?! Sounds warm!\n";
                 break;
        case(4): std::cout<<"Hot chocolate?! Yum!\n";
                 break;
        default: std::cout<<"Enter a valid menu item";
    }
    return 0;
}
```
### For loops
```c++
#include<iostream>
int main(){
    int inp;
    float sum = 0;
    
    for(int i=0; i<5; i++){
        std::cout<<"Enter number "<<i<<":\n";
        std::cin>>inp;
        sum = sum + inp;
    }
    
    std::cout<<"The sum = "<<sum<<"\n";
    std::cout<<"The average = "<<sum/5;
}
```
### while loop
```c++
#include<iostream>

int main()
{
    int a = 0;
    while(a < 5)
    {
        std::cout<<"a = "<<a<<"\n";       
        a++;
        if(a == 3)
            break;
    }
    std::cout<<"The first statement after the first while loop\n\n";
    
    
    while(a < 15)
    {
        a++;
        if(a == 10)
        {
            std::cout<<"\tWhen a=10, go back to the top of the loop";
            std::cout<<"\n\tThis means a=10 is skipped.\n";
            continue;
        }
        std::cout<<"After continue a = "<<a<<"\n";           
    }
    return 0;
}
```
