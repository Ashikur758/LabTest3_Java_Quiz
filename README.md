import java.util.Scanner;

public class GKQuiz {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);
        int score = 0;

        System.out.println("====================================");
        System.out.println("   High School General Knowledge Quiz ");
        System.out.println("====================================");

        // Question 1
        System.out.println("\n1. What is the capital of Bangladesh?");
        System.out.println("A. Chittagong");
        System.out.println("B. Khulna");
        System.out.println("C. Dhaka");
        System.out.println("D. Rajshahi");
        System.out.print("Your answer: ");
        char ans1 = sc.next().toUpperCase().charAt(0);
        if (ans1 == 'C') {
            score++;
        }

        // Question 2
        System.out.println("\n2. Who is known as the Father of Computer?");
        System.out.println("A. Alan Turing");
        System.out.println("B. Charles Babbage");
        System.out.println("C. Bill Gates");
        System.out.println("D. Steve Jobs");
        System.out.print("Your answer: ");
        char ans2 = sc.next().toUpperCase().charAt(0);
        if (ans2 == 'B') {
            score++;
        }

        // Question 3
        System.out.println("\n3. Which planet is known as the Red Planet?");
        System.out.println("A. Earth");
        System.out.println("B. Venus");
        System.out.println("C. Mars");
        System.out.println("D. Jupiter");
        System.out.print("Your answer: ");
        char ans3 = sc.next().toUpperCase().charAt(0);
        if (ans3 == 'C') {
            score++;
        }

        // Question 4
        System.out.println("\n4. What is the chemical symbol of Water?");
        System.out.println("A. CO2");
        System.out.println("B. O2");
        System.out.println("C. H2");
        System.out.println("D. H2O");
        System.out.print("Your answer: ");
        char ans4 = sc.next().toUpperCase().charAt(0);
        if (ans4 == 'D') {
            score++;
        }

        // Question 5
        System.out.println("\n5. How many continents are there in the world?");
        System.out.println("A. 5");
        System.out.println("B. 6");
        System.out.println("C. 7");
        System.out.println("D. 8");
        System.out.print("Your answer: ");
        char ans5 = sc.next().toUpperCase().charAt(0);
        if (ans5 == 'C') {
            score++;
        }

        // Result
        System.out.println("\n====================================");
        System.out.println("              RESULT                ");
        System.out.println("====================================");
        System.out.println("Total Questions: 5");
        System.out.println("Correct Answers: " + score);
        System.out.println("Score: " + score + "/5");

        if (score >= 4) {
            System.out.println("Grade: Excellent");
        } else if (score >= 2) {
            System.out.println("Grade: Good");
        } else {
            System.out.println("Grade: Try Again");
        }

        sc.close();
    }
}
