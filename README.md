# Java
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
