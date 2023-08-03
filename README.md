// Cpp-_program
#include <iostream>
#include <string>

// Function to reverse the given string
std::string reverseString(const std::string& str) {
    std::string reversedStr = str;
    int left = 0;
    int right = reversedStr.length() - 1;

    while (left < right) {
        std::swap(reversedStr[left], reversedStr[right]);
        left++;
        right--;
    }

    return reversedStr;
}

int main() {
    std::string inputString;
    std::cout << "Enter a string: ";
    std::getline(std::cin, inputString);

    std::string reversedString = reverseString(inputString);
    std::cout << "Reversed string: " << reversedString << std::endl;

    return 0;
}
