//# data-stracture-lab-3

Program 1: Push last 4 digits of your ID and display.
Source code:
#include<stdio.h>
#define MAX 4
int stack [MAX],i,top=-1;
void push( int n){
    if(top == MAX-1){
        printf("Overflow...%d\n",n);
    }
    else{
        top++;
        stack[top] = n;
        printf("Pushed %d in stack.\n",n);
    }
}
void display(){
    if(top == -1){
        printf("Empty stack...\n");
    }
    else{
        printf("Element of stack is = ");
        for( i = 0; i<= top; i++){
            printf("%d", stack[i]);
        }
        printf("\n\n");
    }
}
int main(){
    push(2);
    push(3);
    push(7);
    push(4);
    display();
  return 0;
}
Output:
 





Program 2: Push another element and display overflow message.
Source code:
#include<stdio.h>
#define MAX 4
int stack[MAX],top=-1;
void push( int n){
    if( top == MAX-1 ){
        printf("Overflow stack...Can't pushed %d in stack!\n",n);
    }
    else{
        top++;
        stack[top] = n;
        printf("Pushed %d in stack\n",n);
    }
}
void display(){
    if( top == -1){
        printf("Empty stack!\n");
        return;
    }
}
int main(){
    push(1);
    push(2);
    push(3);
    push(4);
    push(12);//This vlaue will be show as overflow.
    display();
  return 0;
}
Output:
 

Program 3: Pop one element and display
Source code:
#include<stdio.h>
#define MAX 4
int stack [MAX],top=-1,i;
void push(int n){
    if( top == MAX-1 ){
        printf("Overflow stack...Can,t pushed %d\n",n);
    }
    else{
        top++;
        stack [top] = n;
        printf("Pushed %d in stack\n",n);
    }
}
void pop(){
    if( top == -1){
        printf("Underflow stack...can,t pop from stack.\n");
    }
    else{
        printf("Pop %d from stack.\n",stack[top]);
 top--;
    }
}
void dis(){
printf("Before poped element of stack is = ");
 for( i = 0; i<=top; i++){
            printf("%d ", stack[i]);
        }
printf("\n\n");
}
void display(){
    if( top == 1){
        printf("Empty stack\n");
    }
    else{
        printf("After poped element of stack is: ");
        for( i = 0; i<=top; i++){
            printf("%d ", stack[i]);
        }
        printf("\n\n");
    }
}
int main(){
    push(10);
    push(20);
    push(30);
    push(40);
    dis();
    pop();
    display();
    return 0;
}
Output:
 

Program 4: Pop remaining three elements and display.
Source code:
#include <stdio.h>
#define MAX 4
int stack[MAX],i,top = -1;
void push( int n){
    if( top == MAX-1 ){
        printf("Overflow stack...can't pushed in stack %d\n",n);
    }
    else{
        top++;
        stack[top] = n;
        printf("Pushed %d in stack\n",n);
    }
}
void dis(){
    printf("Before poped element of stack is = ");
        for( i = 0; i<=top; i++){
            printf("%d ", stack[i]);
        }
        printf("\n\n");
}
void pop(){
    if( top == -1){
        printf("Underflow stack.\n");
    }
    else{
        printf("Poped %d from stack.\n",stack[top]);
        top--;
    }
}
void display(){
    if( top == -1){
        printf("Empty stack.\n");
    }
    else{
        printf("After poped element of stack is = ");
        for( i = 0; i<=top; i++){
            printf("%d", stack[i]);
        }
        printf("\n\n");
    }
}
int main(){
    push(1);
    push(0);
    push(1);
    push(0);
    dis();
    pop();
    pop();
    pop();
    display();

   return 0;
}


Output:
 

Program 5: Pop again and display underflow message.
Source code:
#include<stdio.h>
#define MAX 4
int stack[MAX],i,top=-1;
push( int n){
    if( top == MAX-1){
        printf("Overflow stack...Can't pushed in stack %d\n",n);
    }
    else{
        top++;
        stack[top] = n;
        printf("Pushed %d in stack\n ",n);
    }
}
void dis(){
        printf("Before poped element of stack is = ");
        for(i =0; i<=top; i++){
            printf("%d ",stack[i]);
        }
        printf("\n\n");
}
void pop(){
    if( top == -1){
        printf("Underflow stack.\n");
    }
    else{
        printf("Poped %d from stack\n",stack[top]);
        top--;
    }
}
void display(){
    if( top == -1){
        printf("Empty stack.\n");
    }
    else{
        printf("After poped element of stack is = ");
        for(i =0; i<=top; i++){
            printf("%d ",stack[i]);
        }
        printf("\n\n");
    }
}
int main(){
    push(11);
    push(22);
    push(33);
    push(44);
    dis();
    pop();
    pop();
    pop();
    pop();
    pop();
    return 0;
}

Output:
 











