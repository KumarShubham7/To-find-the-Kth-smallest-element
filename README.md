# To-find-the-Kth-smallest-element
import java.util.*;
public class Main
{
	public static void main(String[] args) {
	    
	    Scanner sc = new Scanner(System.in);
	    System.out.println("Enter the Kth smallest element that you want to find:- ");
	    int x = sc.nextInt();
	 
	    int B[] = {7,10,4,3,20,15};
	    int n = 6;
	    
	    if(x>6)
	    {
	        System.out.println("Error :- Input size is greater than the size of array");
	    }
	    
		int count = 0;
		while(count<=3)
		{
		    for(int i=0;i<n-1;i++)
		    {
		        if(B[i]>B[i+1])
		        {
		            int temp = B[i];
		            B[i] = B[i+1];
		            B[i+1] = temp;
		        }
		        
		    }
		      count++;
		}
		
		/*for(int i=0;i<n;i++)
		{
		    System.out.println(B[i]);
		}*/
		
		switch(x){
		    
		    case 1: System.out.println("Smallest element is:- "+B[x-1]);
		    break;
		    case 2: System.out.println("Second Smallest element is:- "+B[x-1]);
		    break;
		    case 3: System.out.println("Third smallest element is:- "+B[x-1]);
		    break;
		    case 4: System.out.println("Fourth smallest element is:- "+B[x-1]);
		    break;
		    case 5: System.out.println("Fifth smallest element is:- "+B[x-1]);
		    break;
		    case 6: System.out.println("Sixth smallest element or the largest element is:- "+B[x-1]);
		    break;
		}
		
	    
	    
	    
	    
	    
	    
	}
}
