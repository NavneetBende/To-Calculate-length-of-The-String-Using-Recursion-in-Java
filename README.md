# To-Calculate-length-of-The-String-Using-Recursion-in-Java

Calculate length of The String Using Recursion
Today on this page we will learn to create a Java Program to Calculate the Length of the String using Recursion as well as Loop.

Example :

Input : PrepInsta
Output : length of PrepInsta is 9
Explanation : Length of PrepInsta is 9 as it consist of 9 characters.
To Calculate length of The String Using Recursion in Java
Note:
The given program counts any spaces present in the string. For example, length of "Hi" is 2 but length of " Hi" or "Hi " is 3.
Method 1 : Length of the String using Recursion
Algorithm
Start by passing the string to a function
If string is empty then return 0
Else return sum of 1 and recursive call of str[1:]
Print the returned value by function
Calculate length of The String Using Recursion
Java Code
Run
public class Main
{
     //Function to calculate length
    private static int recLength(String str)
    {
        // if we reach at the end of the string
        if (str.equals(""))
            return 0;
        else
            return recLength(str.substring(1)) + 1;
    }

    //Driver program to test the function 
    public static void main(String[] args)
    {
        String str ="Prepinsta";
        System.out.println("length of the string "+recLength(str));
    }
}
Output
length of PrepInsta is 9 
Method 2 : Using Loop
Algorithm
Strat by passing string to the function
Initialize a variable i = 0
Run a while loop until string is not empty
For each iteration increment the value of i by 1 and set the value of str to str[1:]
Return value of i & Print
Java Code
Run
public
class Main {
    public
    static void main(String args[]) {
        int i = 0;
        String str = "Prepinsta";
        char ch[] = str.toCharArray();
        for (char c : ch) {
            i++;
        }
        System.out.println("Length of the string = "+ i);
    }
}
Output
Length of the string = 9
