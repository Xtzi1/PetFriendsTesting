# PetFriendsTesting

автотесты для https://petfriends.skillfactory.ru/apidocs/#/default/delete_api_pets__pet_id_
содержатся в файле test_pet_friends.py

используемые библиотеки:
pytest, json, os, requests, python-dotenv

при запуске 2 из 15 тестов упадут, т.к. обнаружены баги:
при создании пета с пустыми полями, сервер возвращает 200, публикация с пустыми значениями возможна
обновление информации о существующем пете методом PUT c пустыми полями тоже возвращает 200
вот и баги.
