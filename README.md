**Выполненые проекты:**<br>

**Спринт 1**<br>

•Изучил тест-анализ, тест-дизайн<br>
•Анализировал требования, макеты, уточнял серые зоны<br>
•Декомпозировал и визуализировал требования с помощью mindmap<br>
•Состовлял блок схему на логику расчета стоимости и времени маршрута сервиса "Яндекс.Маршруты"<br>
•Выделял классы эквивалентности и граничные значения<br>
•Составлял тестовую документацию тест-кейсы для проектов Яндекс.Маршруты<br>

[Ссылка на проект](https://docs.google.com/spreadsheets/d/1NeUJ14WFq1YXWjXjn3DEMvHp89AUG6n2bw_ZCe5Mz5k/edit#gid=1058266973)<br>


**Спринт 2**<br>

•Изучил принципы работы веб-приложения (клиент-серверная архитектура, протоколы HTTP и HTTPS, структура HTTP-запроса ответ)<br>
•Просмотр запросов фронтенда и ответов бэкенда в DevTools<br>
•Тестировал веб-приложения с помощью чек-листа и тест-кейсов Яндекс.Маршруты на адаптивность, кроссбраузерность, выбирал конфигурацию с помощью pairwise<br> 
•Тестировал новую функциональность с помощью Charles<br>
•Заведение баг-репортов по результатам тестирования<br>

[Ссылка на проект](https://docs.google.com/spreadsheets/d/1CC45X7BmoMc7-vFV8mohzl2HbzJndpYUNHe51AtwTcc/edit#gid=899462569)<br>

**Спринт 3**<br>
•Проводил тестирование мобильного приложения Яндекс.Метро, с помощью реального устройства и эмулятора Android studio<br>
•Проводил тестирование бэкенда сервиса Яндекс.Прилавок API с помощью программы Postman. Протоколы REST и SOAP. Анализировал документацию к API в Apidoc и Swagger<br>
•Заведение баг-репортов по результатам тестирования<br>

[Ссылка на проект](https://docs.google.com/spreadsheets/d/1XXvwTIvaoni9XIDVhbG13rGYnw-Lmhs_ohhoA4_A1s8/edit#gid=857523888)


**Спринт 4**<br>
•Работал в консоли с логами. Подключался к удаленному серверу. <br>
•Изучил команды консоли для работы с логами (поиск, сохранение, перемещение, фильтрация и т.д.)<br>
•Изучил основы PostgreSQL, делал срезы данных, агрегирующие функции, группировка, сортировка данных, объединение таблиц<br>

[Ссылка на проект](https://docs.google.com/document/d/1FIVtbFurf_sOHla0BUemw3VRMTr6mQDLYiFMOSftqfw/edit)

**Спринт 5**<br>
•Изучил основы JavaScript <br>
•Изучил основы автоматизации с библиотекой Puppeteer<br>

Пример автотеста:<br>
https://github.com/Seelector0/Autotest.git

```
const puppeteer = require('puppeteer');

async function testYaRu(){
    console.log('Запуск браузера');
    const browser = await puppeteer.launch();

    console.log('Создание новой вкладки в браузере');
    const page = await browser.newPage();

    console.log('Переход на страницу ya.ru');
    await page.goto('https://ya.ru/');

    console.log('Ввод текста "Автоматизация тестирования" в поисковую строку');
    const searchField = await page.$('#text');
    await searchField.type('Автоматизация тестирования');

    console.log('Клик в кнопку "Найти"');
    const searchButton = await page.$('.button[type=submit]');
    await searchButton.click();
    
    console.log('Ожидание перехода в страницу поисковых результатов');
    await page.waitForNavigation();

    console.log('Получение элементов результата поиска');
    const result = await page.$('.serp-item');

    console.log('Сравнение ОР и ФР');
    if (result === null) 
    {console.log('Результаты поиска не найдены');} 
    else 
    {console.log('Результаты поиска отобразились')}
    
    console.log('Закрытие браузера');
    await browser.close();
}
```

**Дипломная работа**<br>
•Тестирование веб-приложения Яндекс.Самокат<br>
•Тестирование мобильного приложения Яндекс.Самокат<br>
•Тестирование API Яндекс.Самокат<br>

Ссылка на проект<br>

