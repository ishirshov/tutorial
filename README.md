# Что необходимо для использования?

* QEMU i386    >= 4.9.0
* NASM         == 2.14.02
* Make         == 4.2.1
* GDB          == 8.1 (с TUI поддержкой)

# Возможности

* GDB в режиме TUI
* Запуск отладки из Visual Studio с использованием GDBServer

# Как использовать?

Проект использует образ системы сборки buildroot_x86, который можно запустить используя QEMU утилиту qemu-system-i386.

## GDB в режиме TUI

Корневой каталог содержит bash-скрипт для запуска среды исполнения - <em>start-qemu.sh.</em> Среда исполнения позволит использовать TUI режим для отладки исполняемых файлов.

После сборки (единоразовой) будет доступна shell оболочка. В проекте используется автоматизация сборки Makefile, поэтому достаточно запустить команду make.

В каталоге bin будут находиться исполняемые файлы примеров из лекций курса. Запуск в TUI режиме: <em>gdb -x bin/example.gdb.</em>

