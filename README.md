# git-cheat-sheet


### INFO
``` git status ```  
``` git branch ```  
``` git log ```  
``` git help ```  


### PULL/PUSH
``` git add . ```  
``` git commit -m "Fix test.txt" ```  
``` git pull origin master ```  
``` git push origin master ```  


### CHECKOUT
``` git checkout [наименование ветки | хэш коммита] ```  
``` git checkout -b new_branch ```  

``` git checkout -- . ```  
В текущей директории будут отменены все локальные изменения, хранящиеся в репозитории, но не затрагивает индекс (изменения git add)

``` git checkout [хэш коммита] -- [путь к файлу] ```  
Такая команда поместит нужный файл в рабочую директорию. Рекомендуется использовать > git diff вместе с > git checkout, чтобы посмотреть изменения в файлах, прежде чем их отменить. Также помогает команда > git status, обнаруживающая новые изменения.


### CONFIG
``` git config --global --list ```  
``` git config --global user.name [nickname] ```  
``` git config --global --list ```  
``` git config --global user.email "[email]" ```  
``` git config --global --list ```  


### MERGE
``` git merge dev ```  
``` git push origin master ```  


### RESET
``` git reset --hard ```  
Полный сброс состояния репозитория (перемещает указатель HEAD на указанный коммит, обновляет индекс и рабочую директорию до состояния этого коммита)

``` git reset --hard [хэш коммита] ```  
``` git push --force origin main ```  
Когда нужно откатиться к нужному коммиту
