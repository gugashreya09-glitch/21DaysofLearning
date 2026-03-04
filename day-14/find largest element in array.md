import java.util.Scanner;
public class largestInArray{
public static void main(String args[])
{
Scanner sc=new scanner(system.in);
system.out.print("Enter number of elements:");
int n = sc.nextInt();
int[]arr = new int[n];
system.out.println("Enter elements:");
for(int i=0;i<n;i++)
{
arr[i] = sc.nextInt();
}
int largest = arr[0];
for(int i=1;i<n;i++)
{
if(arr[i]>largest)
{
largest = arr[i];
}
}
system.out.println("largest element="+largest);
}
}
