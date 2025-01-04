# zomato-in-java
import java.util.Scanner;

public class zomato {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.println("Welcome to Zomato!");
        System.out.println("Select a Menu:");
        System.out.println("1. north Indian ");
        System.out.println("2. south indian ");
        System.out.println("3. chat");
        System.out.println("4. sweets");
        System.out.println("5. Exit");
        System.out.print("Enter your choice (1-5): ");
        int menuChoice = scanner.nextInt();

        switch (menuChoice) {
            case 1:
                System.out.println("You selected north Indian.");
                break;
            case 2:
                System.out.println("You selected south indian.");
                break;
            case 3:
                System.out.println("You selected chat.");
                break;
            case 4:
                System.out.println("You selected sewwts.");
                break;
            case 5:
                System.out.println("Thank you for using Zomato. Goodbye!");
                scanner.close();
                return;
            default:
                System.out.println("Invalid choice. Exiting.");
                scanner.close();
                return;
        }
        System.out.println("\nSelect a Hotel:");
        System.out.println("1. kongu mess");
        System.out.println("2. abc hotel ");
        System.out.println("3. kfc");
        System.out.print("Enter your choice (1-3): ");
        int hotelChoice = scanner.nextInt();

        switch (hotelChoice) {
            case 1:
                System.out.println("You selected kongu mess.");
                break;
            case 2:
                System.out.println("You selected abc hotel.");
                break;
            case 3:
                System.out.println("You selected kfc.");
                break;
            default:
                System.out.println("Invalid choice. Exiting.");
                scanner.close();
                return;
        }
        System.out.println("\nWould you like to review the hotel? (yes/no): ");
        scanner.nextLine();
        String review = scanner.nextLine();

        if (review.equalsIgnoreCase("yes")) {
            System.out.print("Enter your review: ");
            String userReview = scanner.nextLine();
            System.out.println("Thank you for your review: " + userReview);
        } else {
            System.out.println("Skipping the review.");
        }
        System.out.println("\nPlace your order:");
        System.out.println("1. Starter");
        System.out.println("2. Main Course");
        System.out.println("3. Dessert");
        System.out.print("Enter your choice (1-3): ");
        int orderChoice = scanner.nextInt();

        switch (orderChoice) {
            case 1:
                System.out.println("You ordered a Starter. Enjoy your meal!");
                break;
            case 2:
                System.out.println("You ordered a Main Course. Enjoy your meal!");
                break;
            case 3:
                System.out.println("You ordered a Dessert. Enjoy your meal!");
                break;
            default:
                System.out.println("Invalid choice. Exiting.");
        }

        System.out.println("\nThank you for using Zomato. Have a great day!");
        scanner.close();
    }
}
