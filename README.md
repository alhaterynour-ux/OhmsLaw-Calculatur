# OhmsLaw-Calculatur
import java.util.Scanner;

public class OhmsLawCalculator {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.print("Enter voltage (V): ");
        double voltage = input.nextDouble();

        System.out.print("Enter resistance (R): ");
        double resistance = input.nextDouble();

        if (resistance == 0) {
            System.out.println("Resistance cannot be zero.");
        } else {
            double current = voltage / resistance;
            System.out.println("Current (I) = " + current + " A");
        }

        input.close();
    }
}
