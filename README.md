# Repo-54
Find Whether given number is palindrome or not
import java.util.*;
public class Input {
  public static void max_min(int num)
  {
    int maxi = Integer.MIN_VALUE;
    int mini = Integer.MAX_VALUE;
    while(num!=0) {
        int rem = num%10;
        maxi = Math.max(maxi,rem);
        mini = Math.min(mini,rem);
        num = num/10;
    }
    System.out.println(maxi+""+mini);
}
public static boolean isPalindrome(int n) 
{
    int num = n;
    int rev = 0;
    while(num!=0) {
        int rem = num%10;
        rev = rev*10+rem;
        num = num/10;
    }
    if(rev==n){
        return true;
    }
    else {
        return false;
    }
}
public static void main (String arg[])
{
 Scanner sc = new Scanner (System.in);
 int num = sc.nextInt();
 if (isPalindrome(num) ) {
      System.out.println("yes");
     }
     else {
        System.out.println("No");
     }
     sc.close();
     }
 }

    

