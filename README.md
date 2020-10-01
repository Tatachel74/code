 Установка GIT
Git - одна из самых популярных систем контроля версий, используется разработчиками, для контроля изменений в своих разработках и проектах. Изначально создан для использования на Linux-подобных операционных системах, но позднее, из-за удобства и популярности для Windows был написан специальный эмулятор, поддерживающий функционал Git’a.

Начало работы
Загрузите установщик с[офиц.сайт](https://git-scm.com/downloads)

Установка и запуск
1 Перейдите в папку “Downloads” и запустите на исполнение загруженный файл   
2  Укажите путь до каталога в который будет установлен Git.      
3 Чтобы на рабочем столе была иконка Git, на следующем шаге отметьте галочкой “On the Desktop”.
4 Введите имя директории, которая будет создана в Start Menu. При необходимости можно изменить путь с помощью кнопки Browse.

5 Выберете способ использования из командной строки:
-Use Git from Git Bash only - использование только из командной строки Bash.
-Use Git from the Windows Command Prompt - использование командной строки Bash, а также минимальный набор команд Git из консоли Windows.
-Use Git and optional Unix tools from the Windows Command Prompt - использование Git и утилит Unix из командной строки Windows, в этом случае будут перезаписаны некоторые утилиты Windows, например find и sort.

6 Выберете библиотку, которая будет использована при подключении по протоколу HTTPS:
-OpenSSL - сертификаты сервера будут проверяться с использованием Unix-файла ca-bundle.crt.
-Windows Secure Channel - сертификаты сервера будут проверяться с использованием стандартной библиотеки Windows.


7 Убедитесь, что вы выбрали способ обработки окончания строк «Checkout Windows-style, commit Unix-style line endings». Это значение гарантирует, что Git преобразует LF в CRLF при проверке текстовых файлов. При выполнении текстовых файлов CRLF также преобразуется в LF. Это мера совместимости для защиты новых строк в текстовых файлах, что позволяет легко работать с текстовыми файлами в Windows и на платформах Unix.

 
8 Далее необходимо сконфигурировать используемый терминал:
MinTTY - терминал Unix;
Windows - стандартный терминал Windows.

9 Отметьте галочками нужные вам дополнительные функции:

File system caching - кэширование файловой системы.
Git Credential Manager - включить менеджер учетных данных.
Symbolic links - разрешить символьные ссылки.
Нажмите кнопку Install.



Подключение к удаленному репозиторию
Откройте каталог с файлами, которые необходимо отслеживать в системе контроля версий и выложить на GitHub. В пустую часть каталога нажмите правой кнопкой мыши и выберете Git Bash Here.


Перед вами откроется приглашение командной строки в зависимости от настроек.
Для настройки необходимо указать ваше имя и электронную почту:
git config --global user.email "you@example.com"
git config --global user.name "Ваше имя"

Для того чтобы начать отслеживать содержимое папки в системе, выполните команды:
git init
git add

Выполните первый коммит:
git commit -m "Init"

Чтобы добавить изменения, например, на github выполните действие:
git remote add origin https://github.com/пользователь/репозиторий.git
git push -u origin master

Вы можете встроить NeuroStartUp в ваши приложения с помощью следующих сниппетов (кусочков) кода.

JavaScript:

<script src="https://localhost/neuro.sdk.min.js"></script>
Java (Maven):

&lt;dependency&gt;
  &lt;groupId>neuro</groupId&gt;
  &lt;artifactId>sdk</artifactId&gt;
  &lt;version>1.0.0</version&gt;
&lt;dependency&gt;
iOS (добавьте код в ваш Podfile):

platform :ios, '8.0'
pod "neuro-ios-sdk"



