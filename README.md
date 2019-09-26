# WasteBot

### Перед установкой
1) Установите [python3.6](https://www.python.org/downloads/release/python-362/)
2) Установите убедитесь, что установлена поледняя версия ```pip``` для ```python3.6```

### Python
1) Скачайте последний [релиз](https://github.com/kivicode/Public-Releases/releases) ```WasteBot GUI```
2) Установите необходимые библиотеки ```sudo python3.6 -m pip install -r requirements.txt ```
3) На любом компьютере в локальной сети повторите шаги 1 и 2 и запустите сервер ```sh server.py```

> В данном случае клент отправляет сжатое изображение на сервер через сокеты. Сервер обработывает нейронную сеть и отправляет на клиент только результат

> Для тестов можно использовать не второй компьютер, а просто запустить сервер на том же устройстве, что и клиент. 
> В таком случае в шаге 4 установите SERVER_IP как 127.0.0.1

4) На основном компьютере запустите запустите клиент ```python3.6 client.py SERVER_IP``` где SERVER_IP - локальный ip адресс компьютера-сервера
5) Для отправки голосовой команды используйте кнопку ```Listen me```, произнесите комманду из [списка команд](WasteBot/commands.md) и ожидайте несколько секунд (компьютер-клиент должен иметь поключение к интернету).

---

### Симуляция
1. Скачайте последний [релиз симулятора](https://github.com/kivicode/Public-Releases/releases) ```WasteBot Simulation```
2. Модифицируйте или используйте уже готовый файл конфигурации сцены ```Examples/simple_scene.json```
3. Запустите приложение симуляции
4. Укажите полный путь до файла конфигурации сцены в поле в верхнем правом углу
5. Нажмите кнопку ```Load scene``` и убедитесь, что сцена сконфигурирована правильно
6. Нажмите кнопку ```Start simulation``` для запуска симуляции

***
