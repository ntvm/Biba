
Спасибо Фиксерам с двача      https://rentry.org/BibaUpdated

____

<h1 align="center">Biba</h1>

## Что это?
Подвязка GPT-4 бота Сидни с Бинга к Таверне

## Что можно?
Смут.</br>
14-20к токенов.</br>
Кодинг с рабочим стримом (плюс в сравнении со скалой).</br>
Подтягивать данные из интернета.</br></br>
![image](https://github.com/Barbariskaa/Biba/assets/129290831/b5176621-4a1f-4b57-9c7f-865861825c30)</br></br>
Подтягивать подсказки из бинга (через /suggestion после указанного в URL режима).</br></br>
![image](https://user-images.githubusercontent.com/129290831/236729981-42f4cbf8-abbd-4deb-9a70-1a1cb5917119.png)

## Что по куму?
Ответы с сервера фильтруются посреди стрима, прямо как в чае. В среднем обрубает на 100 токенах и до нескольких сотен. Зависит от выбранного режима.<br>
Возможно это ограничение можно обойти, если повозиться с промптами.</br>
Остановленные ответы соединяются в один большой.</br>
Также банят. Могут забанить за один день, а могут и вовсе нет. Решается перерегом.</br>
С 29.05.2023г. с Российских IP могут возникать проблемы в работе если пользоваться скриптом без VPN.

## Как поставить?
Клонируем репозиторий и запускаем start.bat / start.sh</br>
Команды которые нужно ввести перед запуском start.sh на Linux:

```
chmod 775 start.sh
sudo apt-update
sudo apt-get install python-is-python3
sudo apt install python3.10-venv
./start.sh
```

После установки нужно собрать куки. Они не обязательны, но без них частые проблемы с работой скрипта. Ниже описано как получить их:<br>
* [Логинимся](https://login.live.com/login.srf) или [регистрируем](https://signup.live.com/signup) учетку в Майкрософт.
* Заходим в сам [чат](https://www.bing.com/search?q=Bing+AI&showconv=1&wlsso=0) с Бингом с Эджа. Если отобразился поисковик, а не чат, ниже описано как заставить чат работать: 

Не через Edge придется ставить сторонний юзерагент. Можно поставить следующий:</br> `Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/111.0.1661.51`</br></br>
Также, санкционным анонам придется повозиться с доступом к Бингу. Рекомендую использовать впн и чистить куки, затем искать в самом бинге Bing AI или перейти по ссылке выше. Если нет кнопки перехода в чат, значит нужно либо чистить куки еще раз, выйдя из учетной записи в браузере и поисковике, либо пробовать другой айпи впна.</br></br>
![image](https://user-images.githubusercontent.com/129290831/236732426-91d87aa3-32e2-4f87-9758-ac5c4b222a71.png) </br>

После успешного захода и открытия чата, нужно экспортировать сами куки. Для этого устанавливаем следующий плагин:
* Chrome/Edge: https://chrome.google.com/webstore/detail/cookie-editor/hlkenndednhfkekhgcdicdfddnkalmdm
* Firefox: https://addons.mozilla.org/en-US/firefox/addon/cookie-editor/

Открываем расширение Cookie Editor. 
* Жмем export снизу справа расширения, жем `Export as JSON`. Куки сохранятся в буфер.
* Заходим в папку со скриптом.
* Создаем файл cookies.json.
* Открываем файл в текстовом редакторе и вставляем скопированный текст куки файла. Сохраняем.
* Затем запускаем сам скрипт через батник. 
 
После этого должно заработать.

# Отдельные упоминания и благодарности
https://github.com/acheong08/EdgeGPT</br>
https://github.com/InterestingDarkness/EdgeGPT</br>
