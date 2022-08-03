# heroes-project
Вывести список персонажей в виде таблицы.

API: https://62ea586aad295463258a4036.mockapi.io/hero

Таблица состоит из 4-х колонок:

1) Name Surname
2) Comics (DC, Marvel, Comix Zone)
3) Favourite (чекбокс)
4) Actions (одна кнопка Delete)


Над таблицей форма добавления с тремя полями:

1) Name Surname (input)
2) Comics (DC, Marvel, Comix Zone) (select) – данные запрашиваем методом GET с сущности universes (https://62ea586aad295463258a4036.mockapi.io/universes)
3) Favourite (true, false) (checkbox).


Действия:

1) При сабмите формы происходит добавление персонажа в базу (POST) и вывод в html строки с информацией о герое в таблицу.Если в базе уже существует герой с таким же свойством name, то объект не добавляется в базу (можно просто в консоль вывести инфу, что юзер с таким именем уже есть в базе).
2) При изменении состояния checkbox в колонке Favourite происходит изменение данных по этому персонажу в базе (PUT).
3) При нажатии на кнопку Delete в строке персонажа происходит удаление с базы соответствующего героя (DELETE) и удаление соответствующей tr с таблицы.
