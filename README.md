
#include <iostream>
#include <string>
using namespace std;

void PrintIntro();
string GetGuessAndPrintBack();

// The entry point to the aplication
int main()
{
	PrintIntro();

	GetGuessAndPrintBack();
	GetGuessAndPrintBack();

	cout << endl;
	return 0;
}
void PrintIntro() {
	// introduction to the game
	constexpr int WORLD_LENGHT = 5;
	cout << "Wlecome in Bulls and Cows, a fun word game.\n";
	cout << "Can you guess the " << WORLD_LENGHT;
	cout << " letter isogram I'm thinking of?\n";
	cout << endl;
	return;

}

// get a guess from a player
string GetGuessAndPrintBack() {
	cout << "Enter your guess: ";
	string Guess = "";
	getline(cin, Guess);

	// print the guess back to them
	cout << "Your guess was: " << Guess << endl;
	return Guess;
}
