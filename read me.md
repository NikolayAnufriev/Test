# Синтаксис языка Markdown.
---
- Жирный текст — **
- Курсивный текст — *
- Зачеркнутый текст — ~
- Выделяют заголовки — # в начале строки
- Показать уровень заголовка — подчеркивание знаками = или -
- Нумерованные Списки — обозначаются обычными цифрами 1, 2, 3 
- Ненумерованные Списки — обозначаются знаками * в начале строки
- Вложенные Списки — выполняем отступы
>## *Использование синтаксиса Markdown*    
### **Текст** 
 - Чтобы выделить текст ***курсивом*** необходимо обрамить его звездочками (*) или  знаком нижнего подчеркивания (_). Например *вот так* или _вот так_. 

  - Чтобы выделить текст **полужирным** необходимо обрамить его двойными звездочками (**) или двойным знаком нижнего подчеркивания (__). Например **вот так** или __вот так__

    - Альтернативные способы выделения текста жирным или курсивом нужны для того, что бы мы могли совмещать оба этих способа. Например, _текст может быть выделен курсивом и при этом быть **полужирным**_
### **Список**
- Чтобы добавить ненумерованные списки, необходимо пункты выделить звездочкой (*) или знаком +. 
Например, вот так: 
  * Элемент 1
  * Элемент 2
  * Элемент 3
  + Элемент 4

- Чтобы добавить нумерованные списки, необходимо пункты просто пронумировать. Например, вот так:
  1. Первый пункт
  2. Второй пункт

# Команды Git
---
 - **git --version** 
 
 >Если Git установлен на компьютер, вы увидите его текущую версию.
 -  **git init**   
 
 >Инициализация: указываем папку, в которой Git начнёт отслеживать изменения.
 В папке создаётся скрытая папка **.git**   
 [Важно!][init]
 - **git status**

 >Показывает текущее состояние Git'а, есть ли изменения, которые нужно закоммитить
 (сохранить)
 - **git add**
 
 >Добавляет содержимое рабочего каталога в индекс (staging area) для последующего коммита. Эта команда дается после добавления файлов. Писать название целиком не обязательно: терминал дозаполнит данные автоматически.  
 [Важно!][add]
 - **git commit**

 >Зафиксировать или сохранить. По умолчанию **_git commit_** использует лишь этот индекс, так что вы можете использовать **_git add_** для сборки слепка вашего следующего коммита. Команда **_git commit_** берёт все данные, добавленные в индекс с помощью **_git add_**, и сохраняет их слепок во внутренней базе данных, а затем сдвигает указатель текущей ветки на этот слепок.  
 [Важно!][commit]
 - **git diff** 

 >Показывает разницу между текущим файлом и сохранённым. Перед переключением >версии файла в Git используйте команду **_git log_**, чтобы увидеть количество сохранений.    
 [Важно!][diff]
 - **git log** 

 >Журнал изменений. Перед переключением версии файла в Git используйте команду **_git log_**, чтобы увидеть количество сохранений.    
 [Важно!][log] 
 - **git branch**
 
 >Если у нас несколько версий черновика, мы можем вывести на экран ветку, где находимся, командой **_git branch_**.  
  [Важно!][branch] 
 - **git branch _new_branch_name_**

 >Данная команда предназначена для создания новой ветки. Например, **_git branch_** Название_новой_ветки.   
 [Важно!][branch new]
 -  **git checkout**

 >Если потребуется переключиться с одной ветки на другую, вызовем команду **_git checkout_** <имя ветки>  
  [Важно!][checkout] 
  - **git log -graph**

  >Ключ **_-graph_** в связке с командой **_log_** позволяет отобразить коммиты в виде дерева.   
  [Важно!][log graph]

 - **git merge** 

 >Чтобы слить любую ветку с текущей, вызываем **_git merge_** <имя ветки для слияния с текущей>   
 [Важно!][merge]
- **git ignore**

>В Git не принято добавлять файлы изображений, их хранят на сторонних носителях. Чтобы исключить ненужные файлы из загрузки, есть команда **_git ignore_**.
- **git clone**

>Эта команда позволяет склонировать внешний репозиторий на наш ПК.   
[Важно!][clone]
- **git pull**

>Эта команда позволяет скачать все из текущего репозитория и автоматически
сделать merge с нашей версией   
[Важно!][pull]
- **git push**

>Эта команда позволяет отправить нашу версию репозитория на внешний репозиторий. Процедура ТРЕБУЕТ АВТОРИЗАЦИИ на внешнем репозитории.  
[Важно!][push]


# Работа с удаленными репозитариями
---

## Чтобы работать с удаленными репозитариями нам необходимо выполнить следующие действия:

 1. Делаем форк (fork) интересующего нас репозитория. 
 2. При помощи команды **git clone** делаем копию репозитория.
 3. Создаем новую ветку командой **git branch** название_новой_ветки
 4. Производим все изменения только в новой ветке.
 5. Командой **git push** отправляем эти изменения в свой акквунт на *Github*
 6. Далее на *Github* кнопкой **_pull request_** отправляем изменения автору репозитория.



[init]: ../../../../../../C:/Users/%D0%9D%D0%B8%D0%BA%D0%BE%D0%BB%D0%B0/Desktop/%D0%9E%D0%B1%D1%83%D1%87%D0%B5%D0%BD%D0%B8%D0%B5/git/Pictures/git%20init.PNG
[add]: ../../../../../../C:/Users/%D0%9D%D0%B8%D0%BA%D0%BE%D0%BB%D0%B0/Desktop/%D0%9E%D0%B1%D1%83%D1%87%D0%B5%D0%BD%D0%B8%D0%B5/git/Pictures/Git%20add.png
[commit]: ../../../../../../C:/Users/%D0%9D%D0%B8%D0%BA%D0%BE%D0%BB%D0%B0/Desktop/%D0%9E%D0%B1%D1%83%D1%87%D0%B5%D0%BD%D0%B8%D0%B5/git/Pictures/git%20commit.png
[diff]: ../../../../../../C:/Users/%D0%9D%D0%B8%D0%BA%D0%BE%D0%BB%D0%B0/Desktop/%D0%9E%D0%B1%D1%83%D1%87%D0%B5%D0%BD%D0%B8%D0%B5/git/Pictures/git%20diff.png
[log]: ../../../../../../C:/Users/%D0%9D%D0%B8%D0%BA%D0%BE%D0%BB%D0%B0/Desktop/%D0%9E%D0%B1%D1%83%D1%87%D0%B5%D0%BD%D0%B8%D0%B5/git/Pictures/git%20log.png
[branch]: ../../../../../../C:/Users/%D0%9D%D0%B8%D0%BA%D0%BE%D0%BB%D0%B0/Desktop/%D0%9E%D0%B1%D1%83%D1%87%D0%B5%D0%BD%D0%B8%D0%B5/git/Pictures/git%20branch.png
[branch new]: ../../../../../../C:/Users/%D0%9D%D0%B8%D0%BA%D0%BE%D0%BB%D0%B0/Desktop/%D0%9E%D0%B1%D1%83%D1%87%D0%B5%D0%BD%D0%B8%D0%B5/git/Pictures/git%20branch%20new.png
[checkout]: ../../../../../../C:/Users/%D0%9D%D0%B8%D0%BA%D0%BE%D0%BB%D0%B0/Desktop/%D0%9E%D0%B1%D1%83%D1%87%D0%B5%D0%BD%D0%B8%D0%B5/git/Pictures/git%20checkout.png
[log graph]: ../../../../../../C:/Users/%D0%9D%D0%B8%D0%BA%D0%BE%D0%BB%D0%B0/Desktop/%D0%9E%D0%B1%D1%83%D1%87%D0%B5%D0%BD%D0%B8%D0%B5/git/Pictures/git%20log%20graph.png
[merge]: ../../../../../../C:/Users/%D0%9D%D0%B8%D0%BA%D0%BE%D0%BB%D0%B0/Desktop/%D0%9E%D0%B1%D1%83%D1%87%D0%B5%D0%BD%D0%B8%D0%B5/git/Pictures/git%20merge.png
[clone]: ../../../../../../C:/Users/%D0%9D%D0%B8%D0%BA%D0%BE%D0%BB%D0%B0/Desktop/%D0%9E%D0%B1%D1%83%D1%87%D0%B5%D0%BD%D0%B8%D0%B5/git/Pictures/git%20clone.png
[pull]: ../../../../../../C:/Users/%D0%9D%D0%B8%D0%BA%D0%BE%D0%BB%D0%B0/Desktop/%D0%9E%D0%B1%D1%83%D1%87%D0%B5%D0%BD%D0%B8%D0%B5/git/Pictures/git%20pull.png
[push]: ../../../../../../C:/Users/%D0%9D%D0%B8%D0%BA%D0%BE%D0%BB%D0%B0/Desktop/%D0%9E%D0%B1%D1%83%D1%87%D0%B5%D0%BD%D0%B8%D0%B5/git/Pictures/git%20push.png