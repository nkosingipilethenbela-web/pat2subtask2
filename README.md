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
