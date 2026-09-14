# Java
_Q1. Write a Java program to display your name, age, and college name using variables of appropriate data type_
.
public class {
    public static void main(String[] args) {
        String name = "Aryan";
        int age = 20;
        String college = "COER University";

        System.out.println("Name: " + name);
        System.out.println("Age: " + age);
        System.out.println("College: " + college);
    }
}

Output:
Name: Aryan
Age: 20
College: COER University


Q2. Input two integers and print the result of all arithmetic operations (addition, subtraction, multiplication, division, and modulus).
import java.util.Scanner;

public class Q2 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter first number: ");
        int a = sc.nextInt();

        System.out.print("Enter second number: ");
        int b = sc.nextInt();

        System.out.println("Addition = " + (a + b));
        System.out.println("Subtraction = " + (a - b));
        System.out.println("Multiplication = " + (a * b));
        System.out.println("Division = " + (a / b));
        System.out.println("Modulus = " + (a % b));
    }
}

Output:
Enter first number: 20
Enter second number: 5
Addition = 25
Subtraction = 15
Multiplication = 100
Division = 4
Modulus = 0


Q3. Write a Java program to check whether a given number is even or odd using the modulus operator and if-else.
import java.util.Scanner;

public class Q3 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter a number: ");
        int n = sc.nextInt();

        if (n % 2 == 0) {
            System.out.println("Even number");
        } else {
            System.out.println("Odd number");
        }
    }
}

Output:
Enter a number: 12
Even number


Q4. Write a program to demonstrate the use of relational operators by comparing two numbers.
import java.util.Scanner;

public class Q4 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter first number: ");
        int a = sc.nextInt();

        System.out.print("Enter second number: ");
        int b = sc.nextInt();

        System.out.println("a == b: " + (a == b));
        System.out.println("a != b: " + (a != b));
        System.out.println("a > b: " + (a > b));
        System.out.println("a < b: " + (a < b));
        System.out.println("a >= b: " + (a >= b));
        System.out.println("a <= b: " + (a <= b));
    }
}
Output:
Enter first number: 10
Enter second number: 5
a == b: false
a != b: true
a > b: true
a < b: false
a >= b: true
a <= b: false

Q5. Accept a floating-point number and convert it explicitly to an integer. Print both the original and the converted values.
import java.util.Scanner;

public class Q5 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter a floating-point number: ");
        double num = sc.nextDouble();

        int converted = (int) num;

        System.out.println("Original value: " + num);
        System.out.println("Converted value: " + converted);
    }
}

Output:
Enter a floating-point number: 25.75
Original value: 25.75
Converted value: 25


Q6. Write a program to accept a character and print its ASCII value.
import java.util.Scanner;

public class Q6 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter a character: ");
        char ch = sc.next().charAt(0);

        int ascii = (int) ch;

        System.out.println("Character: " + ch);
        System.out.println("ASCII value: " + ascii);
    }
}

Output:
Enter a character: A
Character: A
ASCII value: 65


Q7. Input a number and check if it is divisible by both 3 and 5 using logical operators.
import java.util.Scanner;

public class Q7 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter a number: ");
        int n = sc.nextInt();

        if (n % 3 == 0 && n % 5 == 0) {
            System.out.println("Number is divisible by both 3 and 5");
        } else {
            System.out.println("Number is not divisible by both 3 and 5");
        }
    }
}

Output:
Enter a number: 30
Number is divisible by both 3 and 5


Q8. Input a character and check whether it is a vowel or a consonant using if-else.
import java.util.Scanner;

public class Q8 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter a character: ");
        char ch = sc.next().charAt(0);

        if (ch == 'a' || ch == 'e' || ch == 'i' ||
            ch == 'o' || ch == 'u' ||
            ch == 'A' || ch == 'E' || ch == 'I' ||
            ch == 'O' || ch == 'U') {
            
            System.out.println("Vowel");
        } else {
            System.out.println("Consonant");
        }
    }
}

Output:
Enter a character: E
Vowel


Q9. Input marks of three subjects, calculate total and percentage, and print pass/fail using if-else (passing criteria: >=40% in all subjects).
import java.util.Scanner;

public class Q9 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter marks of subject 1: ");
        float m1 = sc.nextFloat();

        System.out.print("Enter marks of subject 2: ");
        float m2 = sc.nextFloat();

        System.out.print("Enter marks of subject 3: ");
        float m3 = sc.nextFloat();

        float total = m1 + m2 + m3;
        float percentage = total / 3;

        System.out.println("Total = " + total);
        System.out.println("Percentage = " + percentage + "%");

        if (m1 >= 40 && m2 >= 40 && m3 >= 40) {
            System.out.println("Result: Pass");
        } else {
            System.out.println("Result: Fail");
        }
    }
}

Output:
Enter marks of subject 1: 70
Enter marks of subject 2: 65
Enter marks of subject 3: 80
Total = 215.0
Percentage = 71.666664%
Result: Pass


Q10. Write a program to find the greatest of two numbers using if-else.
import java.util.Scanner;

public class Q10 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter first number: ");
        int a = sc.nextInt();

        System.out.print("Enter second number: ");
        int b = sc.nextInt();

        if (a > b) {
            System.out.println(a + " is the greatest");
        } else if (b > a) {
            System.out.println(b + " is the greatest");
        } else {
            System.out.println("Both numbers are equal");
        }
    }
}

Output:
Enter first number: 25
Enter second number: 40
40 is the greatest


import java.util.Scanner;

class LargestThree {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter three numbers: ");
        int a = sc.nextInt();
        int b = sc.nextInt();
        int c = sc.nextInt();

        if (a > b) {
            if (a > c)
                System.out.println("Largest = " + a);
            else
                System.out.println("Largest = " + c);
        } else {
            if (b > c)
                System.out.println("Largest = " + b);
            else
                System.out.println("Largest = " + c);
        }
    }
}

2.import java.util.Scanner;

class LeapYear {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter year: ");
        int year = sc.nextInt();

        if (year % 400 == 0)
            System.out.println("Leap Year");
        else if (year % 100 == 0)
            System.out.println("Not a Leap Year");
        else if (year % 4 == 0)
            System.out.println("Leap Year");
        else
            System.out.println("Not a Leap Year");
    }
}

13.import java.util.Scanner;

class NumberCheck {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter a number: ");
        int n = sc.nextInt();

        if (n > 0)
            System.out.println("Positive number");
        else if (n < 0)
            System.out.println("Negative number");
        else
            System.out.println("Zero");
    }
}

14. import java.util.Scanner;

class Armstrong {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter a 3-digit number: ");
        int n = sc.nextInt();

        int original = n;
        int sum = 0;

        if (n >= 100 && n <= 999) {
            while (n > 0) {
                int digit = n % 10;
                sum = sum + digit * digit * digit;
                n = n / 10;
            }

            if (sum == original)
                System.out.println("Armstrong number");
            else
                System.out.println("Not an Armstrong number");
        } else {
            System.out.println("Enter a 3-digit number");
        }
    }
}

Output:
Enter a 3-digit number: 153
Armstrong number
16. Calculate Tax

15. import java.util.Scanner;

class TaxCalculator {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter income: ");
        double income = sc.nextDouble();
        double tax;

        if (income <= 250000)
            tax = 0;
        else if (income <= 500000)
            tax = income * 0.05;
        else if (income <= 1000000)
            tax = income * 0.20;
        else
            tax = income * 0.30;

        System.out.println("Tax = " + tax);
    }
}

Output:
Enter income: 600000
Tax = 120000.0
17. Palindrome Number

 16. import java.util.Scanner;

class Palindrome {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter a number: ");
        int n = sc.nextInt();

        int original = n;
        int reverse = 0;

        while (n > 0) {
            int digit = n % 10;
            reverse = reverse * 10 + digit;
            n = n / 10;
        }

        if (reverse == original)
            System.out.println("Palindrome number");
        else
            System.out.println("Not a palindrome number");
    }
}

Output:
Enter a number: 1221
Palindrome number

(18. Prime Number)
import java.util.Scanner;

class PrimeCheck {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter a number: ");
        int n = sc.nextInt();
        int count = 0;

        if (n >= 2) {
            for (int i = 1; i <= n; i++) {
                if (n % i == 0)
                    count++;
            }

            if (count == 2)
                System.out.println("Prime number");
            else
                System.out.println("Not a prime number");
        } else {
            System.out.println("Not a prime number");
        }
    }
}

Output:
Enter a number: 17
Prime number

19. Operator and Calculation
    
import java.util.Scanner;

class Calculator {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter two numbers: ");
        double a = sc.nextDouble();
        double b = sc.nextDouble();

        System.out.print("Enter operator (+, -, *, /): ");
        char op = sc.next().charAt(0);

        if (op == '+')
            System.out.println("Result = " + (a + b));
        else if (op == '-')
            System.out.println("Result = " + (a - b));
        else if (op == '*')
            System.out.println("Result = " + (a * b));
        else if (op == '/') {
            if (b != 0)
                System.out.println("Result = " + (a / b));
            else
                System.out.println("Cannot divide by zero");
        } else
            System.out.println("Invalid operator");
    }
}
Output:
Enter two numbers: 20 5
Enter operator (+, -, *, /): *
Result = 100.0
20. Marriage Eligibility
import java.util.Scanner;

class MarriageEligibility {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter age: ");
        int age = sc.nextInt();

        System.out.print("Enter gender (M/F): ");
        char gender = sc.next().charAt(0);

        if (gender == 'M' || gender == 'm') {
            if (age >= 21)
                System.out.println("Eligible for marriage");
            else
                System.out.println("Not eligible for marriage");
        } else if (gender == 'F' || gender == 'f') {
            if (age >= 18)
                System.out.println("Eligible for marriage");
            else
                System.out.println("Not eligible for marriage");
        } else {
            System.out.println("Invalid gender");
        }
    }
}
Output:
Enter age: 22
Enter gender (M/F): M
Eligible for marriage
Advanced Level
21. Valid Triangle
import java.util.Scanner;

class TriangleCheck {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter three angles: ");
        int a = sc.nextInt();
        int b = sc.nextInt();
        int c = sc.nextInt();

        if (a > 0 && b > 0 && c > 0 && a + b + c == 180)
            System.out.println("Valid triangle");
        else
            System.out.println("Invalid triangle");
    }
}
Output:
Enter three angles: 60 60 60
Valid triangle
22. Square or Rectangle
import java.util.Scanner;

class SquareRectangle {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter length: ");
        int length = sc.nextInt();

        System.out.print("Enter breadth: ");
        int breadth = sc.nextInt();

        if (length == breadth)
            System.out.println("It is a square");
        else
            System.out.println("It is a rectangle");
    }
}
Output:
Enter length: 10
Enter breadth: 10
It is a square
23. Celsius to Fahrenheit
import java.util.Scanner;

class Temperature {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter temperature in Celsius: ");
        double celsius = sc.nextDouble();

        double fahrenheit = (celsius * 9 / 5) + 32;

        System.out.println("Temperature in Fahrenheit = " + fahrenheit);
    }
}
Output:
Enter temperature in Celsius: 25
Temperature in Fahrenheit = 77.0
24. Perfect Number
import java.util.Scanner;

class PerfectNumber {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter a number: ");
        int n = sc.nextInt();

        int sum = 0;

        if (n > 0) {
            for (int i = 1; i < n; i++) {
                if (n % i == 0)
                    sum = sum + i;
            }

            if (sum == n)
                System.out.println("Perfect number");
            else
                System.out.println("Not a perfect number");
        } else {
            System.out.println("Not a perfect number");
        }
    }
}
Output:
Enter a number: 28
Perfect number
25. Logical Operation
import java.util.Scanner;

class LogicalOperation {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter first value (0 or 1): ");
        int a = sc.nextInt();

        System.out.print("Enter second value (0 or 1): ");
        int b = sc.nextInt();

        System.out.print("Enter operator (&, |): ");
        char op = sc.next().charAt(0);

        if (op == '&') {
            if (a == 1 && b == 1)
                System.out.println("Result = 1");
            else
                System.out.println("Result = 0");
        } else if (op == '|') {
            if (a == 1 || b == 1)
                System.out.println("Result = 1");
            else
                System.out.println("Result = 0");
        } else {
            System.out.println("Invalid operator");
        }
    }
}
Output:
Enter first value (0 or 1): 1
Enter second value (0 or 1): 0
Enter operator (&, |): &
Result = 0
26. First and Last Digit Same
import java.util.Scanner;

class FirstLastDigit {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter a five-digit number: ");
        int n = sc.nextInt();

        if (n >= 10000 && n <= 99999) {
            int first = n / 10000;
            int last = n % 10;

            if (first == last)
                System.out.println("First and last digits are same");
            else
                System.out.println("First and last digits are different");
        } else {
            System.out.println("Please enter a five-digit number");
        }
    }
}
Output:
Enter a five-digit number: 12341
First and last digits are same
27. Profit or Loss
import java.util.Scanner;

class ProfitLoss {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter cost price: ");
        double cp = sc.nextDouble();

        System.out.print("Enter selling price: ");
        double sp = sc.nextDouble();

        if (sp > cp)
            System.out.println("Profit = " + (sp - cp));
        else if (cp > sp)
            System.out.println("Loss = " + (cp - sp));
        else
            System.out.println("No profit, no loss");
    }
}
Output:
Enter cost price: 500
Enter selling price: 650
Profit = 150.0
28. Count Number of Digits
import java.util.Scanner;

class CountDigits {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter a number: ");
        int n = sc.nextInt();

        n = Math.abs(n);

        if (n < 10)
            System.out.println("Number of digits = 1");
        else if (n < 100)
            System.out.println("Number of digits = 2");
        else if (n < 1000)
            System.out.println("Number of digits = 3");
        else if (n < 10000)
            System.out.println("Number of digits = 4");
        else if (n < 100000)
            System.out.println("Number of digits = 5");
        else
            System.out.println("Number has more than 5 digits");
    }
}
Output:
Enter a number: 45678
Number of digits = 5
