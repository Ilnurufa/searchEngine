## **Поисковый движок**
Поисковый движок представляет из себя Spring-приложение работающее с локально установленной базой данных MySQL, имеет 
простой веб-интерфейс и API, через который им можно управлять и получать результаты поисковой выдачи по запросу.
1. В конфигурационном файле перед запуском приложения задаются адреса сайтов, по которым движок должен осуществлять поиск.
2. Поисковый движок должен самостоятельно обходить все страницы заданных сайтов и индексировать их (создавать так называемый индекс) так, чтобы потом находить наиболее релевантные страницы по любому поисковому запросу.
3. Пользователь присылает запрос через API движка. Запрос — это набор слов, по которым нужно найти страницы сайта.
4. Запрос определённым образом трансформируется в список слов, переведённых в базовую форму. Например, для существительных — именительный падеж, единственное число.
5. В индексе ищутся страницы, на которых встречаются все эти слова.
6. Результаты поиска ранжируются, сортируются и отдаются пользователю

### **Скриншоты работы программы**
1. Страница статистики.
На этой странице можно просмотреть информацию о индексируемых или проиндексированных сайтах.
![Страница статистики](/images/dashboard.JPG "Страница статистики")
2. Страница индексации.
Можно запустить полную индексацию, либо индексацию отдельно взятой страницы.
![Страница индексации](/images/managment.JPG "Страница индексации")
3. Страница поиска.
Можно искать по всем сайтам, или по отдельно выбранному сайту.
![Страница поиска](/images/search.JPG "Страница поиска")

### **Технологии**
`Java`
`Spring boot`
`MySQL`
`JavaScript`
`CSS`