//Rodrigo Espinoza

//import scanner class
//import random class
//new random seed "1701"
//create 10x10 char array(2-d)
/* create nested for loop
random value boudary set to "14"
each element is random value
-If "0", then '*'
-If "1"||"2", then "."
 */
//create do while loop for boundary conditions
/*
create another do while loop within do while
Ask user where to place satellite "@" picking row&col
-if '*'||'.' is there,"Cannot place there" and pick another location
*/
//print "Starry night"
//print the table

import java.util.Scanner;
import java.util.Random;

public class Starry_Night
{
    public static void main(String[] args)
    {
        Random randomness= new Random(1701);
        try(Scanner reply= new Scanner(System.in))
        {
        int rows=10; //size of row
        int columns=10; //size of column
        int rownum; //user picks
        int colnum;//user picks
        int value;//random values from random object
        char[][] array= new char[rows][columns];
            for(int rowcount=0;rowcount<rows;rowcount++)
            {   
                for(int colcount=0;colcount<columns;colcount++)
                {
                    value=randomness.nextInt(15);
                    if(value==0)
                    {
                         array[rowcount][colcount]='*';
                    }
                    else if(value==1||value==2)
                    {
                        array[rowcount][colcount]='.';
                    }
                    else
                    {
                        array[rowcount][colcount]=' ';
                    }
                }
            }
            System.out.println("Where do you suggest on placing sattelite.");
            do
            {
            do
            {
                System.out.println();
                System.out.println("Enter the row number");
                rownum=reply.nextInt();
                System.out.println("Enter the column number");
                colnum=reply.nextInt();
                if(rownum<0||rownum>9||colnum<0||colnum>9)
                {
                    System.out.println("Please input the correct row and column number again.");
                }
            }
                while(rownum<0||rownum>9||colnum<0||colnum>9);//1 do while
                
                if(array[rownum][colnum]=='*'||array[rownum][colnum]=='.')
                {
                    System.out.println("Cannot place there, pick another spot.");
                }
                else
                {
                    array[rownum][colnum]='@';
                }
            }
            while(array[rownum][colnum]=='*'||array[rownum][colnum]=='.'); //2 do while
        
        System.out.println("Starry night");
        for(int rowcount=0;rowcount<array.length;rowcount++) // less than number of rows array has
        {
            for(int colcount=0; colcount<array[rowcount].length;colcount++) //columns inc as row remains same
            {
                System.out.print(array[rowcount][colcount]);
            }
            System.out.println(); //print new line for every row
        }
        }
    }
}
