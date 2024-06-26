# PowerFunction-Code-in-Java-Practive-Task-Lab

```Java
public class PowerFunction{
    public static double Power(double x, int y){
        if(y == 0){
            return 1;
        }else if(y < 0){
            return 1/Power(x, -y);
        }else{
            return (x * Power(x, y-1));
        }
    }
    public static void main(String[] args) {
        
        double x = 2.5;
        int y = 4;
        System.out.println(x + "Power" + y + "=" + Power(2.5, 4));
    }
}
```
![image](https://github.com/ARIBFIB/PowerFunction-Code-in-Java-Practive-Task-Lab/assets/125716994/68a7b078-40b6-4094-a187-b61a1642b0c5)

![image](https://github.com/ARIBFIB/PowerFunction-Code-in-Java-Practive-Task-Lab/assets/125716994/150f5058-9ed9-4530-9af3-8f9fb9aaa605)

Sure, here's a suggested README.md file for the PowerFunction Java program:

# Power Function in Java ![][]

This is a Java program that demonstrates a recursive function to compute the value of x raised to the power of y (x^y).

## Table of Contents
- [Description](#description)
- [Usage](#usage)
- [Call Stack Diagram](#call-stack-diagram)
- [Output](#output)
- [Contributing](#contributing)
- [License](#license)

## Description
The program defines a `PowerFunction` class with two methods:

- `power(double x, int y)`: A recursive function that calculates the value of `x` raised to the power of `y`.
- `main(String[] args)`: The entry point of the program, which calls the `power()` function with `x = 2.5` and `y = 4`, and prints the result.

## Usage
To run the program, you can copy the following code and save it in a file named `PowerFunction.java`:```java
public class PowerFunction {
    public static double power(double x, int y) {
        if (y == 0) {
            return 1;
        } else if (y < 0) {
            return 1 / power(x, -y);
        } else {
            return x * power(x, y - 1);
        }
    }

    public static void main(String[] args) {
        double x = 2.5;
        int y = 4;
        double result = power(x, y);
        System.out.println(x + "^" + y + " = " + result);
    }
}```

Then, compile and run the program using the following commands:```
javac PowerFunction.java
java PowerFunction```

## Call Stack Diagram
The following diagram shows the call stack as the `power()` function calls itself recursively:![Power Function Call Stack][]

## Output```
2.5^4 = 39.0625```

## Contributing
Contributions are welcome! If you find any issues or have suggestions for improvements, please feel free to open an issue or submit a pull request.

## License
This project is licensed under the [MIT License](LICENSE).
