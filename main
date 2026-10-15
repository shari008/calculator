#calculator

import numpy as np

def show_menu():
    print("\n--- Калькулятор Обыкновенный (NumPy) ---")
    print("Доступные операции:")
    print("1. Сложение (+)")
    print("2. Вычитание (-)")
    print("3. Умножение (*)")
    print("4. Деление (/)")
    print("5. Возведение в степень (**)")
    print("6. Квадратный корень (√)")
    print("0. Выход")


def get_number(prompt):
    while True:
        try:
            return float(input(prompt))
        except ValueError:
            print("Ошибка: введите корректное число.")


def calculator():
    while True:
        show_menu()
        choice = input("\nВыберите операцию (0-9): ").strip()

        if choice == "0":
            print("Программа завершена. До свидания!")
            break

        if choice in ["1", "2", "3", "4", "5"]:
            num1 = get_number("Введите первое число: ")
            num2 = get_number("Введите второе число: ")

            if choice == "1":
                result = np.add(num1, num2)
                print(f"Результат: {num1} + {num2} = {result}")
            elif choice == "2":
                result = np.subtract(num1, num2)
                print(f"Результат: {num1} - {num2} = {result}")
            elif choice == "3":
                result = np.multiply(num1, num2)
                print(f"Результат: {num1} * {num2} = {result}")
            elif choice == "4":
                if num2 == 0:
                    print("Ошибка: деление на ноль!")
                else:
                    result = np.divide(num1, num2)
                    print(f"Результат: {num1} / {num2} = {result}")
            elif choice == "5":
                result = np.power(num1, num2)
                print(f"Результат: {num1} ^ {num2} = {result}")

        elif choice == "6":
            num = get_number("Введите число: ")

            if choice == "6":
                if num < 0:
                    print("Ошибка: нельзя взять корень из отрицательного числа!")
                else:
                    result = np.sqrt(num)
                    print(f"Результат: √{num} = {result}")
        else:
            print("Неверный ввод. Пожалуйста, выберите пункт от 0 до 9.")


if __name__ == "__main__":
    calculator()
