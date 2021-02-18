#include <iostream>
#include <vector>

std::vector<int> merges (int* arr1, int size1, int* arr2, int size2) {
    std::vector<int> v;
    int i = 0;
    int j = 0;
    while ((i != size1) || (j != size2)) {
        if (i == size1) {
            while (j < size2) {
                v.push_back(arr2[j]);
                ++j;
            }
            break;
        } else if (j == size2) {
            while (i < size1) {
                v.push_back(arr1[i]);
                ++i;
            }
            break;
        } else if (arr1[i] < arr2[j]) {
            v.push_back(arr1[i]);
            ++i;
        } else {
            v.push_back(arr2[j]);
            ++j;
        }
    }
    return v;
}

int main()
{
    int size1;
    std::cout << "size_of_first = ";
    std::cin >> size1;
    int* firstArray = new int[size1];
    for (int i = 0; i < size1; i++) {
        std::cin >> firstArray[i];
    }
    int size2;
    std::cout << "size_of_second = ";
    std::cin >> size2;
    int* secondArray = new int[size2];
    for (int i = 0; i < size2; i++) {
        std::cin >> secondArray[i];
    }
    std::vector<int> v = merges(firstArray, size1, secondArray, size2);
    for (int i = 0; i < size1 + size2; i++) {
        std::cout << v[i] << " ";
    }
    std::cout << std::endl;
    return 0;
}
