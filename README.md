# JavaApplication52
java program that let the user choose his/her username and password. The program verifies whether the chosen username and password are valid. If either one of them is invalid, it notifies the user and explain the cause of invalidity. The rules for choosing valid usernames and passwords are: a. A username must be of length 6-15 characters. b. A username must start with an uppercase English alphabet A to Z. c. A password must not be shorter than 8 characters but must not exceed 256. d. There cannot be any types of parentheses or whitespaces in a valid username or password. e. A password cannot contain or be the same as its associated username.

package javaapplication52;
import java.util.Scanner;
/**
 *
 * @author WHITEKABAR
 */
public class JavaApplication52 {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        String username, password, k, l;
        k = "{";
        l = " ";
        Scanner input = new Scanner (System.in);
        System.out.println("Enter your username");
        username = input.next();
        if (username.length()>=6) {
        }else{
            System.out.println("input less than 6");
        }
        if (username.length()<=15) {
        }else{
            System.out.println("input greater than 15");
        }
        if (Character.isUpperCase(username.charAt(0))) {
        }else{
            System.out.println("first letter is lower case");
        }
        System.out.println("Please enter password");
        password = input.next();
        if (password.length()>=8) {
        }else{
            System.out.println("Password is less than 8");
        }
        if (password.length()<=256) {
        }else{
            System.out.println("Password more than 256");
        }
        if (password.contains(k)) {
            System.out.println("Password contains perentheses");
        }else{
        }
        if (password.contains(" ")) {
            System.out.println("Password contains Whitespace");
        }else{}
        if (username.equals(password)) {
            System.out.println("Username is the same with password");
        }else{
        }
           
        }
