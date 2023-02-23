# UsluSayiMetod
www.paatika.dev
---------------


import java.util.Scanner;

public class UsluSayiMetod {
	
	static int Üst(int a,int b) {
		if(b==0) {
			return 1;
		}
		else {
			return a * Üst(a,b-1);
		}
		
	}

	public static void main(String[] args) {
		
		Scanner scanner = new Scanner(System.in);
		
		System.out.println("Tabanı giriniz: ");
		int a= scanner.nextInt();
		System.out.println("Üstü giriniz: ");
		int b = scanner.nextInt();
		
		int result = Üst(a,b);
		System.out.println(a + " Üzeri " +b + " = " + result);
	}

}
