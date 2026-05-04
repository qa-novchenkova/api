# 🔌 REST and SOAP API testing

### REST API — Demoshopping ([Swagger UI](https://intern.demoshopping.ru/api-docs/))

Протестировала REST API учебного интернет‑магазина https://intern.demoshopping.ru по спецификации [Swagger UI](https://intern.demoshopping.ru/api-docs/). 

Собрала коллекцию в **Postman** со всеми методами. Добавила переменные коллекции (в том числе динамические: логин, **токен авторизации** и др.) и скрипты в **Pre-request** / **Post-response** (проверка HTTP‑статуса, извлечение данных в переменные для цепочки запросов и пр.).

**Прогон коллекции (RUN)** полностью автоматический; перед запуском нужно убрать галочки с двух запросов **DELETE** у delete_product (иначе прогон не дойдет до конца).

<ul>
<li>
	<a href="https://drive.google.com/file/d/1QgDvMvWNOIwWLrhdpog0AVrGPM7tooZP/view?usp=sharing" target="_blank">Postman-коллекция (JSON)</a> — коллекция в формате json для импорта в Postman.
</li>
<li>
	<a href="https://drive.google.com/file/d/1DbRqm8_qQ-epODYrywZuS2GZywnbbBF1/view?usp=sharing" target="_blank">Успешный автоматический прогон коллекции.</a>
</li>
</ul>


### REST API — Swagger Petstore ([Swagger UI](https://petstore.swagger.io/))
Протестировала публичный REST API **Swagger Petstore** в **Postman** по модулям `pet`, `store`, `user`; добавила переменные коллекции и автопроверки.  

**Материалы**
- Postman-коллекция (JSON): [Ссылка на файл коллекции](https://drive.google.com/file/d/1y2KQ8vnihapHMXBGA_yeodNrg9CrYD4u/view?usp=sharing)
- Успешный прогон коллекции (скрин): [Ссылка на скрин Runner](https://drive.google.com/file/d/1LsV1Fgd8LATmL7rN9cREmRJ34Dss91kX/view?usp=sharing)


### SOAP API ([WSDL](http://webservices.oorsprong.org/websamples.countryinfo/CountryInfoService.wso?WSDL))

Протестировала публичный SOAP‑веб‑сервис **CountryInfoService** (данные о странах, континентах, языках по [WSDL](http://webservices.oorsprong.org/websamples.countryinfo/CountryInfoService.wso?WSDL)). Собрала в **Postman** коллекцию запросов (**FullCountryInfo**, **ListOfContinentsByName**, **CountryName**, **LanguageName**) с разными входными параметрами (ISO‑коды страны и языка).

Также провожу проверки в **SoapUI**: импорт WSDL, работа с операциями и просмотр XML‑ответов (например, **CapitalCity**).

<ul>
<li>
	<a href="https://drive.google.com/file/d/1fwN4lV8De4AzZOh-suycwjaUIShFLj3a/view?usp=sharing" target="_blank">Postman-коллекция SOAP (JSON)</a> — для импорта в Postman.
</li>
<li>
	<a href="https://drive.google.com/file/d/1N4SMXUQCjm2a6GtYavPUX7SvGT1ChgOQ/view?usp=sharing" target="_blank">Пример работы в SoapUI</a> — запрос к операции сервиса и ответ сервера.
</li>
</ul>
