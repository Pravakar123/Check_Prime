import java.io.*;
import java.util.*;

public class Solution {

    public static void main(String[] args) {
        /* Enter your code here. Read input from STDIN. Print output to STDOUT. Your class should be named Solution. */
        Scanner s=new Scanner(System.in);
        int a=s.nextInt();
        int b=a/2,flag=0;
        if(a==0 || a==1){
            flag=1;
        }
        else{
            for(int i=2;i<=b;i++){
                if(a%i==0){
                    flag=1;
                    break;
                }
            }
        }
        if(flag==1){
            System.out.println("Not a Prime");
        }
        else if(flag==0){
            System.out.println("Prime");
        }
    }
}
