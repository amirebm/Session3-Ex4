# Session3-Ex4

// ب ن ک 3 ضلع زاویه یک مثلث را گرفته قايم الزاویه بودن آن را بررسی کند

package com.personal.ex4;

import java.util.Scanner;

public class ex4 {

	public static void main(String[] args) {


		Scanner sc= new Scanner(System.in);
		System.out.println("Enter three sides of rectangle");
		int num1= sc.nextInt();
		int num2=sc.nextInt();
		int num3=sc.nextInt();
		if(rightTraingle(num1,num2,num3))
			System.out.println("this is a right trangile ");
			else	
			System.out.println("this is not a right trangile ");

				}

	static boolean rightTraingle(int n1,int n2, int n3) {
		
		if(n1*n1== n2*n2+ n3*n3)
			return true;
		else if(n2*n2== n1*n1+ n3*n3)
			return true;
		else if(n3*n3== n1*n1+ n2*n2)
			return true;
		else
			return false;
		
		
	}
}
