using System;
					
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
		int m = 258; 
		
		Console.WriteLine("Input Number:" + m);
        Console.Write("Output Number :"+ Sumsingle(m)); 
	}
}
