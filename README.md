# dsa-java

import java.util.*;

public class palindrome {
    public static void main(String[]args){
        Scanner sc = new Scanner(System.in);
        int num = sc.nextInt();
        int original = num;
        if(num<0){
            System.out.print("No");
            return;
        } 
        int rev = 0;
        while(num>0){
            rev = rev*10+num%10;
            num = num/10;
        }
        if(rev==original){
            System.out.print("Yes");

        }
        else{
            System.out.print("No");
        }
        return;
    }
    
}
