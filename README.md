# Postman

HW_1

Создать запросы в Postman.

Protocol: http IP: 162.55.220.72 Port: 5005

EP_1
Method: GET
EndPoint: /get_method
request url params: 
name: str
age: int

response: [ “Str”, “Str” ]

==================

EP_2
Method: POST
EndPoint: /user_info_3
request form data: 
name: str
age: int
salary: int

response: {'name': name, 'age': age, 'salary': salary, 'family': {'children': [['Alex', 24], ['Kate', 12]], 'u_salary_1_5_year': salary * 4}}

==================

EP_3
Method: GET
EndPoint: /object_info_1
request url params: 
name: str
age: int
weight: int

response: {'name': name, 'age': age, 'daily_food': weight * 0.012, 'daily_sleep': weight * 2.5}

==================

EP_4
Method: GET
EndPoint: /object_info_2
request url params: 
name: str
age: int
salary: int

response: {'start_qa_salary': salary, 'qa_salary_after_6_months': salary * 2, 'qa_salary_after_12_months': salary * 2.7, 'qa_salary_after_1.5_year': salary * 3.3, 'qa_salary_after_3.5_years': salary * 3.8, 'person': {'u_name': [user_name, salary, age], 'u_age': age, 'u_salary_5_years': salary * 4.2} }

==================

EP_5
Method: GET
EndPoint: /object_info_3
request url params: 
name: str
age: int
salary: int

response: {'name': name, 'age': age, 'salary': salary, 'family': {'children': [['Alex', 24], ['Kate', 12]], 'pets': {'cat':{'name':'Sunny', 'age': 3}, 'dog':{'name':'Luky', 'age': 4}}, 'u_salary_1_5_year': salary * 4} }

==================

EP_6
Method: GET
EndPoint: /object_info_4
request url params: 
name: str
age: int
salary: int

response: {'name': name, 'age': int(age), 'salary': [salary, str(salary * 2), str(salary * 3)]}

==================

EP_7
Method: POST
EndPoint: /user_info_2
request form data: 
name: str
age: int
salary: int

response: {'start_qa_salary': salary, 'qa_salary_after_6_months': salary * 2, 'qa_salary_after_12_months': salary * 2.7, 'qa_salary_after_1.5_year': salary * 3.3, 'qa_salary_after_3.5_years': salary * 3.8, 'person': {'u_name': [user_name, salary, age], 'u_age': age, 'u_salary_5_years': salary * 4.2} }

HW_2

http://162.55.220.72:5005/first

Отправить запрос.
Статус код 200
Проверить, что в body приходит правильный string.
http://162.55.220.72:5005/user_info_3

Отправить запрос.
Статус код 200
Спарсить response body в json.
Проверить, что name в ответе равно name s request (name вбить руками.)
Проверить, что age в ответе равно age s request (age вбить руками.)
Проверить, что salary в ответе равно salary s request (salary вбить руками.)
Спарсить request.
Проверить, что name в ответе равно name s request (name забрать из request.)
Проверить, что age в ответе равно age s request (age забрать из request.)
Проверить, что salary в ответе равно salary s request (salary забрать из request.)
Вывести в консоль параметр family из response.
Проверить что u_salary_1_5_year в ответе равно salary*4 (salary забрать из request)
http://162.55.220.72:5005/object_info_3

Отправить запрос.
Статус код 200
Спарсить response body в json.
Спарсить request.
Проверить, что name в ответе равно name s request (name забрать из request.)
Проверить, что age в ответе равно age s request (age забрать из request.)
Проверить, что salary в ответе равно salary s request (salary забрать из request.)
Вывести в консоль параметр family из response.
Проверить, что у параметра dog есть параметры name.
Проверить, что у параметра dog есть параметры age.
Проверить, что параметр name имеет значение Luky.
Проверить, что параметр age имеет значение 4.
http://162.55.220.72:5005/object_info_4

Отправить запрос.
Статус код 200
Спарсить response body в json.
Спарсить request.
Проверить, что name в ответе равно name s request (name забрать из request.)
Проверить, что age в ответе равно age из request (age забрать из request.)
Вывести в консоль параметр salary из request.
Вывести в консоль параметр salary из response.
Вывести в консоль 0-й элемент параметра salary из response.
Вывести в консоль 1-й элемент параметра salary параметр salary из response.
Вывести в консоль 2-й элемент параметра salary параметр salary из response.
Проверить, что 0-й элемент параметра salary равен salary из request (salary забрать из request.)
Проверить, что 1-й элемент параметра salary равен salary*2 из request (salary забрать из request.)
Проверить, что 2-й элемент параметра salary равен salary*3 из request (salary забрать из request.)
Создать в окружении переменную name
Создать в окружении переменную age
Создать в окружении переменную salary
Передать в окружение переменную name
Передать в окружение переменную age
Передать в окружение переменную salary
Написать цикл который выведет в консоль по порядку элементы списка из параметра salary.
http://162.55.220.72:5005/user_info_2

Вставить параметр salary из окружения в request
Вставить параметр age из окружения в age
Вставить параметр name из окружения в name
Отправить запрос.
Статус код 200
Спарсить response body в json.
Спарсить request.
Проверить, что json response имеет параметр start_qa_salary
Проверить, что json response имеет параметр qa_salary_after_6_months
Проверить, что json response имеет параметр qa_salary_after_12_months
Проверить, что json response имеет параметр qa_salary_after_1.5_year
Проверить, что json response имеет параметр qa_salary_after_3.5_years
Проверить, что json response имеет параметр person
Проверить, что параметр start_qa_salary равен salary из request (salary забрать из request.)
Проверить, что параметр qa_salary_after_6_months равен salary*2 из request (salary забрать из request.)
Проверить, что параметр qa_salary_after_12_months равен salary*2.7 из request (salary забрать из request.)
Проверить, что параметр qa_salary_after_1.5_year равен salary*3.3 из request (salary забрать из request.)
Проверить, что параметр qa_salary_after_3.5_years равен salary*3.8 из request (salary забрать из request.)
Проверить, что в параметре person, 1-й элемент из u_name равен salary из request (salary забрать из request.)
Проверить, что что параметр u_age равен age из request (age забрать из request.)
Проверить, что параметр u_salary_5_years равен salary*4.2 из request (salary забрать из request.)
***Написать цикл который выведет в консоль по порядку элементы списка из параметра person.

HW_2*

http://162.55.220.72:5005/user_info_2 

1. Необходимо провести тестирование API данного эндпоинта на валидацию входных параметров. Суть задания: проверить валидации каждого поля, подаваемого в эндпоинт на возможные значения. Будем УСЛОВНО считать, что негативная проверка должна возвращать какой угодно статус НО НЕ 200! Ваша задача написать тест кейсы в постмане таким образом, что одна негативная проверка - один запрос, позитивные проверки можно объединять в 1. Ваша задача протестировать исходя из требований на все возможные аспекты. В каждом запросе тест ТОЛЬКО НА СТАТУС КОД (200 - позитивное значение, не 200 - негативное). P.S. ЗАДАНИЕ НЕ ПОДРАЗУМЕВАЕТ, ЧТО ЭНДПОИНТ РАБОТАЕТ СОГЛАСНО НАПИСАННЫМ ТРЕБОВАНИЯМ. МЫ УЧИМСЯ ПИСАТЬ ТЕСТЫ НА API! 
Требования: 
Name: 3-40 символов включительно, запрещены префиксные и постфиксные пробелы. Поле обязательное
Age: только целые цифры в диапазоне 18-120 включительно. Поле обязательное
Salary: только целые цифры в диапазоне 1-1000000 включительно. Поле обязательное

1****.
Преобразовать задание 1 таким образом, чтобы вы отправляли параметры через CSV файл. У вас будет ровно 1 запрос в коллекции, который будет повторяться столько раз, сколько строк в CSV файле. Также должна быть написана функция в тестах, которая проверяет валидность входящих данных, и в зависимости от этого проверяет на статус 200 или НЕ 200.

2. http://162.55.220.72:5007/object_info_4 Преобразовать пункты 12-13-14 (salary из реквеста и респонса равны) таким образом, чтобы проверка производилась циклом, в котором будет всего ОДИН тест. Имя теста должно меняться в зависимости от значения в Salary

3. http://162.55.220.72:5005/object_info_3 Преобразовать задания 5-7 (сравнить идентичные поля в реквесте и респонсе) таким образом, чтобы это делалось ЗА ОДИН ТЕСТ (сразу все 3 поля) БЕЗ ЦИКЛОВ! (глубокое сравнение объектов)

4. http://162.55.220.72:5005/user_info_2
1) Преобразовать задания 8 - 13 (проверить что в json имеется нужный параметр) таким образом, чтобы все проверки делались в цикле (1 проверка в цикле, в которую попадают нужные параметры). Название теста должно видоизменяться исходя из подаваемых данных. ( ${} или другим способом)
2) ** Преобразовать задания 14 - 18 (проверить что параметр равен salary умножить на коэффициент) таким образом, чтобы все проверки делались в цикле (1 проверка в цикле, в которую попадают нужные параметры). Название теста должно видоизменяться исходя из подаваемых данных. ( ${} или другим способом)
3) *** Преобразовать описанные выше задания 1 и 2 для данного эндпоинта в ОДИН ЦИКЛ, в котором будут проходить ОБА теста.

HW_3

1) Необходимо залогиниться.
POST
http://162.55.220.72:5005/login
login : str (кроме /)
password : str

Приходящий токен необходимо передать во все остальные запросы.

===================
Дальше все запросы требуют наличие токена.
===================

2) http://162.55.220.72:5005/user_info
req. (RAW JSON)
POST
age: int
salary: int
name: str
auth_token


resp.
{'start_qa_salary':salary,
 'qa_salary_after_6_months': salary * 2,
 'qa_salary_after_12_months': salary * 2.9,
 'person': {'u_name':[user_name, salary, age],
                                'u_age':age,
                                'u_salary_1.5_year': salary * 4}
                                }

Тесты:
1) Статус код 200.
2) Проверка структуры json в ответе.
3) В ответе указаны коэффициенты умножения salary, напишите тесты по проверке правильности результата перемножения на коэффициент.
4) Достать значение из поля 'u_salary_1.5_year' и передать в поле salary запроса http://162.55.220.72:5005/get_test_user
===================
3) http://162.55.220.72:5005/new_data
req.
POST
age: int
salary: int
name: str
auth_token

Resp.
{'name':name,
  'age': int(age),
  'salary': [salary, str(salary*2), str(salary*3)]}

Тесты:
1) Статус код 200.
2) Проверка структуры json в ответе.
3) В ответе указаны коэффициенты умножения salary, напишите тесты по проверке правильности результата перемножения на коэффициент.
4) проверить, что 2-й элемент массива salary больше 1-го и 0-го.
===================
4) http://162.55.220.72:5005/test_pet_info
req.
POST
age: int
weight: int
name: str
auth_token

Resp.
{'name': name,
 'age': age,
 'daily_food':weight * 0.012,
 'daily_sleep': weight * 2.5}

Тесты:
1) Статус код 200.
2) Проверка структуры json в ответе.
3) В ответе указаны коэффициенты умножения weight, напишите тесты по проверке правильности результата перемножения на коэффициент.

5) http://162.55.220.72:5005/get_test_user
req.
POST
age: int
salary: int
name: str
auth_token

Resp.
{'name': name,
 'age':age,
 'salary': salary,
 'family':{'children':[['Alex', 24],['Kate', 12]],
 'u_salary_1.5_year': salary * 4}
  }

Тесты:
1) Статус код 200.
2) Проверка структуры json в ответе.
3) Проверить что занчение поля name = значению переменной name из окружения.
4) Проверить что занчение поля age в ответе соответсвует отправленному в запросе значению поля age.
