# pat2subtask2
Practical Assessment Task 2 - Subtask 2: C++ Program Morse Code 
#include <iostream>
#include <string>
#include <cctype>
using namespace std;

int main()
{
    // Morse code for A-Z. Index 0 = A, 1 = B, etc.
    string morseCode[26] = {
        ".-", "-...", "-.-.", "-..", ".", "..-.", "--.", "....", "..", ".---",
        "-.-", ".-..", "--", "-.", "---", ".--.", "--.-", ".-.", "...", "-",
        "..-", "...-", ".--", "-..-", "-.--", "--.."
    };

 string message, fullMorse = "";

    cout << "Enter a message: ";
    getline(cin, message);

    cout << "\nMorse code for each letter:" << endl;

    for (int i = 0; i < message.length(); i++)
    {
        char letter = toupper(message[i]);

        if (letter == ' ')
        {
            fullMorse += " "; // space between words
            continue;
        }
