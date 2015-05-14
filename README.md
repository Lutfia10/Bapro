# Bapro
package coin;

import java.util.Scanner;

public class Coin {

    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
     double  money;
     System.out.println("Masukkan Jumlah Uang ");
     money = input.nextDouble();

     while (money > 0 && money<= 2000){
       if (money >= 500) {
          System.out.println(Math.floor(money/500)+" 500an");
          money -= Math.floor(money/500)*(double)500;
       }
       else if (money>=200) {
         System.out.println(Math.floor(money/200)+" 200an");
         money-= Math.floor(money/200)*(double)200;
       }
       else if (money>=100) {
         System.out.println(Math.floor(money/100)+" 100an");
         money-= Math.floor(money/100)*(double)100;
       }
     }
  }
    }
