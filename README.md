# Transpose-Matrix
Transpose Matrix in java
import java.util.Scanner;

public class TransposeMatrix {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter the no. of rows: ");
        int n = sc.nextInt();
        System.out.println("Enter the no. of columns: ");
        int m = sc.nextInt();
        int arr1[][]=new int[n][m];
        System.out.println("Enter the elemets in Array: ");
        for (int i =0;i<n;i++){
            for (int j = 0;j<m;j++){
                arr1[i][j]= sc.nextInt();
            }
        }
        int trans[][] = new int[n][m];
        for (int i =0;i<m;i++){
            for (int j = 0;j<n;j++){
                trans[i][j]=arr1[j][i];
            }
        }
        for (int i =0;i<n;i++){
            for (int j = 0;j<m;j++){
                System.out.print(trans[i][j]+" ");
            }
            System.out.println();
        }
    }
}
