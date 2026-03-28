Лабораторная работа №1: Структура данных

  Задание:

<img width="1143" height="538" alt="image" src="https://github.com/user-attachments/assets/435f143a-1092-42ec-818d-6876ab8164eb" />

Реализация:

Листинг программы:

	import math

	def find_max_gcd_pair(N):
    if N % 2 == 0:
        return N // 2, N // 2

    for i in range(3, int(math.isqrt(N)) + 1, 2):
        if N % i == 0:
            return i, N - i

    return 1, N - 1

	N = int(input())
	A, B = find_max_gcd_pair(N)
	print(A, B,"Манжин Дмитрий Евгеньевич, 090301")
	print('Манжин Дмитрий Евгеньевич, группа 090301-ПОВа-025')
Результат выполнения программы:

<img width="549" height="64" alt="image" src="https://github.com/user-attachments/assets/02be72dc-6e6f-4b5f-82b6-c0c4e482846b" />
