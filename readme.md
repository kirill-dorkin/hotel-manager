# HotelManager

### О проекте
«HotelManager» - это приложение, предназначенное для администратора гостиницы. Обеспечивает хранение сведений о гостинице, гостиничных номерах, проживающих клиентах и работниках, убирающих номера.

«HotelReportsServer» - TCP-сервер, принимающий отчеты о работе гостиниц.

### Используемые технологии
* С#/.NET Framework 4.7
* Entity Framework 6
* WPF (MVVM pattern)
* N-Layer Architecture
* Material Design In XAML Toolkit
* MahApps.Metro
* AutoMapper

### Features
* Динамический поиск клентов и работников по любой характеристике
* Гибкая фильтрация и сортировка
* Темная и светлая темы
* Свободная настройка цветовой палитры приложения
* Material Design
* Многослойная архитектура

![alt text](/Screenshots/screenshot1.png?raw=true)
![alt text](/Screenshots/screenshot2.png?raw=true)
![alt text](/Screenshots/screenshot3.png?raw=true)

### Запуск

1. Установите **Visual Studio 2019** или более новую версию с рабочей нагрузкой
   "Разработка классических приложений .NET". Вместе с ней будет
   установлен **.NET Framework 4.7.2**.
2. Убедитесь, что на компьютере установлен **SQL Server Express LocalDB**.
   Приложение использует подключение `HotelDbContext` к экземпляру
   `(localdb)\MSSQLLocalDB`.
3. Склонируйте репозиторий или загрузите архив с исходным кодом.
   ```bash
   git clone <url репозитория>
   ```
4. Откройте файл `HotelManager/HotelManager_Coursework.sln` в Visual Studio и
   дождитесь восстановления NuGet‑пакетов. После этого постройте решение.
5. Для приёма отчётов запустите сервер из решения
   `HotelReportsServer/HotelReportsServer.sln`. Установите проект
   `HotelReportsServer` стартовым и запустите его (порт по умолчанию `8888`).
6. Вернитесь к решению `HotelManager_Coursework.sln` и запустите приложение
   `HotelManager.UI` (F5). При первом старте база данных будет создана
   автоматически.
7. В приложении выберите период формирования отчёта и отправьте его на сервер.
   После успешной отправки появится уведомление.
