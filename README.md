# Termux

Сайт termux.dev является официальным ресурсом для проекта Termux — мощного эмулятора терминала и среды Linux для Android. Он предоставляет подробную информацию о функциональности, возможностях настройки и использования Termux, а также служит основным источником для загрузки и поддержки приложения.

⚠️ Важное замечание
С версии Termux 0.101 приложение больше не обновляется в Google Play Store. Это связано с изменениями в политике Google, которые ограничивают выполнение бинарных файлов в приватных директориях приложений. Разработчики рекомендуют устанавливать Termux через F-Droid или загружать APK-файлы с официального репозитория на GitHub.​

🔧 Основные возможности Termux
Минимальная установка Linux: Termux предоставляет базовую систему Linux без необходимости root-доступа.
Управление пакетами через APT: Установка и обновление программного обеспечения с использованием пакетного менеджера APT, аналогичного Debian и Ubuntu.
Поддержка различных оболочек: Выбор между Bash, fish или Zsh для командной строки.
Разнообразие редакторов: Возможность использовать редакторы nano, Emacs или Vim.
Доступ к удалённым серверам: Использование SSH-клиента OpenSSH для подключения к удалённым системам.
Поддержка языков программирования: Установка и использование актуальных версий Perl, Python, Ruby и Node.js.
Разработка и отладка: Компиляция программ на Go, Rust, Swift или C с использованием Clang и инструментов CMake, а также отладка с помощью lldb/GDB и strace


## Download

[Termux](https://termux.dev/)
[github](https://github.com/termux/termux-app)
[play.google](https://play.google.com/store/apps/details?id=com.termux)
[f-droid](https://f-droid.org/packages/com.termux/)


```
pwd
pkg i git gh

git -v
gh --version

alias updg = "apt update && apt upgrade"

help
pkg help

clear
pkg list-all
pkg list-install
pkg show git
```

```
pkg install
pkg uninstall
pkg reinstall
```



---



📦 Управление пакетами

Обновление списка пакетов:
```bash
pkg update
apt update
```

Обновление установленных пакетов:
```bash
pkg upgrade
apt upgrade
```

Установка пакета:
```bash
pkg install <имя_пакета>
apt install <имя_пакета>
```

Удаление пакета:
```bash
pkg uninstall <имя_пакета>
apt remove <имя_пакета>
```

Поиск пакета:
```bash
pkg search <название>
```

Список установленных пакетов:
```bash
pkg list-installed
```

Информация о пакете:
```bash
pkg info <имя_пакета>
```

📁 Работа с файлами и каталогами

Переход в каталог:
```bash
cd /путь/к/каталогу
```

Список файлов:
```bash
ls -la
```

Создание файла:
```bash
touch <имя_файла>
```

Создание каталога:
```bash
mkdir <имя_каталога>
```

Удаление файла:
```bash
rm <имя_файла>
```

Удаление каталога:
```bash
rm -r <имя_каталога>
```

Копирование файла:
```bash
cp <источник> <назначение>
```

Перемещение/переименование файла:
```bash
mv <старое_имя> <новое_имя>
```

🧰 Системные утилиты

Проверка использования памяти:
```bash
free -h
```

Проверка свободного места на диске:
```bash
df -h
```

Информация о системе:
```bash
uname -a
```

Список процессов:
```bash
ps aux
top
```

Завершение процесса:
```bash
kill <PID>
killall <имя_процесса>
```

Управление фоновыми задачами:
```bash
bg <job_id>
fg <job_id>
jobs
```

🌐 Сетевые команды

Проверка подключения:
```bash
ping <адрес>
```

Информация о сетевых интерфейсах:
```bash
ifconfig
```

Скачивание файла:
```bash
wget <URL>
curl -O <URL>
```

Подключение по SSH:
```bash
ssh <пользователь>@<хост>
```

Сканирование сети с использованием Nmap:
```bash
nmap <цель>
```

💻 Разработка и скрипты

Запуск Python-скрипта:
```bash
python <скрипт.py>
```

Запуск Bash-скрипта:
```bash
bash <скрипт.sh>
```

Компиляция C-кода:
```bash
clang <файл.c> -o <выходной_файл>
```

Установка Git:
```bash
pkg install git
```

Клонирование репозитория:
```bash
git clone <URL_репозитория>
```

📱 Команды Termux API

Получение состояния батареи:
```bash
termux-battery-status
```

Получение текущего местоположения:
```bash
termux-location
```

Вибрация устройства:
```bash
termux-vibrate
```

Сканирование Wi-Fi сетей:
```bash
termux-wifi-scaninfo
```

Сделать фото с камеры:
```bash
termux-camera-photo <путь_к_файлу>
```

Отправка SMS:
```bash
termux-telephony-sms-send <номер> "<сообщение>"
```

🛠️ Утилиты и инструменты
Установка Nmap:
```bash
pkg install nmap
```

Установка Metasploit:
```bash
pkg install wget curl openssh git
git clone https://github.com/OnlineHacKing/Metasploit_Termux
cd Metasploit_Termux
chmod +x metasploit.sh
./metasploit.sh
```

Установка Aircrack-ng:
```bash
pkg install aircrack-ng
Для более подробного и структурированного справочника по командам Termux вы можете ознакомиться с Termux Command Handbook 
```
