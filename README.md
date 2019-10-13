### Для начала сделай форк этого репозитория

## Запуск проекта

### `yarn`

### `yarn start`

Открыть в браузере [http://localhost:3000](http://localhost:3000)

### Все вопросы по заданию пиши в чат

[Телеграм-чат ReactWarriors](https://t.me/rw_master_class)

### Решение задания отправляй мне в личку

[Мой телеграм](https://t.me/evgeniypodgaetskiy)

### Разбор решения этого задания и код-ревью, кто прислал свое решение

### Проведу 19 октября в 12:00. Ссылку на трансляцию отправлю за 1 час

### Задание

Нужно написать таблицу, по функционалу похожую на табличек в программе Excel.

То есть, написанный веб приложение должно представлять собой окно, где есть таблица, в ячейки которой можно записывать числа, строки, денежные суммы, ссылки и формулы.

Должен также быть строка, в которой мы будем видеть формальный запись содержимого ячейки, на которую кликнули. Например. Есть ячейка с координатами (1,4), в ней записано ссылки https://reactwarriors.com. Тогда в этой строке должно быть выведено что-то типа = HYPERLINK ( 'https://reactwarriors.com").

Вот формулы, которые нужно реализовать:
сумма чисел в ячейках (= SUM (...) допустимые типы - числа и денежные суммы. Числа к деньгам добавлять нельзя. Только деньги к деньгам и числа до цифр.)
среднее арифметическое выбранных ячеек (= AVERAGE (...), условия такие же.)
конкатенация строк в выбранных ячеек (= CONCAT (...), конкатенуваты можно различные типы данных. Они просто приводятся к строке.)
гиперссылки (= HYPERLINK (...) должна быть валидация на то, что ссылки валидных. Например: https: //asdasdasd.asd - хоть и не действительное ссылки, но семантика подходит, asd: // asdsad ---- asd-asd -asd - не валидный ссылка).

Если в формулу попадает ячейка с недопустимым типом данных - нужно показать сообщение об ошибке.

Денежные суммы нужно реализовать следующим образом:
формат записи: 1300 000,00 - целую часть необходимо разбить на тройки цифрам. Дробная часть имеет всегда состоять из 2 знакиив после запятой (не больше и не меньше).
Также должна быть возможность указать валюту.

Необходимо использовать следующие технологии: React + Redux. Для компонент, которые могут быть классами (не обязательно для всех), использовать новую возможность в React - Hooks (https://reactjs.org/docs/hooks-intro.html)

Бонусные задания:
если фокус курсора стоит на клетке, в которой записано ссылки, то где-то на экране зньявляеться область Превью, в которой мы видим небольшое изображение страницы, на которую ведет ссылка, или сообщение о том, что превью матча. Для ячеек с другими формулами и типами эта область не должна показываться.
