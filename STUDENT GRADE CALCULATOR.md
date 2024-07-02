import java.util.Scanner;

public class StudentGrades {

public static void main(String[] args) {
Scanner scanner = new Scanner(System.in);

// Initialize variables for each subject
int english, hindi, maths, physics, chemistry;

// Input marks for each subject
System.out.print(s: "Enter marks for English (out of 100): "); english = scanner.nextInt();

System.out.print(s: "Enter marks for Hindi (out of 100): ");
hindi = scanner.nextInt();

System.out.print(s: "Enter marks for Maths (out of 100): ");
maths = scanner.nextInt();

System.out.print(s: "Enter marks for Physics (out of 100): "); physics = scanner.nextInt();

System.out.print(s: "Enter marks for Chemistry (out of 100): "); chemistry = scanner.nextInt();

// Calculate total marks
int totalMarks = english + hindi + maths + physics + chemistry;

// Calculate average percentage
double  averagePercentage = totalMarks / 5.0;

// Determine grade based on average percentage char grade;
if (averagePercentage >= 90) {
grade = 'A';
} else if (averagePercentage >= 80) {
grade = 'B';
} else if (averagePercentage >= 70) {
grade = 'C';
} else if (averagePercentage >= 60) {
grade = 'D';
} else {
grade = 'F';
}

// Display the results
System.out.println("\nTotal Marks: " + totalMarks);
System.out.println("Average Percentage: " + averagePercentage + "%"); 
System.out.println("Grade: + grade);
// close the scanner
 scanner.close();
}
}
