# Zinchenko_Kostya_dz_1
домашнее задание за 1 урок


# Задание 1
 duration = int(input('Введите время в секундах: '))
 days = duration // (60 * 60 * 24)
 hours = (duration - days * (60 * 60 * 24)) // (60 * 60)
 minutes = (duration - days * (60 * 60 * 24) - hours * (60 * 60)) // 60
 seconds = duration - days * (60 * 60 * 24) - hours * (60 * 60) - minutes * 60
 print(days, 'дн', hours, 'час', minutes, 'мин', seconds, 'сек')


# Задание 2


my_list = []
for num in range(1, 1001, 2):
    my_list.append(num ** 3)
# a
final_sum = 0  # финальный ответ
for num in my_list:
    check_sum = 0  # сумма всех цифр конкретного числа
    for check_num in str(num):
        check_sum += int(check_num)
    if check_sum % 7 == 0:
        final_sum += num
print(final_sum)

# b&c
final_sum = 0
for num in my_list:
    num += 17  # отличие от a
    check_sum = 0
    for check_num in str(num):
        check_sum += int(check_num)
    if check_sum % 7 == 0:
        final_sum += num
print(final_sum)



# Задание 3
 

percent = int(input('Введите число процента: '))
if percent == 1:
    word = 'процент'
elif percent <= 4:
    word = 'процента'
else:
    word = 'процентов'
print(percent, word)
