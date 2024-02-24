# Day5-with-java

Hey all. Today is 5th day of my coding journey. Today i practiced one problem in my own to solve the problem of 30days coding challenge with tap academy. 

In below program Scanner is used because values of n1 and n2 are not assigned inside the program, after execution, we will give the values for n1 and n2. 

By using for loop, program will print all values withing some range only. 

import java.util.Scanner;

public class CommonFactors {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // For Input part
        System.out.print("n1: ");
        int n1 = scanner.nextInt();
        
        System.out.print("n2: ");
        int n2 = scanner.nextInt();

        // Finding common factors 
        System.out.print("Common factors of " + n1 + " and " + n2 + ": ");
        for (int i = 1; i <= Math.min(n1, n2); i++) {
            if (n1 % i == 0 && n2 % i == 0) {
                System.out.print(i + " ");
            }
        }

        scanner.close();
    }
}
