# Experiment---18  

### Aim 
To study and implement Stack implementation in C++ using array. <br> 
Menu options - <ol><li> Push </li> <li> Pop </li> <li>Display</li><li>Exit</li></ol>

### Software 
Visual Studio Code 

### Theory 
A <b>Stack</b> is an abstract data stucture that contains a collection of elements. Stack implements the <b>LIFO</b> (Last In First Out) mechanism i.e., the element that is pushed at the end is popped out first. Some of the principle operations in the stack are - <ol><li>Push - This adds a data value to the top[ of the stack.</li><li>Pop - This removes the data value on the top of the stack.</li><li>Peek - This returns the top value of the stack.</li></ol> 

### Code
(A) 
```
// NAME - SHLOKA PATEL 
// PRN - 23070123120 
// EXPERIMENT - 18(A) 

// STACK 

#include<iostream>
using namespace std;

int stack[100], n = 100, top = -1;

void push(int val) {
    if (top >= n - 1) {  // Correct condition for Stack Overflow
        cout << "Stack Overflow" << endl;
    } else {
        top++;
        stack[top] = val;
    }
}

void pop() {
    if (top <= -1) {
        cout << "Stack Underflow" << endl;
    } else {
        cout << "The popped element is " << stack[top] << endl;
        top--;
    }
}

void display() {
    if (top >= 0) {
        cout << "Stack elements are: ";
        for (int i = top; i >= 0; i--)
            cout << stack[i] << " ";
        cout << endl;
    } else {
        cout << "Stack is empty" << endl;
    }
}

int main() {
    int ch, val;
    cout << "(1) Push in Stack" << endl;
    cout << "(2) Pop from Stack" << endl;
    cout << "(3) Display Stack" << endl;
    cout << "(4) Exit" << endl;

    do {
        cout << "Enter Choice: " << endl;
        cin >> ch;
        switch (ch) {
            case 1:
                cout << "Enter value to be pushed: " << endl;
                cin >> val;
                push(val);
                break;
            case 2:
                pop();
                break;
            case 3:
                display();
                break;
            case 4:
                cout << "Exit" << endl;
                break;
            default:
                cout << "Invalid Choice." << endl;
        }
    } while (ch != 4);

    return 0;
}
```

(B) 
```
```

(C) 
```
```

### Output 
(A) <br> 
![]() 

(B) <br> 
![]() 

(C) <br> 
![]() 

### Conclusion 
