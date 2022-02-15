**** Гриднев Алексей МК-401 ЛР-1
1) Основные принципы Unix-way  
	* Одна задача - одна программа  
	* Есть множество путей решения  
	* Все есть файл

2) Линус Торвальдс является разработчиком чего  
	Ядра ОС Linux, системы управления версиями Git 

3) Как посмотреть  название ядра системы из консоли?   
	`uname -r`

4) Промежутки измерения загрузки системы для команды uptime следующие  
	1,5,15 минут

5) какой командой узнать сколько занято на HDD  
	`df -H`

6) какие разделы содержит вывод команды vmstat
	* procs (количество процессов)
	* memory (память)
	* swap (файл подкачки)
	* io (загрузка ввода-вывода)
	* cpu (загрузка процессора)

7) Описать работу своего Linux дистрибутива: какое ядро, архитектура, размеры hdd, объеме ОЗУ, загрузке процессора и т.д
 * Ядро, архитектура:  
    ```
    alexey@ubuntu:~$ uname -ar
    Linux ubuntu 5.13.0-27-generic #29~20.04.1-Ubuntu SMP Fri Jan 14 00:32:30 UTC 2022 x86_64 x86_64 x86_64 GNU/Linux
    ```
     * Информация HDD:  
     ```
     alexey@ubuntu:~$ df -H
      Filesystem      Size  Used Avail Use% Mounted on
      udev            2.1G     0  2.1G   0% /dev
      tmpfs           409M  2.1M  407M   1% /run
      /dev/sda5        21G   15G  5.0G  75% /
      tmpfs           2.1G   29k  2.1G   1% /dev/shm
      tmpfs           5.3M  4.1k  5.3M   1% /run/lock
      tmpfs           2.1G     0  2.1G   0% /sys/fs/cgroup
      /dev/loop0      132k  132k     0 100% /snap/bare/5
      /dev/loop1      230M  230M     0 100% /snap/gnome-3-34-1804/72
      /dev/loop2       69M   69M     0 100% /snap/gtk-common-themes/1519
      /dev/loop3       59M   59M     0 100% /snap/core18/2253
      /dev/loop4      261M  261M     0 100% /snap/gnome-3-38-2004/87
      /dev/loop5       54M   54M     0 100% /snap/snap-store/547
      /dev/loop6       69M   69M     0 100% /snap/gtk-common-themes/1515
      /dev/loop7       59M   59M     0 100% /snap/core18/2284
      /dev/loop8       66M   66M     0 100% /snap/core20/1328
      /dev/loop9       66M   66M     0 100% /snap/core20/1270
      /dev/loop10      57M   57M     0 100% /snap/snap-store/558
      /dev/loop11      46M   46M     0 100% /snap/snapd/14295
      /dev/loop12     230M  230M     0 100% /snap/gnome-3-34-1804/77
      /dev/loop13      46M   46M     0 100% /snap/snapd/14549
      /dev/sda1       536M  4.1k  536M   1% /boot/efi
      tmpfs           409M   33k  409M   1% /run/user/1000
    ```
     * Информация ОЗУ:  
     ```
     alexey@ubuntu:~$ free -h
               	      total        used        free      shared  buff/cache   available
  	Mem:          3.8Gi       1.3Gi       1.2Gi        15Mi       1.3Gi       2.2Gi
  	Swap:         923Mi          0B       923Mi
     ```
     * Загрузка процессора:  
     ```
     alexey@ubuntu:~$ uptime
      04:33:36 up 3 min,  1 user,  load average: 0.40, 0.79, 0.39
     ```
       
