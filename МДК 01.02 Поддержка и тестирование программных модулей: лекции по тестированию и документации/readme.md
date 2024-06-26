# ЛК1 22.01.24

ОСНОВЫ ТЕСТИРОВАНИЯ 

![image](https://github.com/DanAndy/6_semt/assets/113089418/8cf150f2-597b-43bc-ba0c-98c1c44fb23a)
![image](https://github.com/DanAndy/6_semt/assets/113089418/a51c0ae6-25e5-4d78-b8cc-5cbc11b006b1)
![image](https://github.com/DanAndy/6_semt/assets/113089418/4dfd753f-307a-4b0a-b1b8-b9c5e54e78ba)

Требования к тестировщика: 
  1) Теория тестирования и документация
  2) Знания прдмета который тестируется
  3) Использовать инструменты автоматического тестирования

Тестирование : 
  1) Включен во все активности жизненного цикла
  2) Статическое ( без выполнения кода ) и динамическое ( во время выполнения кода )
  3) Оценивается ожидание и реальность

1) Объект это программа ( что сравнивается ) 
2) Базис тестировнаие ( с чем сравниивается )

Программа может быть : 
  1) Отдельный модуль
  2) Компонент
  3) Подсистема
  4) Система 

Дефект : 
  1) Программа не делает того, что она должна делать
  2) Программа делает то, что не должна деать
  3) Программа делает то, что не упоминалось
  4) Программа неудобна

Ошибка -> Дефект -> Отказ

Пример дефектов : 
  1) Неккоректные требования :
       1) Раскладка клавиатуры 100 на 100
       2) 
![image](https://github.com/DanAndy/6_semt/assets/113089418/504e572e-4674-4cab-a0c0-4f69fbea8c3f)

Ошибка в проектировании :
  1) Неправильная БД

** ВЕРИФИКАЦИЯ VS ВАЛИДАЦИЯ **

![image](https://github.com/DanAndy/6_semt/assets/113089418/07d5d5bf-8143-43aa-9608-bc34cb1f2cfb)

Качество : 
  1) Суъективно
  2) Минимальные требования выполнены
  3) Удовлетворяет потрености

Тестирование и качество : 
  1) обеспечение качества - разраотчик
  2) контроль качетсва - тестировщик

Контроль качества : 
  1) Тестирование
  2) Рецензирование кода
  3) Статический анализ кода
  4) Внешняя оценка и аудит

Обеспечение качества : 
  1) Усовершенствование процессов 
  2) Контроль качества
  3) Упарвление изменениями

**Семь принципов тестирования :** 
  1) Наличие дефектов ( все найти невозможно )
  2) Исчерпывающее тестирование недостижимо
  3) Раннее тестирование ( чем раньше тем лучше )
  4) Скопление дефектов 
  5) Парадокс пестецида ( потвторяя одно и тоже, новые дефекты не найти )
  6) Тестирование зависит от контекста
  7) Заблуждение в отсутствии ошбики ( не забываем про пользователя )


# 12.02.2024 TDD
**Разработка через тестирование.**
Жизненный цикл ПО
Модели жизненного цикла разработки :
  1) Каскадная модель :
      1) Под тестирование выделен один этап. Дефекты во время эксплуатации нельзя исправить.
      2) Нет плана тестирования. 
  2) V - модель :
      1) Тестируется каждый этап, но возврата по прежнему нет.
  3) Итеративная или инкрементальная модель :
       1)![image](https://github.com/DanAndy/6_semt/assets/113089418/e99aa652-b725-4459-a326-f2d0920f6050)
       2) Большие объемы регрессионного тестирования
       3) Отсутствие плана
  4) Спиральная модель
       1) Сложно тестировать на ранних этапах но тестирование становится ключевым этапом

![image](https://github.com/DanAndy/6_semt/assets/113089418/05c4244c-d720-4cb3-b8a0-aa8fa49e9ecf)

![image](https://github.com/DanAndy/6_semt/assets/113089418/67b8ea9f-f469-44b0-b60f-cd2502f4903e)

Уровень тестирования :
  1) Компонентоное
  2) Интеграционное
  3) Системное
  4) Приемочное

Тестирование бывает - статическое и динамическое.
Статическое без исполнения кода, динамическое с исполением кода.
1) Функциональные тесты : 
    1) Поиск в браузере
    2) Создание новых вкладок
    3) Параметры браузера
2) Тесты производительности :
    1) Сколько времени грузит поиск чего либо
    2) Сколько грузит определенные страницы
    3) Скорость перехода по вкладкам
3) Нагрузочные тесты :
    1) Сколько пользователей может пользоваться им одновременно
    2) Сколько запросов может обработать за 1 сек
    3) Тестирование скроллинга и открытие новых вкладок
4) Тестирование совместимости :
    1) НА каких ОС поддерживается
    2) ПРоверка после патчей на каких ОС будет доступен
    3) Тестирование на разных устройствах
5) Позитивные тесты :
    1) Открытие браузера без ошибок
    2) Проверка правильной загрузки страниц
    3) Проверка роботоспасобности открытие вкладок, поиск и тп
6) Негативные тесты :
    1) Открытие неправильного URL адреса который выдаст ошибку
    2) Открытие неправильной созданной страницы
    3) Использование браузера без подключения к интренету
7) Исследовательские тесты :
    1) Тестирование и настройка системы безопасности и хранения личных данных
    2) Исследование настройка интерфейса браузера
    3) Тестирование новых функций добавленных с новой версией браузера
8) Модульное тестирование:
    1) Проверить, что функция регистрации пользователя работает корректно.
    2) Проверить отображение статистики на отдельной странице.
    3) Проверить функционал добавления сообщений на форуме.
9) Интеграционное тестирование:
    1) Залогиниться на форуме, затем перейти на страницу статистики - убедиться, что система продолжает узнавать пользователя.
    2) Проверить совместную работу модуля учета статистики и модуля добавления сообщений - убедиться, что данные корректно обновляются.
    3) Проверить, что основные сценарии использования форума соответствуют ожиданиям при работе в разных разделах.
10) Системное тестирование:
    1) Проверить воспроизведение встроенного видео на форуме.
    2) Убедиться, что изображения отображаются корректно в различных разделах форума.
    3) Проверить корректное отображение текста при использовании различных функций форума
   
# ЛК3 19.02.2024 Дефекты.

Отчет о дефекте - это документ, который содержит информацию о том, что может привести систему к невозможности выполнить требуемую функцию.

![image](https://github.com/DanAndy/6_semt/assets/113089418/9318f048-607f-4c99-b5a7-0017a9049788)


Отчет о дефекте включает в себя:

Идентификатор
Краткое описание: характер проблемы, границы дифекта, последствия дифекта.
Подробное описание: ожидаемые и фактические результаты.
Влияние - степинь дефект. Критичность и приоритет.
Причины почему дефекты не устраняют

Нехватка времини
Дефект вовсе не дефект
Устранить неисправность слишком рисковано
Это того не стоит
Неэффективный отчет о дефектах
Упражнение:

Идентификатор: 1

Краткое описание: Сложение четных чисел происходит неверно

Подробное описание: В ходе сложения двух четных результат больше на 1, чем должно было быть

Шаги:

Открыть калькулятор

Нажатие на четное число №1

Нажатие на +

Нажатие на четное число №2

Нажатие на =

Ожидаемый результат: четное число 1 + четное число 2 = четная сумма чисел

Фактический результат: четное число 1 + четное число 2 = нечетная сумма чисел

Влияние: критический дефект, сложение важная математическа операция.

Тестовый сценарий

Тестовый набор: тестовые сценарий, тестовые данные или правило генерации тестовых данных.

Выбор данных: покрытие операторов, покрытие узлов ветвления, комбинаторное покрытие условий.

Классы эквивалентности - одинаковая верояность обнаружения конкретного типа обнаружения.

Задание телефон https://docs.google.com/document/d/1sHSNe2zvoUOkp4Pa3Vziefj0eyd10DrPCe11BxJ5gVE/edit?usp=sharing

# !! ВАЖНО https://docs.google.com/document/d/1HOLKqPUAQFTGmtaQGacwKFFMZiCr6q8s/edit#heading=h.gjdgxs  !!

# Unit test 

Unit тест - блок кода (обычно метод), который вызывает
тестируемый блок кода и проверяет правильность его
работы. Если результат юнит-теста не совпадает с
ожидаемым результатом, тест считается не пройденным
Должен проверять одно действие и быть
универсальным

Uint testы - Функция, которая проверяет одно действие из кода, есть ожидаемые результаты, если он не получен, то тест не пройден. 

** Именование проекта **

На демоэкзамене могут снять баллы, если даны названия функций, а вы их не использовали 

** 23.04.2024 **

https://drive.google.com/drive/folders/1uSLYp6sysN3RDsxJuvqs-rRF_86xz2Ui?usp=drive_link
