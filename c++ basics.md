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
