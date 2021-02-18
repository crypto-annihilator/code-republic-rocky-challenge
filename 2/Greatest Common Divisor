#include <iostream>

int greatest_Common_Divisor (int& first, int& second)
{
    while (first != second) {
        if (first > second) {
            first -= second;
        } else {
            second -= first;
        }
    }
    return first;
}

int main()
{
    int first;
    int second;
    std::cout << "first_number = ";
    std::cin >> first;
    std::cout << "second_number = ";
    std::cin >> second;
    std::cout << "greatest common divisor = ";
    std::cout << greatest_Common_Divisor(first, second) << std::endl;
    return 0;
}
