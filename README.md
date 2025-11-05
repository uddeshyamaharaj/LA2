//LA2
import java.util.ArrayList;
import java.util.Scanner;

public class NameCollector {
    public static void main(String[] args) {
        ArrayList<String> names = new ArrayList<>();
        Scanner scanner = new Scanner(System.in);
        String input;

        System.out.println("Enter names (type 'exit' to finish):");

        while (true) {
            System.out.print("Enter name: ");
            input = scanner.nextLine();

            if (input.equalsIgnoreCase("exit")) {
                break;
            }
            names.add(input);
        }

        System.out.println("Names entered:");
        for (String name : names) {
            System.out.println(name);
        }
    }
}
