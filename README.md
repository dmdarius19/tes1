#include <stdio.h>
int sum_odd_n(int n){
    if (n==1){
        return 1;
    }else{
        return (2*n-1) + sum_odd_n(n-1);
    }
}

int main(){
    int n;
    printf("Enter the value of n: ");
    scanf("%d", &n);
    printf("Sum of odd numbers from 1 to %d: %d\n",2*n-1, sum_odd_n(n));
    return 0;
}