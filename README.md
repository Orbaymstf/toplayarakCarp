# toplayarakCarp
package recursive;

import java.util.Scanner;

public class toplayarakcarpma {

    public static int topcarp(int sayı, int carpılacak) {
        if (sayı == 0 || carpılacak == 0) {
            return 0;
        } else {
            return sayı + topcarp(sayı, carpılacak - 1);
        }
    }

    public static void main(String[] args) {
        Scanner klv = new Scanner(System.in);
        System.out.println("sayıyı giriniz");
        int sayı = klv.nextInt();
        System.out.println("carpılacak sayıyı giriniz");
        int carp = klv.nextInt();
        System.out.println(topcarp(sayı, carp));
    }
}
