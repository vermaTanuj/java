# java
 one
 import java.util.Scanner;
public class q___6 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter First No:-");
        int a = sc.nextInt();
        System.out.print("Enter second No:-");
        int b =sc.nextInt();
        prime_no(a,b);
    }

    private static void prime_no(int a, int b) {

        for(int i=a;i<b;i++){
            
            System.out.println(i +" :- "+ isPrime(i));
        }
    }
    private static String isPrime(int l) {
        if (l == 1) {
            return "prime";
        }
        for (int i = 2; i < l; i++) {
            if (l % i == 0) {
                return "Composit no";
            }
        }
        return "Prime No";
    }
}

