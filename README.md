# Мета роботи

Розібрати принципи та базові команди для роботи з git. Створити опис для свого акаунта GitHub.

# Хід роботи

1. Створити обліковий запис GitHub

![image_2023-05-05_02-37-28](https://user-images.githubusercontent.com/132616149/236353521-5467affe-e67b-4229-a0f3-a240f195db36.png)

2. Встановити CHOCOLATEY за допомогою powershell:
```
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
```


3. Встановити git на комп'ютер за допомогою Chocolatey:
```
choco install git -y
```
Перевіряємо правильність установки. Для цього дізнаємось версію встановленого гіт.

![image_2023-05-05_02-39-08](https://user-images.githubusercontent.com/132616149/236353576-5fe88ea4-56fd-4710-8993-18a305e9af08.png)

4. Налаштувати гіт за своїми даними:
```
git config --global user.name "AndriyVorobyov"
git config --global user.email andrey2001vor@gmail.com
```

5. Згенерувати новий SSH ключ:
```
ssh-keygen -t ed25519 -C "andrey2001vor@gmail.com"
```

Ключ було згенеровано за шляхом "C:\Users\hp\.ssh\" у файлі id_ed25519.pub

6. Додати ключ до облікового запису Github:

![image_2023-05-05_02-40-42](https://user-images.githubusercontent.com/132616149/236353645-9b323494-6013-4993-b029-43750eeeff5d.png)

7. Створити новий репозиторій з назвою такою ж як і назва акаунту:

![image_2023-05-05_02-56-41](https://user-images.githubusercontent.com/132616149/236354015-d94ddb8b-ed50-438b-8e00-51b3c8f016e1.png)

8. Склонувати репозиторій за допомогою git clone на локальний пк та відредагувати README.md:

![image_2023-05-05_02-42-03](https://user-images.githubusercontent.com/132616149/236354134-ff9e8c3a-314f-47db-8b2c-48de38e3804a.png)

9. Завантажити опис профілю:
```
git add .
git commit -m "prikol"
git push
```

![image_2023-05-05_02-44-16](https://user-images.githubusercontent.com/132616149/236354170-994ee548-7ce8-4bed-b08f-bd0cce891e68.png)

Висновок

Після виконання лабораторної роботи отримав знання про використання git та GitHub. Засвоїв принципи роботи з репозиторіями: як змінювати, додавати або видаляти файли з них. Ви ознайомилися з форматуванням тексту для файлу README.md.
