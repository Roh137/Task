public static void main(String[] args) {
Scanner scanner = new Scanner(System.in);
Random random = new Random();

int roundswon = 0;
boolean playAgain = true;

while (playAgain) {
int numberToGuess = random.nextInt(bound:100) + 1; // Random number between 1 and 100
int attempts = 0;
boolean guessedCorrectly = false;

System.out.println(x: "I have generated a random number between 1 and 100. Can you guess it ?")
 while (attempts < 10 && !guessedCorrectly) {
System.out.print("Enter your guess (attempt " + (attempts + 1) + " of 10): ");
 int userGuess = scanner.nextInt();
attempts++;

if (userGuess == numberToGuess) {
guessedCorrectly = true;
roundsWon++;
System.out.println("Congratulations! You guessed the number in " + attempts +" attempts".)
} else if (userGuess < numberToGuess) {
System.out.println(x: "Too low!");
} else {
System.out.println(x: "Too high!");
}
}

if (!guessedCorrectly) {
System.out.println("Sorry, you've used all 10 attempts. The number was:"+number
}

System.out.print(s: "Do you want to play another round? (yes/no): ");
 playAgain = scanner.next().equalsIgnoreCase(anotherString: "yes");
tem.out.println("You won "+ roundswon +" rounds. Thank you for playing!");

nner.close();
