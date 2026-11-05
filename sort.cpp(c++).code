#include <iostream>
#include <vector>

using namespace std;

// Функция сортировки пузырьком
void bubbleSort(vector<int>& arr) {
    int n = arr.size();
    
    // Внешний цикл: количество проходов
    for (int i = 0; i < n - 1; i++) {
        bool swapped = false; // Флаг для оптимизации
        
        // Внутренний цикл: сравнение соседних элементов
        // n - i - 1, потому что последние i элементов уже на своих местах
        for (int j = 0; j < n - i - 1; j++) {
            
            // Если текущий элемент больше следующего, меняем их местами
            if (arr[j] > arr[j + 1]) {
                swap(arr[j], arr[j + 1]);
                swapped = true;
            }
        }
        
        // Если за проход не было обменов, массив отсортирован
        if (!swapped) {
            break;
        }
    }
}

// Функция для вывода массива на экран
void printArray(const vector<int>& arr) {
    for (int num : arr) {
        cout << num << " ";
    }
    cout << endl;
}

int main() {
    // Инициализируем вектор (массив) числами
    vector<int> numbers = {64, 34, 25, 12, 22, 11, 90};
    
    cout << "Исходный массив: ";
    printArray(numbers);
    
    // Вызываем сортировку
    bubbleSort(numbers);
    
    cout << "Отсортированный массив: ";
    printArray(numbers);
    
    return 0;
}