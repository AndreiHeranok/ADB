__ADB_HW__


Сценарий напишите в .txt файл.
.txt сценарий и .log файл прииложения todolist выгружайте на GitHub.
Ссылкку на гитхаб присылайте в лс.   

1. Отобразить подключённый девайс в консоли.
    ```adb devices```

2. Вывести адрес приложения todolist в системе Android
   ```adb shell pm list packages | grep todolist```

3. Установить .apk файл приложениия todolist на телефон с компьютера через  ADB
   ```adb install C:\Users\andre\Desktop\ksendzov\app-debug.apk```
 
4. Сделать скриншот запущенного приложения todolist и сразу скопировать на компьютер в одной команде.
   ```adb shell screencap /sdcard/123.png | adb pull /sdcard/123.png C:/Users/Andre/Downloads```

5. Вывести в консоль логи приложения todolist
   ```adb shell "logcat | grep -nw com.android.todolist"```

6. Скопировать логи приложения todolist на компьютер.
   ```adb shell "logcat | grep -nw com.android.todolist" > C:\Users\Andre\Desktop\log_todolist.log```

7. Удалить приложение todolist с телефона через ADB
   ```adb uninstall com.android.todolist```