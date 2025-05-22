package lima;
import java.util.Scanner;
class multiplication extends Thread{
	public void run() {
		try {
			System.out.println("multiplication table of 5");
			for(int i=1;i<=10;i++) {
				System.out.println(i+"X"+"5"+"="+(i*5));
			    Thread.sleep(200);
			}
		}
		catch(InterruptedException e) {
			System.out.println("Interrupted");
		}
	}
}
class prime extends Thread{
	public void run() {
		int j;
		int l;
		Scanner s=new Scanner(System.in);
		System.out.println("Enter limit:");
		 l = s.nextInt();
		 try {
			 int n=2,i=1;
			 while(i<=l) {
				 int f=1;
				 for(j=2;j<n;j++) {
					 if(n%j==0) {
						 f=0;
						 break;
					 }
				 }
					if(f==1) {
						i++;
						System.out.println("prime No:"+n);
					}
					n++;
					Thread.sleep(200);
			 }
		 }
		 catch(InterruptedException e) {
			 System.out.println("interrupted");
		 }
	}
}
public class MultiPrime {

	public static void main(String[] args) {
	multiplication m=new multiplication();
	prime p=new prime();
	m.start();
	p.start();

	}

}
