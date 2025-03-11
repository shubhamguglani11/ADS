import java.util.Scanner;
import java.util.*;
public class homework {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        System.out.println("enter the size of array");
        int[] a=new int[n];
        System.out.println("enter the elements of array");
        for(int i=0;i<n;i++)
        {
            a[i]=sc.nextInt();
        }
        System.out.println(issorted(a));

    }
    public static boolean issorted(int[]a)
    {
        for(int i=1;i<a.length;i++)
        {
            if(a[i-1]>a[i])
            {
                return false;
            }

        }
        return true;
    }
}
