Task 9.1

Screenshot 1.
Написал функцию fizzbuzz. В цикле for указан иапазон от 1 до 100, далее идут условия с делением нацело каждого числа из диапазона на 3 и 5, на 3 и на 5 и последующими выводами "FizzBuzz", "Fizz" и "Buzz" соответственно при соблюдении условий. На Screenshot 2 показан второй вариант функции с выводом в строку.
![00.png](https://github.com/Iferial/DevOps_online_Dnipro_2020Q42021Q1/blob/main/m9/task9.1/screenshots/00.png)
def fizzbuzz(number):
    for number in range(1,101):
        if number % 3 == 0 and number % 5 == 0:
            print('FizzBuzz') 
        elif number % 3 == 0:
            print('Fizz')
        elif number % 5 == 0:
            print('Buzz')
        else:
            print(number)

print(fizzbuzz(number))
Screenshot 2.
![01.png](https://github.com/Iferial/DevOps_online_Dnipro_2020Q42021Q1/blob/main/m9/task9.1/screenshots/01.png)
def fizzbuzz(x):
    for x in range(1,101):
        if x % 3 == 0 and x % 5 == 0:
            print("FizzBuzz", end=' ')
        elif x % 3 == 0:
            print("Fizz", end=' ')
        elif x % 5 == 0:
            print("Buzz", end=' ')
        else:
            print(x, end=' ')


print(fizzbuzz(x))
Screenshot 3.
На скриншоте ниже реализована функция подсчета гласных из введённого текста. Функция при запуске просит ввести текст при помощи input, далее цикл for проходит по тексту и вычисляет каждое значение, которое есть в заданной мной переменной vowels, при успешной итерации значение count увеличивается на 1 и выводится. На Screenshot 4 второй вариант этой функции, только в одну строку при помощи встроенной функции sum))
![02.png](https://github.com/Iferial/DevOps_online_Dnipro_2020Q42021Q1/blob/main/m9/task9.1/screenshots/02.png)
Screenshot 4.
![03.png](https://github.com/Iferial/DevOps_online_Dnipro_2020Q42021Q1/blob/main/m9/task9.1/screenshots/03.png)
