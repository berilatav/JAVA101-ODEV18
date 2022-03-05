# JAVA101-ODEV18

Java döngüler ile tek bir sayı girilene kadar kullanıcıdan girişleri kabul eden ve girilen değerlerden çift ve 4'ün katları olan sayıları toplayıp ekrana basan programı yazıyoruz.


import java.util.Scanner;

public class Odev18 {
    public static void main(String[] args) {

            int c;
            int sum = 0;

            // Kullanıcıdan sayı alınır.
            Scanner input = new Scanner(System.in);

            do{
                System.out.print(" Enter a number : ");
                c = input.nextInt();

                if(c % 2 == 0 && c % 4 == 0)     //Çift ve dördün katları olan sayılar döngüyü çalıştırır ve toplamları hesaplanır.
                {
                    sum += c;
                }
            }while(c % 2 == 0);                  // Tek sayı girilene kadar döngü devam eder.


            System.out.print(" The sum of the numbers that are multiples of two and four among the entered numbers: " + sum );

        }
    }



