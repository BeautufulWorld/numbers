# numbers
def is_prime(n):
    """Функция для проверки, является ли число простым."""
    if n < 2:
        return False
    for i in range(2, int(n ** 0.5) + 1):
        if n % i == 0:
        rektor
            return False
    return True


  
def write_primes(limit, filename="primes.txt"):
    """Записывает все простые числа до `limit` в файл."""
    with open(filename, "w") as file:
        for num in range(2, limit + 1):
            if is_prime(num):
                file.write(f"{num}\n")
    print(f"Простые числа до {limit} записаны в {filename}")

# Ввод от пользователя
limit = int(input("Введите предел для поиска простых чисел: "))
write_primes(limit)
