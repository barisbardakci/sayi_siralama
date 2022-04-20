# sayi_siralama
Java101_11 Girilen 3 sayıyı "küçükten büyüğe" sıralayan program

/* Ödev - Patika.dev
Girilen 3 sayıyı "küçükten büyüğe" sıralayan programı yazınız.*/

import java.util.Scanner;
public class Main
{
	public static void main(String[] args) {
	    int a, b, c ;
	    
	    Scanner input=new Scanner(System.in);
	    
	    System.out.print("a sayısı : ");
	    a=input.nextInt();
	    
	    System.out.print("b sayısı : ");
	    b=input.nextInt();
	    
	    System.out.print("c sayısı : ");
	    c=input.nextInt();
	    
	    if (a < b && a < c){
	        if (b < c){
	            System.out.print("a < b < c");
	        }else{
	            System.out.print("a < c < b");
	        }
	    }else if (b < a && b < c){
	        if (a < c){
	            System.out.print("b < a < c");
	        }else{
	            System.out.print("b < c < a");
	        }
	    }else{
	        if (a < b ){
	            System.out.print("c < a < b");
	        }else{
	            System.out.print("c < b < a");
	        }
	    }
	}
}
