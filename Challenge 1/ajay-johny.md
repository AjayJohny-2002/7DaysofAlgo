/***************************
 Author : Ajay Johny
 progrm des : Program to print whether a number is prime or not
 version : 1.0
 date : 21/06/2021
 ***************************/
#include<stdio.h>

int main(){
    
    int number;
    printf(" Enter the number to check it is prime or not : \t");
    scanf("%d",&number);

    if(number==1 || number==0){
        printf("\nThe number 0 nd 1 is neither prime nor composite");
    }else if(number<0){
        printf("\n Please enter a positive number");
    }else if( number==2 || number==3 || number==5 || number==7 ){
        printf("\nThe number %d is a prime number",number);
    }else if( number%2==0 || number%3==0 || number%5==0 || number%7==0 ){
        printf("\nThe number %d is not a prime number",number);
    }else{
        printf("\nThe number %d is a prime number",number);
    }


    return 0;
}