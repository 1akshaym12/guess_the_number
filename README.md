# guess_the_number
import java.util.Scanner;
import java.util.Random;

public class guess_the_number {
   int user;
   int step=0;
  static  Scanner sc = new Scanner(System.in);
  //created a constructor
   public guess_the_number() {
       System.out.println("guess the number=");
        user = sc.nextInt();
   }
}
class take_computer_input{
    int randomRange;
    public static void main(String[] args) {
        System.out.println("Designed by Akshay Nayak");
        take_computer_input vvv = new take_computer_input();
        int steps=0;
        while (true) {
            guess_the_number number = new guess_the_number();
            steps++;
            if (number.user < vvv.randomRange) {
                System.out.println("the number must be greater");
            } else if (number.user > vvv.randomRange) {
                System.out.println("the number must be smaller");
            } else {
                System.out.println("what a guess man!!");
                System.out.println("steps="+steps);
            }

        }
    }
    public take_computer_input(){
        Random random=new Random();
        randomRange=random.nextInt(100);
    }
}

