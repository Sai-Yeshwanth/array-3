import java.util.Scanner;


public class Jala {

	public static void main(String[] args) {
		int arr[] = new int[100];
		int flag=0;
		Scanner input = new Scanner(System.in);
		System.out.println("Enter size of array:");
		int n = input.nextInt();
		System.out.println("Enter " + n +" elements of array:");
		for(int i=0;i<n;i++)
		{
			arr[i] = input.nextInt();
		}
		System.out.println("Enter element whose index to be find:");
		int ind = input.nextInt();
		for(int i=0;i<n;i++)
		{
			if(ind==arr[i])
			{
				System.out.println("Element is found at index:"+i);
				flag=flag+1;
				break;
			}
		}
		if(flag==0){
			System.out.println("element not found");
		}
	}
}
