# TICTAC
import java.util.Random;
import java.util.Scanner;

public class Magic {
	 public static void main(String[] args) {
	
	    int[] magicSquare = new int[]{2,7,6,9,5,1,4,3,8};
	    int[] input = new int[] {1,2,3,4,5,6,7,8,9};
	    
	    	int a = 5;
	    	Scanner sc= new Scanner(System.in); 
	    	System.out.print("Enter user number- ");
	    	int b = sc.nextInt();
	    		 int c = 4;
	    		Scanner sc1= new Scanner(System.in); 
		    	System.out.print("Enter user number- ");
		    	int d = sc1.nextInt();
	    		int e = 15 - (a+c);
	    	if ( e == d) {
	    			System.out.println("user win");
	    			
	    				    		}
	    		else {
	    			  e = 15-(a+d);
	    		}
	    	    	Scanner sc2= new Scanner(System.in); 
	    	System.out.print("Enter the name of the user ");
	    	int f = sc2.nextInt();
    			int g = a + e;
	    		if (f != 9) {
	    			System.out.println("machine wins");
	    		}
	    		
	        Magic ticTacToe = new Magic();
	   
	  
	 }

	 
	 
	    void checkWinner() {
	        if (hasWon('a')) 

	        	System.out.println("user  win");
	        else if

	        (hasWon('r'))
 
	        	System.out.println("computer  win");
	        else 
	        	System.out.println("Anyone cannot win win");
	    }

	    static boolean hasWon(int i) {
	        int[] magicSquare = null;
			for (int a = 0; a < 9; a++)
	            for (int b = 0; b < 9; b++)
	                for (int c = 0; c < 9; c++)
	                    if (a != b && a != c && b != c)
	                       
	                            if (magicSquare[a] + magicSquare[b] + magicSquare[c] == 15)
	                                return true;
	        return false;
	    }
}
