# Создание логики сокращения ссылки.

# Создаем функцию, выбираем язык python37-preview, в точку входа пишем - index.handler. 
Обратите внимание, что функция должна быть публичная.

Создаем файл index.py и в него записываем код - https://github.com/beeeeemaya/yandex-scale-2020-lab-serverless/blob/master/steps/5/index.py

    
## Редактируем api gw   

Код в файлике gw.yml  https://github.com/beeeeemaya/yandex-scale-2020-lab-serverless/blob/master/steps/5/gw.yml
Пока что нет подключения к базе данных и работы с ней, вместо этого стоят TODO. 
Но уже можно удостовериться в том, что ссылки сокращаются корректно, для этого редактируем наш api-шлюз, добавив в него несколько новых путей. 


## Проверяем
Теперь переходим по адресу шлюза, вводим какую нибудь ссылку в поле для ввода и нажимаем сократить. 
Должна появиться сокращенная ссылка. Осталось добавить логику для заполнения базы данных и получения исходной ссылки по сокращенной ссылке.
