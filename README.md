# bash
## 1.	Создал учетную запись на ресурсе github.com.
## 2.	Создал на ресурсе github.com репозиторий для выполнения практической работы. 
## 3.	Создал папку для работы с Git.
## 4.	Создал локальный репозиторий в текущей папке.
### •	git init
## 5.	Добавил туда пустой текстовый документ.
### •	echo. > Text.txt
## 6.	Создал commit для каждого абзаца, не менее 5 абзацев.
### •	echo Первый >> Text.txt
### •	git add Text.txt
### •	git commit -m "Первый"
![image](https://github.com/Fader77/bash/assets/137108770/f6954833-fd05-4b3d-ab95-214b611c5e04)
## 7.	Посмотрел статус текущего репозитория. 
### •	git status
![image](https://github.com/Fader77/bash/assets/137108770/958bd475-95cd-48ac-96bc-600699090a67)
## 8.	Добавил файл. 
### •	echo. > Еще один.txt
![image](https://github.com/Fader77/bash/assets/137108770/b64ae56d-cf3b-4b18-8ab7-28dcba1967bf)
## 9.	Создал коммит, указал для него комментарий.
### •	git commit -m "еще один документ"
![image](https://github.com/Fader77/bash/assets/137108770/2beae35a-6922-429a-b9ff-3b2f58bfc687)
## 10.	Посмотрел протокол коммитов. 
### •	git log
![image](https://github.com/Fader77/bash/assets/137108770/89b0ddd3-b92b-4a98-aa2d-f54705cf473a)
## 11.	Посмотрел изменения в файле по сравнению с последним коммитом.
### •	git diff
![image](https://github.com/Fader77/bash/assets/137108770/a4215709-8d9e-4485-b00b-2f8ebd42fe25)
## 12.	Убрал изменения относительно последнего коммита из файла.
### •	git restore Еще.txt
![image](https://github.com/Fader77/bash/assets/137108770/59c64103-8d69-4334-9ecd-77b0df81dd68)
## 13.	Просмотрел существующие ветки.
### •	git branch
![image](https://github.com/Fader77/bash/assets/137108770/ba1ba275-c292-432d-9d56-d63ac8c3778e)
## 14.	Создал новую ветку. 
### •	git branch mainNo2
![image](https://github.com/Fader77/bash/assets/137108770/66de8650-17c1-4f7d-bccf-906fecb3b8f1)
## 15.	Переключил на другую ветку. 
### •	git checkout mainNo2
![image](https://github.com/Fader77/bash/assets/137108770/173cb748-5c65-417d-959d-6553f8b8aae2)
## 16.	Создал новую ветку и сразу же переключился на нее. 
### •	git checkout -b mainNo3
![image](https://github.com/Fader77/bash/assets/137108770/e87a73e4-467a-4cba-9cd6-794b4e274396)
## 17.	Удалил ветку. 
### •	git branch -d mainNo2
![image](https://github.com/Fader77/bash/assets/137108770/b31e538e-f482-45fb-b735-dee22377193d)
## 18.	Добавил (merge) изменения из указанной ветки в текущую.
### •	git merge main
![image](https://github.com/Fader77/bash/assets/137108770/cf5273f5-d618-4d24-92ae-24f87e2ba119)
## 19.	Создал конфликт.
### •	Переключился на ветку main
### git checkout main
### •	Добавляем коммит
### echo "для конфликта" > Еще.txt
### git add Еще.txt
### git commit -m "для конфликта"
### •	Переключился на ветку mainNo3
### git checkout mainNo3
### •	Создал текстовый документ и добавил коммит
### echo "для конфликта" > Еще.txt
### git add Еще.txt
### git commit -m "для конфликта"
### •	Переключился на ветку main
### git checkout main
### •	Добавляем коммит
### echo "для конфликта" >> Еще.txt
### git add Еще.txt
### git commit -m "для конфликта"
### •	И запускаю команду слияния merge
### git merge mainNo3
![image](https://github.com/Fader77/bash/assets/137108770/22298ecc-f17e-4f61-935c-d481d281c2d4)
## 20.	Посмотрел в каких файлах есть конфликты. 
### •	git status
![image](https://github.com/Fader77/bash/assets/137108770/272b9fb3-3527-4bc7-8c49-90abe0fcc222)
## 21.	Устранил конфликты. 
### •	Отредактировал конфликтный файл
### •	Добавил коммит
### git add Еще.txt
### git commit -m "для конфликта"
![image](https://github.com/Fader77/bash/assets/137108770/d721b4a9-4f1a-420e-b4cc-2d88f6e06ff4)
## 22.	Переключился на указанный коммит. 
### •	git checkout 390e4fa
![image](https://github.com/Fader77/bash/assets/137108770/2b46a126-75e9-43ff-81b2-9c8fb072471b)
## 23.	Сделал ребазирование (rebase) текущей ветки. 
### •	git rebase main
![image](https://github.com/Fader77/bash/assets/137108770/07b7d50d-b682-449c-b3c7-8f88d8c814f8)
## 24.	Удалил ветку. 
### •	git branch -d mainNo3
![image](https://github.com/Fader77/bash/assets/137108770/686904b2-d89a-4cf5-9ede-8c8613c88e2b)
## 25.	Пропустил текущий конфликтный коммит и перейти к следующему. 
### •	git rebase --skip
## 26.	Отправил изменения из локального репозитория для указанной ветки в удаленный (дистанционный). 
### •	git push origin main
![image](https://github.com/Fader77/bash/assets/137108770/b0f16834-5c31-47e1-baf6-e0eceeb5cd4e)
## 27.	Забрал изменения из репозитория, для которого были созданы удаленные ветки по умолчанию.
### •	git pull origin main
![image](https://github.com/Fader77/bash/assets/137108770/70b39582-4961-4663-b864-22f147829f08)
## 28.	Забрал изменения удаленной ветки из репозитория основной ветки по умолчанию.
### •	git fetch
### •	git merge
![image](https://github.com/Fader77/bash/assets/137108770/6cfe7d2d-0338-4b3d-ae5b-2ffb3d53e81a)
## 29.	Создал копию репозитория.
### •	git clone https://github.com/Fader77/bash.git
![image](https://github.com/Fader77/bash/assets/137108770/5068d0ea-5152-4325-b8d0-0252dc5038ae)
