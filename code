import java.util.Scanner;

public class BMICalculator {
    public static void main(String[] args) {
        try (Scanner scanner = new Scanner(System.in)) {
            System.out.println("Enter your weight in kilograms:");
            double weight = scanner.nextDouble();

            System.out.println("Enter your height in centimeters:");
            double heightCm = scanner.nextDouble();

            // Convert height from centimeters to meters
            double height = heightCm / 100;

            if (height <= 0) {
                System.out.println("Error: Height must be greater than zero.");
                return;
            }

            double bmi = weight / (height * height);

            System.out.printf("Your BMI is: %.2f\n", bmi);

            if (bmi < 18.5) {
                System.out.println("Category: Underweight");
            } else if (bmi >= 18.5 && bmi < 24.9) {
                System.out.println("Category: Normal weight");
            } else if (bmi >= 25 && bmi < 29.9) {
                System.out.println("Category: Overweight");
            } else {
                System.out.println("Category: Obesity");
            }
        }
    }
}
