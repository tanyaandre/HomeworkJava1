# **Краткое описание**

13.03.2021 - 14.03.2021 было проведено функциональное тестирование приложения KeyValidator.class.

**На тестирование затрачено:** 2 часа

**В результате тестирования выявлены следующие дефекты:**

* [При проверке ключей в терминале некоторые валидные ключи распознаются как невалидные](https://github.com/tanyaandre/HomeworkJava1/issues/1)
* [При проверке ключей в терминале некоторые невалидные ключи распознаются как валидные](https://github.com/tanyaandre/HomeworkJava1/issues/2)

# **Описание процесса тестирования**

**В процессе тестирования использовались следующие артефакты:**

1. [Инструкция по установке OpenJDK11](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/openjdk11-manual.md)
2. [Руководство использования программф KeyValidator](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/user-manual.md)
3. [Домашнее задание к занятию «1.1. Введение в Java: JDK, JRE, JVM, IntelliJ IDEA»](https://github.com/netology-code/javaqa-homeworks/tree/master/intro)

**В качестве тестовых данных** использовались данные [Руководства использования KeyValidator](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/user-manual.md):

1. Для данных 00000000-0000-0000-0000-000000000000, 00000000-0000-0000-0000-000000000001 результат:
Result for 00000000-0000-0000-0000-000000000000: OK
Result for 00000000-0000-0000-0000-000000000001: FAIL

Для данных 8f05e6a7-70e9-33d7-bfe7-b19eae0d8998
80b427f8-92cd-3aae-ba04-3927fbe17c6
b295bc63-9f03-3b4b-af80-969b39f8c262
387eedc6-12e9-3b32-9881-63b6b5e85317
c19a8cf9-5c3a-37c5-b7f3-d16d38a0c180
Результат - OK

Для данных 18252235-78e0-44a5-8720-556f0c7da17a
e66075b6-ddad-445e-baf6-161b3289522b
b6d53250-f07e-4352-a293-6102ddf7f1ca
c2bc778a-1cb9-46c6-b435-0489649d2a42
2fb98b44-93e7-3bdd-a2ad-79347bfe4ad1
Результат - FAIL

**Тестирование производилось в следующем окружении:**

Windows 8.1 x64
Java 11
Git 2.30.2
