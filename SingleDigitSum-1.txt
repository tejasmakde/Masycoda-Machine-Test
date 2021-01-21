uusing System;
					
public class Program
{
	static int Sumsingle (int t) 
    { 
        int no = 0; 
  
        while (t > 0 || no > 9)  
        { 
            if (t == 0) 
            { 
                t = no; 
                no = 0; 
            } 
            no += t % 10; 
            t /= 10; 
        } 
        return no; 
    } 
	
	public static void Main()
	{
		Console.WriteLine("Single Digit Sum Program");
		int m = 548399; 
		
		Console.WriteLine("Input Numbers:" + m);
        Console.Write("A single digit sum of that Numbers :"+ Sumsingle(m)); 
	}
}