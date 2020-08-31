
package demo;

import java.util.Scanner;

public class Guess {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int count=0;
        while (true){
            if (n==1){
                break;
            }else if (n % 2 == 0) {
                n=n/2;
            }else {
                n=(n*3+1)/2;
            }
            count++;
        }
        System.out.println(count);
    }
}
