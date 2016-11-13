# tamirinta6
package tamirinta;

import static java.util.EnumSet.range;
import java.util.Scanner;
import static java.util.stream.IntStream.range;
import static java.util.stream.LongStream.range;

public class tamirinta6 {
    private static int range;

    public static void main(String[] args) { //begin main method

        Scanner console = new Scanner(System.in);

        System.out.println("This program prints the sequence of numbers between"
                + " the two numbers that you give");

        //obtain values
        System.out.println("Enter two numbers (x,y)");
        System.out.print("Number x: ");
        int x = console.nextInt();
        System.out.print("Number y: ");
        int y = console.nextInt();

        int sequence;
        sequence = printRange(x, y);

        System.out.println("The sequence of your number is " + sequence);

    } //end main method

    public static int printRange(int x, int y) { //begin printRange method   
        //this method accepts two parameters and return an integer
         
    if (x > y) { //begin if statement
            //x is larger than y
            for (int i = x; i <= y; i++) {//begin for loop i
                System.out.print("[" + i + "]");
                range = range + i;
            }//end for loop i

        } //end if method
        else if (x < y) { //begin else if method
            //x is smaller than y
            for (int j = x; j >= y; j--) {//begin for loop j
                System.out.print("[" + j + "]");
                range = range + j;
            }//end for loop j
        } //end else if method
        else if (x == y) { //begin else if method
            //x is equal to y
            System.out.print(x);
            range = range + x;
        } //end else if method
        return range;
    } //end printRange method

}
