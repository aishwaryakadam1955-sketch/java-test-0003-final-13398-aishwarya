# java-test-0003-final-13398-aishwarya
Final Project Assignment - This repository contains the complete final project code and documentation.
public class DiamondPattern {
    public static void main(String[] args) {
        int n = 5; // Number of rows for the top half

       
        for (int i = 1; i <= n; i++) {
            // Print leading spaces
            for (int j = i; j < n; j++) {
                System.out.print(" ");
            }
           
            for (int k = 1; k <= (2 * i - 1); k++) {
                if (k == 1 || k == (2 * i - 1)) {
                    System.out.print("*");
                } else {
                    System.out.print(" ");
                }
            }
            System.out.println();
        }

       
        for (int i = n - 1; i >= 1; i--) {
           
            for (int j = n; j > i; j--) {
                System.out.print(" ");
            }
           
            for (int k = 1; k <= (2 * i - 1); k++) {
                if (k == 1 || k == (2 * i - 1)) {
                    System.out.print("*");
                } else {
                    System.out.print(" ");
                }
            }
            System.out.println();
        }
    }
}
