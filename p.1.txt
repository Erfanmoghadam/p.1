import java.util.Scanner;
public class JavaPorgram {
        public static void main(String args[]) {
            int n, b, k, space = 1;
            Scanner row = new Scanner(System.in);
            System.out.print("Enter Number of Rows : ");
            n = row.nextInt();
            space = n - 1;
            for (k = 1; k <= n; k++) {
                for (b = 1; b <= space; b++) {
                    System.out.print(" ");
                }
                space--;
                for (b = 1; b <= (2 * k - 1); b++) {
                    System.out.print("*");
                }
                System.out.println();
            }
            space = 1;
            for (k = 1; k <= (n - 1); k++) {
                for (b = 1; b <= space; b++) {
                    System.out.print(" ");
                }
                space++;
                for (b = 1; b <= (2 * (n - k) - 1); b++) {
                    System.out.print("*");
                }
                System.out.println();
            }
        }
    }

