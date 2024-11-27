# anudipTestfinal
//question: find largest element in array
package anudipCodingTest;

//to find largest element in array
import java.util.Scanner;
public class Test {

	public static void main(String[] args) {
		Scanner scanner=new Scanner(System.in);
  //enter number of elements in array
		System.out.print("enter no. of elements in array:");
		int n=scanner.nextInt();
  //initialize an array 
		int[] array=new int[n];
		System.out.println("enter the elements of the array:");
		for(int i=0; i<n ;i++) {
			array[i]=scanner.nextInt();
		}
  //assume first is largest 
		int largest=array[0];
  //iterate through array to find largest
		for(int i=1;i<array.length;i++) {
			if(array[i]>largest) {
				largest=array[i];
			}
		}
  //print largest
		System.out.println("largest element in array is" + largest);
		scanner.close();
		

	}

}

