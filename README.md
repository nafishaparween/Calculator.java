# Calculator.java
**Problem 1:- small calculator which performs operation as addition , subtraction, multiplication and division.
/*
Programming language -Java
*/
package com.company;
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {

        Scanner scanner =new Scanner(System.in);
        System.out.println("enter type of operation");
        String type= scanner.nextLine();
        System.out.println("enter values of a and b");
        double a= scanner.nextInt();
        double b=scanner.nextInt();

        switch(type)
        {
            case "addition":
                System.out.println("Addition of "+a+ " and "+b+ " is "+(a+b));
                break;
            case "subtraction":
                System.out.println("Subtraction of "+a+ " and "+b+ " is "+(a-b));
                break;
            case "multiplication":
                System.out.println("Multiplication of "+a+ " and "+b+ " is "+(a*b));
                break;
            case "division":
                if(b==0)
                {
                    System.out.println("result is infinity as value of b is 0");
                    break;
                }
                else
                {
                    System.out.println("division of "+a+ " and "+b+ " is "+(a/b));
                    break;
                }
            default:
                System.out.println("Invalid choice ");
        }
        scanner.close();
    }
}
