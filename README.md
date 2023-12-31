# План внедрения автоматизации возможности записаться на обучение профессии «Тестировщик ПО»
## Перечень автоматизируемых сценариев:
### Валидные данные для ввода в форму записи:
* **Имя** - состоит из символов на кириллице или латинице, длиной от 1 до 64, с возможностью использования символов: "пробел", "дефис", "апостроф".
* **Номер телефона** - состоит из 11 цифр - **79991234567**
* **Электронная почта** - состоит из имени пользователя , символа "@", имени хоста и домена первого уровня, разделенных "." - **username@hostname.domen**
### Позитивный Е2Е сценарий записи на обучение профессии «Тестировщик ПО» для незарегистрированного пользователя c главной страницы https://netology.ru путем:
1. Нажать кнопу "Каталог курсов" в "шапке" страницы
2. Нажать кнопку "Все курсы"
3. Нажать на блок «Тестировщик ПО»
4. Нажать кнопку "Записаться"
5. Ввести валидные данные в форму записи
6. Нажать кнопку "Записаться" в форме записи
* **Ожидаемый результат:** сообщение об успешной отправке формы, появление записи в базе данных
### Позитивный Е2Е сценарий записи на обучение профессии «Тестировщик ПО» для зарегистрированного, авторизованного пользователя c главной страницы https://netology.ru путем:
1. Нажать кнопу "Каталог курсов" в "шапке" страницы
2. Нажать кнопку "Все курсы"
3. Нажать на блок «Тестировщик ПО»
4. Нажать кнопку "Записаться"
5. Нажать кнопку "Записаться" в форме записи
* **Ожидаемый результат:** сообщение об успешной отправке формы, появление записи в базе данных
### Переход на страницу курса «Тестировщик ПО» c главной страницы https://netology.ru путем:
**№1**
1. Нажать кнопу "Каталог курсов" в "шапке" страницы
2. Нажать кнопку "Программирование"
3. Нажать на блок «Тестировщик ПО»
* **Ожидаемый результат:** переход на страницу курса «Тестировщик ПО» https://netology.ru/programs/qa

**№2**
1. Нажать кнопу "Каталог курсов" в "шапке" страницы
2. Ввести в поле "Какой курс вам нужен?" первые две буквы названия професии
3. Нажать блок «Тестировщик ПО»
* **Ожидаемый результат:** переход на страницу курса «Тестировщик ПО» https://netology.ru/programs/qa

**№3**
1. Нажать на раздел "Программирование" в блоке "Направления обучения"
2. Нажать на блок «Тестировщик ПО»
* **Ожидаемый результат:** переход на страницу курса «Тестировщик ПО» https://netology.ru/programs/qa

**№4**
1. Нажать нажать "Программирование" в блоке "Направления обучения"
2. Ввести в поле "Какой курс вам нужен?" первые две буквы названия професии
3. Нажать на блок «Тестировщик ПО»
* **Ожидаемый результат:** переход на страницу курса «Тестировщик ПО» https://netology.ru/programs/qa

**№5**
1. Нажать кнопу "Каталог курсов" в "подвале" страницы
2. Нажать на блок «Тестировщик ПО»
* **Ожидаемый результат:** переход на страницу курса «Тестировщик ПО» https://netology.ru/programs/qa

**№6**
1. Нажать кнопу "Программирование" в "подвале" страницы
2. Нажать на блок «Тестировщик ПО»
* **Ожидаемый результат:** переход на страницу курса «Тестировщик ПО» https://netology.ru/programs/qa
### Переход к форме заполнения для записи со страницы курса «Тестировщик ПО» https://netology.ru/programs/qa
#### №1
1. Пролистать страницу до формы записи
* **Ожидаемый результат:** переход к форме заполнения https://netology.ru/programs/qa#/order

#### №2
1. Нажать кнопу "Записаться" в "шапке" страницы
* **Ожидаемый результат:** переход к форме заполнения https://netology.ru/programs/qa#/order
### Заполение невалидными данными поля "имя" формы для записи на странице https://netology.ru/programs/qa#/order
#### №1
**Входные данные:**
* Невалидное имя с цифрой - Иван1
* Валидный номер телефона
* Валидный адрес электронной почты 
1. Заполнить невалидными данными поле "имя"
2. Заполнить валидными данными поле номера телефона
3. Заполнить валидными данными поле "Электронная почта"
4. Нажать кнопку "Записаться"
* **Ожидаемый результат:** форма не отправится с сообщением о неправильно заполенном поле

#### №2
**Входные данные:**
* Невалидное имя с символом * - Иван*
* Валидный номер телефона
* Валидный адрес электронной почты 
1. Заполнить невалидными данными поле "имя"
2. Заполнить валидными данными поле номера телефона
3. Заполнить валидными данными поле "Электронная почта"
4. Нажать кнопку "Записаться"
* **Ожидаемый результат:** форма не отправится с сообщением о неправильно заполенном поле

#### №3
**Входные данные:**
* Невалидное имя с символом @ - Иван@
* Валидный номер телефона
* Валидный адрес электронной почты 
1. Заполнить невалидными данными поле "имя"
2. Заполнить валидными данными поле номера телефона
3. Заполнить валидными данными поле "Электронная почта"
4. Нажать кнопку "Записаться"
* **Ожидаемый результат:** форма не отправится с сообщением о неправильно заполенном поле
### Заполение данных граничными значениями поля "имя" формы для записи на странице https://netology.ru/programs/qa#/order
#### №1
**Входные данные:**
* Значение имени состоящее из одного символа - И
* Валидный номер телефона
* Валидный адрес электронной почты
1. Заполнить валидными данными поле "имя" длинной 1 символ
2. Заполнить валидными данными поле номера телефона
3. Заполнить валидными данными поле "Электронная почта"
4. Нажать кнопку "Записаться"
* **Ожидаемый результат:** сообщение об успешной отправке формы

#### №2
**Входные данные:**
* Значение имени состоящее из 64 символов на кириллице
* Валидный номер телефона
* Валидный адрес электронной почты
1. Заполнить валидными данными поле "имя" длинной из 64 символов на кириллице
2. Заполнить валидными данными поле номера телефона
3. Заполнить валидными данными поле "Электронная почта"
4. Нажать кнопку "Записаться"
* **Ожидаемый результат:** сообщение об успешной отправке формы

#### №3
**Входные данные:**
* Значение имени состоящее из 65 символов на кириллице
* Валидный номер телефона
* Валидный адресс электронной почты
1. Заполнить данными поле "имя" длинной из 65 символов на кириллице
2. Заполнить валидными данными поле номера телефона
3. Заполнить валидными данными поле "Электронная почта"
4. Нажать кнопку "Записаться"
* **Ожидаемый результат:** форма не отправится с сообщением об ограничении длинны ввода символов
### Заполение граничными значениями поля номера телефона формы для записи на странице https://netology.ru/programs/qa#/order
#### №1
**Входные данные:**
* Валидное имя
* Значение из 10 цифр номнра телефона
* Валидный адрес электронной почты
1. Заполнить валидными данными поле "имя"
2. Заполнить поле номера телефона значением из 10 цифр
3. Заполнить валидными данными поле "Электронная почта"
4. Нажать кнопку "Записаться"
* **Ожидаемый результат:** форма не отправится с сообщением о неправильно заполенном поле

#### №2
**Входные данные:**
* Валидное имя
* Значение из 12 цифр номнра телефона
* Валидный адрес электронной почты
1. Заполнить валидными данными поле "имя"
2. Заполнить поле номера телефона значением из 12 цифр
3. Заполнить валидными данными поле "Электронная почта"
4. Нажать кнопку "Записаться"
* **Ожидаемый результат:** форма не отправится с сообщением о неправильно заполенном поле
### Заполение невалидными данными поля "Электронная почта" формы для записи на странице https://netology.ru/programs/qa#/order
#### №1
**Входные данные:**
* Валидное имя
* Валидное значение номера телефона
* Невалидный адрес электронной почты без имени пользователя - @hostname.domen
1. Заполнить валидными данными поле "имя"
2. Заполнить валидными данными поле номера телефона
3. Заполнить невалидными данными, без имени пользователя, поле "Электронная почта"
4. Нажать кнопку "Записаться"
* **Ожидаемый результат:** форма не отправится с сообщением о неправильно заполенном поле

#### №2
**Входные данные:**
* Валидное имя
* Валидное значение номера телефона
* Невалидный адрес электронной почты без символа @ - usernamehostname.domen
1. Заполнить валидными данными поле "имя"
2. Заполнить валидными данными поле номера телефона
3. Заполнить невалидными данными, без символа @, поле "Электронная почта"
4. Нажать кнопку "Записаться"
* **Ожидаемый результат:** форма не отправится с сообщением о неправильно заполенном поле

#### №3
**Входные данные:**
* Валидное имя
* Валидное значение номера телефона
* Невалидный адрес электронной почты без имени хоста - username@.domen
1. Заполнить валидными данными поле "имя"
2. Заполнить валидными данными поле номера телефона
3. Заполнить невалидными данными, без имени хоста, поле "Электронная почта"
4. Нажать кнопку "Записаться"
* **Ожидаемый результат:** форма не отправится с сообщением о неправильно заполенном поле

#### №4
**Входные данные:**
* Валидное имя
* Валидное значение номера телефона
* Невалидный адрес электронной почты без домена первого уровня - username@hostname
1. Заполнить валидными данными поле "имя"
2. Заполнить валидными данными поле номера телефона
3. Заполнить невалидными данными, без имени домена первого уровня, поле "Электронная почта"
4. Нажать кнопку "Записаться"
* **Ожидаемый результат:** форма не отправится с сообщением о неправильно заполенном поле
### Оставление поля пустым в форме для записи на странице https://netology.ru/programs/qa#/order
#### №1
1. Оставить поле "имя" пустым
2. Заполнить валидными данными поле номера телефона
3. Заполнить валидными данными поле "Электронная почта"
4. Нажать кнопку "Записаться"
* **Ожидаемый результат:** форма не отправится с сообщением об обязательном заполнении поля

#### №2
1. Заполнить валидными данными поле "имя"
2. Оставить поле номера телефона пустым
3. Заполнить валидными данными поле "Электронная почта"
4. Нажать кнопку "Записаться"
* **Ожидаемый результат:** форма не отправится с сообщением об обязательном заполнении поля

#### №3
1. Заполнить валидными данными поле "имя"
2. Заполнить валидными данными поле номера телефона
3. Оставить поле "Электронная почта" пустым
4. Нажать кнопку "Записаться"
* **Ожидаемый результат:** форма не отправится с сообщением об обязательном заполнении поля
## Перечень используемых инструментов с обоснованием выбора:
* IntelliJ IDEA - инструмет для написания и редактирования кода
* Java - язык программирования для написания автотестов
* Gradle - сборка проекта
* Selenide - для тестирования UI
* Faker - для генерации данных
* DBUtils - для взаимодействия с базой данных
* Lombok - для удобства написания кода
* Allure - для формирования отчетов
* Git и GitHub - контроль версий
## Перечень и описание возможных рисков при автоматизации:
* В HTML не у всех элементов есть тестовые метки "data test id"
* Классы в HTML сгенерированы автоматически
## Перечень необходимых разрешений, данных и доступов:
* Разрешение на тестирование
* Техническая документация
* Доступ к базе данных
## Перечень необходимых специалистов для автоматизации:
* Один QA engineer
## Интервальная оценка с учётом рисков в часах:
* 112 часов