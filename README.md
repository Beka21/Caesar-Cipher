# Caesar-Cipher
how to return original input of count
import java.util.Scanner;

public class CaesarCipher1253 {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        int tests = scan.nextInt();
        input.nextLine();

        while (tests > 0){
            String str = input.nextLine();
            int counts = input.nextInt();
            int changedCount = 1;
            char[] arr = str.toCharArray();

            for (int i = 0; i < str.length(); i++){
                if (arr[i] >= 'A' && arr[i] <= 'Z') {

                    if (arr[i] == 'Z') {
                        arr[i] = 'A';
                        counts++;
                    }
                    if (arr[i] == 'A') {
                        arr[i] = 'Z';
                        counts--;
                    }

                    arr[i] -= counts;
                    //if (counts-- || counts++){
                        
                    //}
                }
            }
            System.out.println(arr);
        }
    }
}
