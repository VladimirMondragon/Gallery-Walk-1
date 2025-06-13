import java.util.Random;

public class RandomNameGenerator {
    public static void main(String[] args) {
        String alphabet = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
        String name = "";

        Random random = new Random();

        for (int i = 0; i < 4; i++) {
            int index = random.nextInt(alphabet.length());
            name += alphabet.charAt(index);
        }

        System.out.println("Random 4-letter name: " + name);
    } 
}
