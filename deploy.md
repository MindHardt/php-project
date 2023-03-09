Как деплоить на локальной машине.

### 1. Клонируем репу, желательно внутри папки /OSPanel (например, `C://OSPanel/auth`)

### 2. Поднимаем мускуль любым способом. Я использую докер

<details>
  <summary>Команда для докера</summary>
  
   `docker run --name some-mysql -e MYSQL_ROOT_PASSWORD=my-secret-pw -e MYSQL_DATABASE=default -p 3306:3306 -d mysql:latest`
</details>

Если вы не используете докер то измените файл `./.env` чтобы стучало к вашей БД

### 3. Открываем консось опенсервера, переходим в папку проекта (`cd auth`), даем божеству по имени artisan включить вам вебсервер (`php artisan serve`)

Готово, вы замечательны!

![мопс](https://yandex-images.clstorage.net/5H1rsH168/423204DZ8b/rS7UgUVk0fpK_DKJa_NpqaUxKYyv6-kRNIHRz7inr5BR68ZHHcPuA9mMyJvQprqtEaByvh9E4ptUNIzy9hCJQ-1-k81eep7wS_wxhGLoYK6uOSaEq__uE2zWyp3itfGTHq_MF3CsmHb54r75rtnD0V6gfu9PDPvfF1uy_7BqwjKeCsG0bVin_knnTrt8xGuUl1M2jZSB2H4Uo6qe97yNoi2Og0FXvpNRzsuLyqDK7NpEtmDSXSOP6zBChq-iQ9YdrSjurm97mM1AxV2HY9R_ir5bN7m4t_FDEJSCrPWsmL43k4hkZ5evXfnpkNGX2fP7a7V3w148msktfquPmnLFHKEByLhlXrnHQOprmXraV527fC6CobbvdC63v5_NgL-hI7eLd0CajEfM7rD9hNjj3XWKYc5aLbfcB3SPj7FL-ACWCMWYWnyK50XkS4V-yW-UllQVpK2m-G0agLyR4KmFjh-nhm9Yu5tU_N6Z3ovGwthskkTObzeX4RFvta2FeuggswDOsURil8Be6nGGYPJ6g6dKBoi2g-9GPISmn_aogroJtYhkWIKoXs7kmO-X9sLYbbB47UU-u8kHV4y0kVbDMagEw4d1VqvbfOV5qnDHap6WdCagtLXFZxiTlazoqruiKpqEUVmKu3nZ6YfyttHEz3agXNJTJozMFEyqnod1whKvAdWXfXCH533idp9s2keKsn0Li7OG1VQRsKWz4q6isSWvl0RHvZt01861-4z808t1lXj6SBub9RBJr62TUcgMtgX3iX5yue5Fw1GfeO9ruo1TA5Oxq9dtJaSchfy2vaYUrLtAW6S4cNT1md2f78XMZK1D-EU_sf8ufK-ujVj-K54o9bFTZbHSW9lygmn0e4SZdhellJTYSy2Ro4bit7KPHqmHQ1yBj3rf5Z_ygOvJ21SqXfpIGYT9E2Orta5b3w2KNfaWc1S7wnboabRbx3mUuFYkgaGo7Fsys5W3xLQ)

# Как редактировать что-то???

### Если изменяем `.php` файлы то думать не надо, перезапускать сервер тоже, сохранили на `Ctrl+S`, обновили на `F5` в браузере и кайфуем
