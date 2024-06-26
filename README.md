import java.util.*;
import java.util.Scanner;

class HelloWorld {
      /* public static int  myName( int a,int b)
    { int sum = a + b ;
         return sum;}
     public static int  myName1( int a,int b)
    { int sub = a - b ;
         return sub;}
     public static int  myName2( int a,int b)
    { int mul = a * b ;
         return mul;}
     public static float  myName3( int a,int b)
    { float div = a / b ;
         return div;}
    
     public static float  myName4( int a,int b)
    { float mod = a % b ;
         return mod; }*/
         
       //  String name = "bhuva" ;
    // this is the function of the each statements
    
    
    
    public static void printArray(int arr[])
    {
        for(int i=0;i<arr.length;i++)
        {
            System.out.print(arr[i]+" ");
            
        }
        System.out.println();
    }
    public static void main(String[] args) {
    /*    System.out.println("Start");
        
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        int b = sc.nextInt();
        
        System.out.println("Choise : \n For + ==> 1 \n For - ==> 2 \n for * ==> 3 \n for / ==> 4 \n For % ==> 5");
        int c = sc.nextInt();
        if(c==1)
        { int sum =  myName(a,b);
            System.out.println(sum);}
        else if(c==2)
        {  int sub =  myName1(a,b);
             System.out.println(sub);}
        else if(c==3)
        { int mul =  myName2(a,b);
            System.out.println(mul);}
        else if(c==4)
        { float div =  myName3(a,b);
             System.out.println(div);}
        else  if(c==5)
        { float mod =  myName4(a,b);
            System.out.println(mod);}
        else 
        { System.out.println(" yessss ");}
        */
        
        Scanner sc = new Scanner(System.in);
        int arr[] = new int[4];
        System.out.println("Enter the array: ");

        for(int i=0;i<arr.length;i++)
        {
            arr[i]=sc.nextInt();
        }
        for(int i=0;i<arr.length-1;i++)
        {
            for(int j=0;j<arr.length-i-1;j++)
            {
                if(arr[j]>arr[j+1])
                {
                    int t = arr[j];
                    arr[j]=arr[j+1];
                    arr[j+1]=t;
                }
            }
        }
        printArray(arr);
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
    }
}
