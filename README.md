#include <stdio.h>
#include <stdbool.h>  // Для типа bool

int main() {
    int A, B, C;
    bool result;
    int positive_count = 0;
    
    // Ввод трех чисел
    printf("Введите три целых числа A, B, C:\n");
    printf("A = ");
    scanf("%d", &A);
    printf("B = ");
    scanf("%d", &B);
    printf("C = ");
    scanf("%d", &C);
    
    // Подсчет положительных чисел
    if (A > 0) positive_count++;
    if (B > 0) positive_count++;
    if (C > 0) positive_count++;
    
    // Проверка: ровно два положительных?
    result = (positive_count == 2);
    
    // Вывод результатов
    printf("\nАнализ чисел:\n");
    printf("A = %d, B = %d, C = %d\n", A, B, C);
    printf("Количество положительных чисел: %d\n", positive_count);
    printf("Утверждение 'Ровно два числа положительные': ");
    
    if (result) {
        printf("ИСТИНА\n");
    } else {
        printf("ЛОЖЬ\n");
    }
    
    return 0;
}
