# changenumber-x-to-y
import java.util.*;  
class changenumber {  
    public static void main(String[] args) {  
       int x, y1, y2 ;
       Scanner sc = new Scanner(System.in);  
       System.out.println("Enter the value of x");  
       x = sc.nextInt();
       System.out.println("Enter the value of y1 and y2");  
       y1 = sc.nextInt();  
       y2 = sc.nextInt();  
     int result=0, mult=1;
      while (x / 10 > 0)
        {
            int remainder = x % 10;
            if (remainder == y1)
                res = res + y2 * mult;
 
            else
                result= result + remainder * mult;
            mult *= 10;
            x = x / 10;
        }
        if (x == y1)
            result = result + y2 * mult;
 
        else 
            res = res + x * mult; 
         System.out.println("After swapping: "+res);  
       System.out.println( );  
    }    
}
