# simpleJavaCalculator
SimpleJavaCalculator

import java.util.Scanner;
public class Main {
    
    static void print(String print){
        System.out.print(print);
    }
    
    public static void main(String[] args) {
     Scanner s = new Scanner(System.in);
        
        double num1,num2,val;
        char operator;
        int choose = 0;
        
        while(choose != 2){
            print("enter first number: ");
            num1 = s.nextDouble();
            
            print("enter operator (+,*,-,/) : ");
            operator = s.next().charAt(0);
            
            switch(operator){
                case '+':
                    print("enter second number: ");
                    num2 = s.nextDouble();
                    
                    val = (num1 + num2);
                    
                    print("\n" + num1 + " + " + num2 + " = " + val);
                    break;
                case '-':
                    print("enter second number: ");
                    num2 = s.nextDouble();
                    
                    val = (num1 - num2);
                    
                    print("\n" + num1 + " - " + num2 + " = " + val);
               
                    break;
                case '/':
                    print("enter second number: ");
                    num2 = s.nextDouble();
                    
                    val = (num1 / num2);
                    
                    print("\n" + num1 + " / " + num2 + " = " + val);
               
                    break;
                case '*':
                     print("enter second number: ");
                    num2 = s.nextDouble();
                    
                    val = (num1 * num2);
                    
                    print("\n" + num1 + " * " + num2 + " = " + val);
              
                    break;
                default: print("\n\nwrong operator");
            }
            print("\n\n\nchoose...\n1. clear\n2. exit\n");
            print("enter here: ");
            choose = s.nextInt();
            
            if(choose == 1){
                for(int i = 1; i<= 50; i++) System.out.println();
            }else if(choose == 2){
                print("\n\n\nexit successfully...");
            }else{
                print("\n\n\nnone of the choices");
            }
        }
    }
    
    
}
