# Отчёт о тестировании Money_Transfer

## Краткое описание

25.07.2021 было проведено модульное тестирование приложения Money_Transfer.

На тестирование затрачено: 1 час

В результате тестирования выявлены следующие дефекты:
* [Итоговая сумма при выполнении пополнения счета неверна](https://github.com/senselessmessinspace/task_2-1_Money_Transfer/issues/1)

## Описание процесса тестирования

В качестве тестовых данных использовались данные, используя которые при пополнении счёта VIP-клиента что-то пошло не так:
* Данные по счету:

    Текущий баланс счёта клиента - переменная типа int, значение - 2_000_000_000 (два миллиарда рублей);

    Сумма перевода - переменная типа int, значение - 500_000_000 (пятьсот миллионов рублей).

    Ожидаемый результат после перевода суммы - 2500000000 (два миллиарда пятьсот миллионов рублей)

Тестирование производилось в следующем окружении:
* Windows 8.1 x64
* Openjdk version "11.0.11" 2021-04-20
* OpenJDK Runtime Environment AdoptOpenJDK-11.0.11+9 (build 11.0.11+9);
* OpenJDK 64-Bit Server VM AdoptOpenJDK-11.0.11+9 (build 11.0.11+9, mixed mode)