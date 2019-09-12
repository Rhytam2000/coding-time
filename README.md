WAP to check the number is palindrome or not.

#include<stdio.h>
void main()
{
int d,rev,n=0;
printf("Enter a number");
scanf("%d",&n);
while(n!=0)
{
d=n%10;
rev=(rev*10)+d;
n=n/10;
}
if(rev==n)
printf("the number is palindrome");
else
printf("the number is not a palindrome")
}

// now we will do the dry run of the above program
//  n         d       rev
    0         0        0
    153       3        3
    15        5        35
    1         1        351
    // because n=0 after further incrementation, so it will proceed out of the loop
       and then it checks whether rev=n
       and displays the answer accordingly!!!
