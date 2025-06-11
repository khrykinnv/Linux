# Editing Files

Linux, как и другие операционные системы, позволяет редактировать файлы для различных целей, будь то настройка некоторых системных функций или написание скриптов.
В Linux по умолчанию доступно множество текстовых редакторов, в том числе: nano, vi/vim, emacs, и gedit. Каждый из них имеет свою собственную кривую обучения и набор команд.

Например, nano— это базовый текстовый редактор, который прост в использовании и идеально подходит для простого редактирования текстовых файлов.
Vi/vimС другой стороны, он более продвинут и предлагает широкий спектр функций и команд.

Чтобы отредактировать файл, сначала его нужно открыть с помощью команды типа:

```nano [filename]```

```vi [filename] or vim [filename]```

```gedit [filename]```

https://www.scaler.com/topics/how-to-edit-a-file-in-linux/

## Vim: 
![Image_vim](images/vim.png)



### VimTutor
https://i-notes.org/vimtutor-uchebnik-vim-versiya-1-7/

https://rigovanov.ru/vim/

i - режим вставки текста

Esc - режим ввода команд 

/ - поиск

:q! - выход без сохранения (:wq - сохранить и выйти)


## Nano
### Подсветка синтаксиса
На удаленных серверах для правки конфигов можно использовать nano – быстрый, понятный, простой текстовый редактор, с подсведкой синтаксиса. Согласитесь, это очень удобно :-)

1. Найдем, где в нашей системе находятся примеры файлов .nanorc. На Ubuntu они обычно в каталоге /usr/share/nano/. Скопируем к себе в каталог, файл конфигурации:

``$ cp /etc/nanorc ~/.nanorc ``



2. Добавим строчки в файл ~/.nanorc (на Ubuntu примеры конфигурации идут в поставке) для подсветки необходимых нам файлов, если они отсутствуют в стандартном файле конфигурации:

#### TeX
include "/usr/share/nano/patch.nanorc"
#### POV-Ray
include "/usr/share/nano/pov.nanorc"
#### Perl
include "/usr/share/nano/perl.nanorc"
#### Nanorc files
include "/usr/share/nano/nanorc.nanorc"
#### Python
include "/usr/share/nano/python.nanorc"
#### C/C++
include "/usr/share/nano/c.nanorc"
#### Groff
include "/usr/share/nano/groff.nanorc"
#### Assembler
include "/usr/share/nano/asm.nanorc"
#### Ruby
include "/usr/share/nano/ruby.nanorc"
#### Manpages
include "/usr/share/nano/man.nanorc"
#### HTML
include "/usr/share/nano/html.nanorc"
#### Bourne shell scripts
include "/usr/share/nano/sh.nanorc"
#### Sun Java
include "/usr/share/nano/java.nanorc"

### Как отобразить нумерацию строк в nano при открытии файла
``sudo nano /etc/nanorc``

``linenumbers yes``

https://mascloud.ru/kratkaya-shpargalka-po-sochetaniyam-klavish-nano/


