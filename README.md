# 4.36-Sides-of-a-Right-Triangle-Write-an-application-that-reads-three-nonzero-integers-and-de--term
4.36 (Sides of a Right Triangle) Write an application that reads three nonzero integers and de- termines and prints whether they could represent the sides of a right triangle.


import java.util.Scanner;

public class Main {



    public static void main(String[] args) {
        Scanner console = new Scanner(System.in);
        System.out.println("Enter Three Sides of a Triangle: ");
        int Side1=console.nextInt();
        int Side2=console.nextInt();
        int Side3 = console.nextInt();

        int S1Square =Side1*Side1;
        int S2Square =Side2*Side2;
        int S3Square = Side3*Side3;

        if((S1Square+S2Square)==S3Square){
            System.out.println("Right Angle Triangle is Valid: ");
        }else if((S2Square+S3Square)==S1Square){
            System.out.println("Right Angle Triangle is Valid: ");
        } else if ((S1Square+S3Square)==S2Square) {
            System.out.println("Right Angle Triangle is Valid: ");
        } else
            System.out.println("Not a valid Right Angle Triangle: ");


    }
}
