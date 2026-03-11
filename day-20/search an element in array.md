import java.util.Scanner;
public class SearchArray {
 static void search(int arr[], int key) {
        boolean found = false;
        for(int i = 0; i < arr.length; i++) {
            if(arr[i] == key) {
                found = true;
                break;
            }
        }
  if(found)
            System.out.println("Element Found");
        else
            System.out.println("Element Not Found");
    }
  public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int arr[] = new int[5];
        System.out.println("Enter 5 numbers:");
        for(int i = 0; i < 5; i++) {
            arr[i] = sc.nextInt();
        }
        System.out.print("Enter number to search: ");
        int key = sc.nextInt();
        search(arr, key);
    }
}
