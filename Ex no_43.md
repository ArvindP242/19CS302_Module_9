# EX 43 C program to Write a function to display queue elements using array.
## DATE:
## AIM:
To Write a function to display queue elements using array.

## Algorithm:
1. Start. 
2. Define a variables. 
3. Write a function to display queue elements using array. 
4. Read the value using scanf. 
5. Ask the user to make an input. 
6. Print out the answer. 
7. End.

## Program:
```
#include <stdio.h>
int main(){
char queue[MAX];
int front = -1;
int rear = -1;

void enqueue(char val) {
    if (rear == MAX - 1) {
        printf("Queue is full\n");
        return;
    }
    if (front == -1) {
        front = 0;
    }
    rear++;
    queue[rear] = val;
}

void display() {
    if (front == -1 || front > rear) {
        printf("no elements to display\n");
    } else {
        for (int i = front; i <= rear; i++) {
            printf("%c ", queue[i]);
        }
        printf("\n");
    }
}
```

## Output:

![image](https://github.com/user-attachments/assets/6b1348f5-936d-4b8f-9478-3a848914c08c)


## Result:
Thus the program was executed and the output was verified successfully.
