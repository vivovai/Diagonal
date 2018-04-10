# Diagonal
import java.util.Scanner;

public class Zadacha5 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Scanner in = new Scanner(System.in);
		System.out.println("Write N");
		int n=in.nextInt();
		int [][] numbers= new int[n][n];
		int diag1=0;
		int diag2=0;
		
		for(int i=0;i<numbers.length;i++)
		{
			for(int j=0;j<numbers[i].length;j++)
			{
				numbers[i][j] = in.nextInt();
			}
		}
		for(int i=0;i<numbers.length;i++)
		{
		
			diag1 += numbers[i][i];
		diag2 += numbers[i][n-i-1];
		}
		if(diag1>diag2)
		{
			System.out.println("Po-golqm e diag1=" + diag1);
		}
		else if(diag2>diag1)
		{
			System.out.println("Po-golqm e diag2=" + diag2);
		}
		else {
			System.out.println("diag1=diag2=" + diag1);
		}
			System.out.println("diag1=" + diag1);
			System.out.println("diag2=" + diag2);
		}

	
}
