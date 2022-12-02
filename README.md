# Fibonacci
Fibonacci is a sequence of numbers staring from 0 until an infinite number of additions of the N-1 and N-2. With N being the current value. For example we can look at the sequence which is 0 1 1 2 3 5 8 13 21 34 55 and so on. So the formula to actually get each value within the Fibonacci sequence N = Current value within the sequence being N - 1 + N -2 for example we could look at value 5 which is 3 so how to get 3 would be N - 1 which is 2 and N - 2 which is 1 so 2 + 1 = 3. The only rule within the sequence is the first N value has to be 0 and the second N value has to be 1.
# Fibonacci Iterative
```c
int fibonacciIterative(int N){
    int num1=0;
    int num2=1;
    int output;

    if (N==0) {
        return num1;
    } else if (N==1){
        return num2;
    } else {
        for (int i = 2; i<= N; i++){ 
            output = num1+num2;
            num1 = num2;
            num2 = output;
        }
        return output;
    }
}
```
#Fibonacci Recursive
```c
int fibonacciRecursive (int N){
    if (N==0){
        return 0;
    } else if (N==1){
        return 1;
    } else {
        return fibonacciRecursive(N - 1) + fibonacciRecursive(N-2);
    }
}
```
![Gay](images/same.png)
