# dizidekielemanlariKucuktenBuyugeSiralama
import javax.xml.stream.events.StartDocument;
import java.sql.SQLOutput;
import java.util.Arrays;
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {

        Scanner input = new Scanner(System.in);
        int arrLength;

        System.out.println("Dizi boyutunu giriniz : ");
        arrLength = input.nextInt();

        int[] arr = new int[arrLength];
        System.out.println("Dizi elemanlarini giriniz : ");

        int[] arrSort = new int[arrLength];

        for (int i = 0; i < arrLength; i++) {

            arrSort[i] = Integer.parseInt(input.next());
            System.out.println((i + 1) + ". Eleman : " + arrSort[i]);
        }
        Arrays.sort(arrSort);
        System.out.print("Siralama : ");
        for (int i = 0; i < arrSort.length; i++) {

            System.out.print(arrSort[i] + " ");
        }

    }
}


