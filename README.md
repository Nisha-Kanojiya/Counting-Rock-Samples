# Counting-Rock-Samples
My first new repository, Coded by ME in JAVA


***********COUNTING ROCK SAMPLE*****************



import java.util.ArrayList; 

import java.util.Scanner;

public class Main
{

	public static void main(String[] args) {
  
        int count=0;
  
        Scanner s =new Scanner(System.in);
    
	ArrayList<Integer> l=new ArrayList<Integer>();
    
        int nos=s.nextInt();
        
        System.out.print(" ");
        
        int range=s.nextInt();
        
        for(int i=0;i<nos;i++) 
        {
        
            int sa=s.nextInt();
            
            l.add(sa);
            
            System.out.print(" ");
            
        }
        
        int min[]=new int[1000];
        
        int max[]=new int[1000];
        
        for(int i=0 ; i<range ; i++)
        {
            min[i]=s.nextInt();
            System.out.print(" ");
            max[i]=s.nextInt();
            System.out.println();
        }
        for(int i=0;i<range;i++)
        {
            for(int num:l)
            {
                if(num>=min[i] && num<=max[i])
                {
                   count++; 
                }
            }
            System.out.print(count+" " );
            count=0;
        }
        
        
	}
}
