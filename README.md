#include <iostream>
#include <map>
#include <iostream>
#include <map>
#include <string>
#include <cctype>

using namespace std;

// Define dot and dash characters
const char DOT = '.';   // ASCII 46
const char DASH = '-';  // ASCII 45

// Morse code mapping for A-Z
map<char, string> morseCode = {
    {'A', ".--"}, {'B', "-..."}, {'C', "-.-."}, {'D', "-.."}, {'E', "."},
    {'F', "..-."}, {'G', "--."}, {'H', "...."}, {'I', ".."}, {'J', ".---"},
    {'K', "-.-"}, {'L', ".-.."}, {'M', "--"}, {'N', "-."}, {'O', "---"},
    {'P', ".--."}, {'Q', "--.-"}, {'R', ".-."}, {'S', "..."}, {'T', "-"},
    {'U', "..-"}, {'V', "...-"}, {'W', ".--"}, {'X', "-..-"}, {'Y', "-.--"},
    {'Z', "--.."}
};

int main() {
    string input;
    cout << "Enter a short message: ";
    getline(cin, input);

    string fullMorse = "";

    for (char ch : input) {
        if (isalpha(ch)) {
            char upperChar = toupper(ch);
            int main() {
    string input;
    cout << "Enter a short message: ";
    getline(cin, input);

    for (char ch : input) {
        if (isalpha(ch)) {
            char upperChar = toupper(ch);
            cout << upperChar << endl;
        }
    }

    return 0;
}

            // Output individual letter and its Morse code
            cout << upperChar << ": ";
            for (char symbol : morse) {
                if (symbol == '.') cout << DOT;
                else if (symbol == '-') cout << DASH;
            }
            cout << endl;

            // Append to full Morse code message
            for (char symbol : morse) {
                fullMorse += (symbol == '.' ? DOT : DASH);
            }
            fullMorse += "   "; // Three spaces between letters
        }
        // Ignore non-alphabetic characters
    }

    cout << "\nFull Morse code with spaces:\n" << fullMorse << endl;
    return 0;
}
