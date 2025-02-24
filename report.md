## Part 1. Установка ОС
![linux](images/task1.jpg)

## Part 2. Создание пользователя
![linux](images/task2.2.jpg)

![linux](images/task2.3.jpg)

## Part 3. Настройка сети ОС
1) ![linux](images/task3.1.jpg)

   ![linux](images/task3.2.jpg)
2) ![linux](images/task3.3.jpg)

3) ![linux](images/task3.4.jpg)

lo - loopback, внутренний интерфейс, который используется для коммуникации на самом сервере. обычно используется для тестирования сетевых приложений.
4) ![linux](images/task3.5.jpg)

Адресс - 10.0.2.15/24

DHCP - протокол динамаческой конфигурации хоста. Это сетевой протокол, который автоматически назначает IP-адреса и другие сетевые параметры устройствам в сети.

5) ![linux](images/task3.6.2.jpg)

   ![linux](images/task3.6.jpg)

6) ![linux](images/task3.7.1.jpg)
   
7) ![linux](images/task3.7.3.jpg)

   ![linux](images/task3.7.4.jpg)

## Part 4. Обновление ОС
![linux](images/task4.jpg)

![linux](images/task4.1.jpg)

## Part 5. Использование команды sudo
![linux](images/task5.jpg)

Назначение команды sudo заключается в предоставлении пользователям временных привилегий администратора для выполнения определенных задач или команд, которые обычно доступны только суперпользователю (root).

## Part 6. Установка и настройка службы времени
![linux](images/realtask6.jpg)

## Part 7. Установка и использование текстовых редакторов
![linux](images/task_7_vim.jpg)

![linux](images/task_7_nano.jpg)

![linux](images/task_7_mcedit.jpg)

Vim - Shift + ZZ

Nano - Ctrl + O, Enter, Ctrl + X

Mcedit - F2, F10


![linux](images/task_7_vim2.jpg)

![linux](images/task_7_nano2.jpg)

![linux](images/task_7_mcedit2.jpg)

Vim - :q!

Nano - Ctrl + X, выбрать N

Mcedit - F10, выбрать No


![linux](images/task_7_vim3.1.jpg)

![linux](images/task_7_vim3.2.jpg)

![linux](images/task_7_nano3.1.jpg)

![linux](images/task_7_nano3.2.jpg)

![linux](images/task_7_mcedit3.1.jpg)

![linux](images/task_7_mcedit3.2.jpg)

Меняем Nutshell на Jar.

Vim - Поиск /Nutshell | Замена :%s/Nutshell/Jar/g

Nano - Поиск Ctrl + W, ввести Nutshell | Замена Alt + R, ввести Nutshell и Jar

Mcedit - Поиск F7, ввести Nutshell | Замена F4, ввести Nutshell и Jar

## Part 8. Установка и базовая настройка сервиса SSHD
![linux](images/task_8.jpg)

![linux](images/task_8.2.jpg)

![linux](images/task_8.3.1.jpg)

![linux](images/task_8.3.2.jpg)

![linux](images/task_8.4.jpg)

Кючи команды ps: -e отображает процессы для всех пользователей, -f выводит полную информацию о каждом процессе.

![linux](images/task_8.5.jpg)

-tan -комбинация ключей, где -t отображает только TCP-порты, -a отображает все соединения и прослушивающие порты, а -n показывает порты в 
числовом формате, а не их имена.

tcp: Это протокол, к которому относится соединение, является одним из основных протоколов передачи данных в Интернете.

0: Это номер ID соединения.

0: Это номер ID устройства.

0.0.0.0:2022: Это адрес и порт, на котором служба прослушивает входящие соединения. 0.0.0.0 означает "любой адрес" или "любой интерфейс". Поэтому служба прослушивает все доступные сетевые интерфейсы на порту 2022.

0.0.0.0:*: Это адрес и порт, на который служба связана. Снова 0.0.0.0 означает "любой адрес", а * означает "любой порт". Это означает, что служба связана с любым доступным портом на всех интерфейсах.

LISTEN: Это состояние порта. В данном случае LISTEN указывает на то, что служба активно прослушивает указанный порт и готова принимать новые соединения.

## Part 9. Установка и использование утилит top, htop
![linux](images/task_9.jpg)

- top:
 - uptime - 3 min
  - количество авторизованных пользователей - 1 user
  - общую загрузку системы - 0.01, 0.02, 0.00 за 1, 5, 15 минут соответсвенно
  - общее количество процессов - 80
  - загрузку cpu - 0, 0, 0, 100, 0, 0, 0, 0 в разных категориях
  - загрузку памяти - 1971.6 Mib Total
  - pid процесса занимающего больше всего памяти - 1
  - pid процесса, занимающего больше всего процессорного времени - 1


- htop:

![linux](images/task_9.1.jpg)

![linux](images/task_9.2.jpg)

![linux](images/task_9.3.jpg)

![linux](images/task_9.4.jpg)

![linux](images/task_9.5.jpg)

![linux](images/task_9.6.jpg)

![linux](images/task_9.7.jpg)

## Part 10. Использование утилиты fdisk
![linux](images/task_10.jpg)

- Название жесткого диска - /dev/sda
- Размер - 12 GiB
- Колличество секторов - 25165824
- Размер swap - 512 MB

## Part 11. Использование утилиты df

- df /:
  - размер раздела - 12G
  - размер занятого пространства - 3.3G
  - размер свободного пространства - 7.5G
  - процент использования - 31%
- единицей измерения в выводе команды df является гигабайт

- df -Th /:
    - размер раздела - 12G
    - размер занятого пространства - 3.3G
    - размер свободного пространства - 7.5G
    - процент использования - 31%
- корневой раздел использует файловую систему ext4

## Part 12. Использование утилиты du
![linux](images/task_12_1.jpg)

![linux](images/task_12_2.jpg)

![linux](images/task_12_3.jpg)

![linux](images/task_12_4.jpg)

![linux](images/task_12_5.jpg)

## Part 13. Установка и использование утилиты **ncdu**
![linux](images/task_13_1.jpg)

![linux](images/task_13_2.jpg)

![linux](images/task_13_3.jpg)

## Part 14. Работа с системными журналами
![linux](images/task_14_1.jpg)

- Apr 23 16:51:08
- gastonar
- by LOGIN

![linux](images/task_14_2.jpg)

## Part 15. Использование планировщика заданий **CRON**
![linux](images/task_15.jpg)

![linux](images/task_15_2.jpg)

![linux](images/task_15_3.jpg)