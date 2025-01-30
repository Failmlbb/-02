Глава 1
[311u28@311U28 ~]$ klklklk
bash: klklklk: команда не найдена
[311u28@311U28 ~]$ date
Чт янв 30 10:19:06 +07 2025
311u28@311U28 ~]$ cal
     Январь 2025
Пн Вт Ср Чт Пт Сб Вс
       1  2  3  4  5
 6  7  8  9 10 11 12
13 14 15 16 17 18 19
20 21 22 23 24 25 26
27 28 29 30 31
311u28@311U28 ~]$ df
Файловая система         1K-блоков Использовано   Доступно Использовано% Cмонтировано в
devtmpfs                      4096            0       4096            0% /dev
tmpfs                      7857404        64456    7792948            1% /dev/shm
tmpfs                      3142964         4100    3138864            1% /run
/dev/nvme0n1p5            48281448     26044472   19751932           57% /
/dev/nvme0n1p2              995224       352732     573760           39% /boot
/dev/nvme0n1p6           188018008     97587704   80856096           55% /home
/dev/nvme0n1p1              610120         8028     602092            2% /boot/efi
/dev/sda1                479600448     34004148  421160640            8% /VSD
tmpfs                      1571480          144    1571336            1% /run/user/1804802287
//OPEX1/WinStation.All   976542716    828002740  148539976           85% /media/share/X
//OPEX1/Owners/311/U28 11699159040   2082659736 9616499304           18% /media/share/Z
//OPEX1/SoftWare          62455808     29309788   33146020           47% /media/share/Y
311u28@311U28 ~]$ free
               total        used        free      shared  buff/cache   available
Mem:        15714808     4754184      202148      126388    11226460    10960624
Swap:        7931900       16128     7915772
[311u28@311U28 ~]$ exit
//я обучился командам free ,df,cal,date и если команды нету он их не находит ,
а также если команда хаписана заглавной буквы он её тоже не видет
Глава 2
[311u28@311U28 ~]$ pwd
/home/311u28@nkti.local
 ls
 sync.sh           Видео       Загрузки      Музыка         'Рабочий стол'
'VirtualBox VMs'   Документы   Изображения   Общедоступные   Шаблоны
[311u28@311U28 ~]$ cd/usr/bin
bash: cd/usr/bin: No such file or directory
корневом каталог
[me@linuxbox ~]$ cd /usr/bin
[me@linuxbox bin]$ pwd
/usr/bin
[me@linuxbox ~]$ cd /usr/bin
[me@linuxbox bin]$ pwd
/usr/bin
Отлично, а теперь допустим, что мы хотим сменить рабочий каталог на родительский для каталога /usr/bin, которым является /usr.
cd Сменить рабочий каталог на домашний
cd - Сменить рабочий каталог на предыдущий рабочий каталог
cd ~username Сменить рабочий каталог на домашний каталог пользователя
username. Например, cd ~bob выполнит переход в домашний каталог
пользователя bob
Глава3
[311u28@311U28 ~]$ ls ~ /usr
sync.sh           Видео       Загрузки      Музыка         'Рабочий стол'
'VirtualBox VMs'   Документы   Изображения   Общедоступные   Шаблоны

/usr:
bin    i686-w64-mingw32  lib    libexec  sbin   src  x86_64-w64-mingw32
games  include           lib64  local    share  tmp
[311u28@311U28 ~]$
С ее помощью можно увидеть, что находится в каталоге, и узнать
некоторые важные атрибуты файлов и каталогов
итого 40
-rw-------.  1 311u28 пользователи домена  720 янв 15 12:17  sync.sh
drwxr-xr-x. 10 311u28 пользователи домена 4096 янв 23 15:04 'VirtualBox VMs'
drwxr-xr-x.  2 311u28 пользователи домена 4096 янв 15 12:17  Видео
drwxr-xr-x.  2 311u28 пользователи домена 4096 янв 21 12:04  Документы
drwxr-xr-x.  2 311u28 пользователи домена 4096 янв 29 12:12  Загрузки
drwxr-xr-x.  2 311u28 пользователи домена 4096 янв 15 12:17  Изображения
drwxr-xr-x.  2 311u28 пользователи домена 4096 янв 15 12:17  Музыка
drwxr-xr-x.  2 311u28 пользователи домена 4096 янв 15 12:17  Общедоступные
drwx------.  2 311u28 пользователи домена 4096 янв 30 09:15 'Рабочий стол'
drwxr-xr-x.  2 311u28 пользователи домена 4096 янв 15 12:17  Шаблоны
//Параметр -l, добавленный в команду, требует использования «длинного» (long)
формата вывода.
[311u28@311U28 ~]$  ls -lt
итого 40
drwx------.  2 311u28 пользователи домена 4096 янв 30 09:15 'Рабочий стол'
drwxr-xr-x.  2 311u28 пользователи домена 4096 янв 29 12:12  Загрузки
drwxr-xr-x. 10 311u28 пользователи домена 4096 янв 23 15:04 'VirtualBox VMs'
drwxr-xr-x.  2 311u28 пользователи домена 4096 янв 21 12:04  Документы
drwxr-xr-x.  2 311u28 пользователи домена 4096 янв 15 12:17  Видео
drwxr-xr-x.  2 311u28 пользователи домена 4096 янв 15 12:17  Изображения
drwxr-xr-x.  2 311u28 пользователи домена 4096 янв 15 12:17  Музыка
drwxr-xr-x.  2 311u28 пользователи домена 4096 янв 15 12:17  Общедоступные
drwxr-xr-x.  2 311u28 пользователи домена 4096 янв 15 12:17  Шаблоны
-rw-------.  1 311u28 пользователи домена  720 янв 15 12:17  sync.sh
Добавим параметр с длинным именем --reverse, чтобы изменить порядок сортировки на обратный:
//выводит котологи их изменения
[311u28@311U28 ~]$  ls -lt --reverse
итого 40
-rw-------.  1 311u28 пользователи домена  720 янв 15 12:17  sync.sh
drwxr-xr-x.  2 311u28 пользователи домена 4096 янв 15 12:17  Шаблоны
drwxr-xr-x.  2 311u28 пользователи домена 4096 янв 15 12:17  Общедоступные
drwxr-xr-x.  2 311u28 пользователи домена 4096 янв 15 12:17  Музыка
drwxr-xr-x.  2 311u28 пользователи домена 4096 янв 15 12:17  Изображения
drwxr-xr-x.  2 311u28 пользователи домена 4096 янв 15 12:17  Видео
drwxr-xr-x.  2 311u28 пользователи домена 4096 янв 21 12:04  Документы
drwxr-xr-x. 10 311u28 пользователи домена 4096 янв 23 15:04 'VirtualBox VMs'
drwxr-xr-x.  2 311u28 пользователи домена 4096 янв 29 12:12  Загрузки
drwx------.  2 311u28 пользователи домена 4096 янв 30 09:15 'Рабочий стол'
//выводит котологи их изменения в их обратном порядккеды
ls -a
 .                      .cache          .pki              Загрузки
 ..                     .config         sync.sh           Изображения
 .bash_history          .dbus           .themes           Музыка
 .bash_logout           .gphoto        'VirtualBox VMs'   Общедоступные
 .bash_profile          .ICEauthority   .wine            'Рабочий стол'
 .bash_profile.rpmnew   .icons          .yandex           Шаблоны
 .bashrc                .lab1.txt.swp   Видео
 .bashrc.rpmnew         .local          Документы
//Список всех (all) файлов, даже с именами, начинающимися с точки, которые обычно не выводятся
(то есть скрытых)
311u28@311U28 ~]$ ls -A
 .bash_history          .config         .pki              Документы
 .bash_logout           .dbus           sync.sh           Загрузки
 .bash_profile          .gphoto         .themes           Изображения
 .bash_profile.rpmnew   .ICEauthority  'VirtualBox VMs'   Музыка
 .bashrc                .icons          .wine             Общедоступные
 .bashrc.rpmnew         .lab1.txt.swp   .yandex          'Рабочий стол'
 .cache                 .local          Видео             Шаблоны
Действует подобно параметру -a, но не выводит
каталоги . (текущий рабочий каталог) и .. (родительский каталог)
[311u28@311U28 ~]$ ls -f
 Документы              .bash_profile   .local          .
 .themes                Видео           .config        'Рабочий стол'
 .pki                   sync.sh         Общедоступные  'VirtualBox VMs'
 .wine                  .yandex         Музыка          .lab1.txt.swp
 .bash_profile.rpmnew   Загрузки        .bash_logout    .bashrc.rpmnew
 ..                     Изображения     .bash_history   .icons
 .dbus                  .ICEauthority   .cache
 .bashrc                .gphoto         Шаблоны
Добавляет в конец каждого имени символ-индикатор
(например, прямой слеш, если это имя каталога)
[311u28@311U28 ~]$ ls -l
итого 40
-rw-------.  1 311u28 пользователи домена  720 янв 15 12:17  sync.sh
drwxr-xr-x. 10 311u28 пользователи домена 4096 янв 23 15:04 'VirtualBox VMs'
drwxr-xr-x.  2 311u28 пользователи домена 4096 янв 15 12:17  Видео
drwxr-xr-x.  2 311u28 пользователи домена 4096 янв 21 12:04  Документы
drwxr-xr-x.  2 311u28 пользователи домена 4096 янв 29 12:12  Загрузки
drwxr-xr-x.  2 311u28 пользователи домена 4096 янв 15 12:17  Изображения
drwxr-xr-x.  2 311u28 пользователи домена 4096 янв 15 12:17  Музыка
drwxr-xr-x.  2 311u28 пользователи домена 4096 янв 15 12:17  Общедоступные
drwx------.  2 311u28 пользователи домена 4096 янв 30 09:15 'Рабочий стол'
drwxr-xr-x.  2 311u28 пользователи домена 4096 янв 15 12:17  Шаблоны
//Выводит формата
[311u28@311U28 ~]$ ls -s
итого 40
4  sync.sh          4  Документы    4  Музыка         4  Шаблоны
4 'VirtualBox VMs'  4  Загрузки     4  Общедоступные
4  Видео            4  Изображения  4 'Рабочий стол'
//Сортировать результаты по размеру (size)
[311u28@311U28 ~]$ ls -t
'Рабочий стол'  'VirtualBox VMs'   Видео         Музыка          Шаблоны
 Загрузки        Документы         Изображения   Общедоступные
//Сортировать результаты по времени (time) последнего изменения
[311u28@311U28 ~]$ ls -1
sync.sh
'VirtualBox VMs'
Видео
Документы
Загрузки
Изображения
Музыка
Общедоступные
'Рабочий стол'
Шаблоны
//Число жестких ссылок на файл. Подробнее о ссылках рассказывается в разделах «Символические ссылки» и «Жесткие ссылки» далее
в этой главе
[311u28@311U28 ~]$ ls -root
итого 40
-rw-------.  1 311u28  720 янв 15 12:17  sync.sh
drwxr-xr-x.  2 311u28 4096 янв 15 12:17  Шаблоны
drwxr-xr-x.  2 311u28 4096 янв 15 12:17  Общедоступные
drwxr-xr-x.  2 311u28 4096 янв 15 12:17  Музыка
drwxr-xr-x.  2 311u28 4096 янв 15 12:17  Изображения
drwxr-xr-x.  2 311u28 4096 янв 15 12:17  Видео
drwxr-xr-x.  2 311u28 4096 янв 21 12:04  Документы
drwxr-xr-x. 10 311u28 4096 янв 23 15:04 'VirtualBox VMs'
drwxr-xr-x.  2 311u28 4096 янв 29 12:12  Загрузки
drwx------.  2 311u28 4096 янв 30 09:15 'Рабочий стол'
//Имя группы/лица владеющей файлом
[311u28@311U28 ~]$ ls -32059
ls: invalid option -- '3'
По команде «ls --help» можно получить дополнительную информацию.
[311u28@311U28 ~]$ ls -oo-cd-cover.odf
ls: invalid option -- '-'
//Имя файла
Глава 4
https://prepod.nspu.ru/pluginfile.php/379121/mod_resource/content/1/Шоттс%20У.%20-%20Командная%20строка%20Linux.%20Полное%20руководство.%202-е%20межд.%20изд.%20%28Для%20профессионалов%29%20-%202020.pdf





