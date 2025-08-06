# <span style="color: #425CB5">ID Заказа</span> и <span style="color: #425CB5">ID Торгов</span>

При регистрации заявки на платформе каждому заказу присваивается уникальный идентификатор **"ID заказа"**. При выкладке заказа на торги создается **"ID торгов"**, что позволяет отслеживать весь <span style="color: #425CB5">"жизненный цикл"</span> заказа. 

---

## Из чего состоит <span style="color: #425CB5">ID Заказа</span>  

- Системный идентификатор заказа 
- Конвертация последних 5 цифр ИНН Заказчика в буквы 
- **<span style="color: #425CB5">Время (час) по Гринвичу</span>** создания заказа  
- **<span style="color: #425CB5">Дата создания заказа</span>** в формате: `ITMM-ДД`  

---

<div class="schema-container">
  <div class="header">
    <span>0-MPREE-2506-03-06-001</span>
  </div>
  <div class="row">
    <div class="box" style="margin-left: 5%; margin-right: 1%;">
      <p>Системный<br>идентификатор<br>заказа</p>
    </div>
    <div class="box" style="margin-left: 1%; margin-right: 1%;">
      <p>Порядковый<br>номер заказа<br>созданный<br>в рамках<br>часа</p>
    </div>
    <div class="box" style="margin-left: 1%; margin-right: 1%;">
      <p>Конвертация<br>последних<br>5-ти цифр<br>ИНН Заказчика<br>в буквы</p>
    </div>
    <div class="box" style="margin-left: 1%; margin-right: 1%;">
      <p>Время (час)<br>по Гринвичу<br>когда был<br>создан заказ</p>
    </div>
    <div class="box" style="margin-left: 1%; margin-right: 5%;">
      <p>Дата создания<br>заказа, в формате:<br>ГГММ-ДД</p>
    </div>
  </div>
</div>

<style>
    .schema-container {
        flex-direction: column;
        align-items: center;
        background-color: #f9f9f9; /* Светло-серый фон */
        padding: 10px;
    }

    .header {
        text-align: center;
        font-size: 30px;
        font-weight: bold;
        margin-bottom: 100px;
        }

    .row {
        display: flex;
        justify-content: space-around;
        margin-bottom: 30px;
        }

    .box {
        background-color: white;
        border: 1px solid #ccc;
        padding: 10px;
        border-radius: 5px;
        box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        vertical-align: middle;
        min-width: 80px;
        position: relative; /* Добавляем relative для корректной работы ::before */
        }

    /* Добавляем стрелки между блоками */
    .box::before {
        content: "";
        position: absolute;
        width: 0;
        height: 0;
        border-style: solid;
        border-width: 10px 10px 0 10px;
        border-color: #425CB5 transparent transparent transparent;
        top: -20px;
        left: 50%;
        transform: translateX(-50%);
        }

    /* Позиционирование стрелок */
    .box:nth-child(1)::before {
        top: -20px;
        }
        .box:nth-child(2)::before {
        top: -20px;
        }
        .box:nth-child(3)::before {
        top: -20px;
        }
        .box:nth-child(4)::before {
        top: -20px;
        }
        .box:nth-child(5)::before {
        top: -20px;
        }
  </style>

## Из чего состоит <span style="color: #425CB5">ID Торгов</span>  

- **<span style="color: #425CB5">Системный идентификатор торгов</span>**  
- **<span style="color: #425CB5">Конвертация последних 5 цифр ИНН Заказчика в буквы</span>***  
- **<span style="color: #425CB5">Время (час) по Гринвичу</span>** размещения заказа на торги  
- **<span style="color: #425CB5">Дата размещения заказа на торги</span>** в формате: `ITMM-ДД`  

---

\* По запросу Заказчика в поддержку платформы партнер может заменить **<span style="color: #425CB5">префикс</span>** (буквенную замену 5 последних цифр ИНН) на любую другую аббревиатуру.  

Все изменения для этого проекта могут быть выполнены в вашем общедоступном репозитории GitHub под названием "diplodoc-example/docs".
Чтобы внести изменения и применить их:

- перейдите в ваш репозиторий по адресу "diplodoc-example/docs"
- внесите изменения в структуру проекта или контент
- закоммитьте и отправьте изменения в ваш репозиторий
- перейдите на вкладку "Actions" (Действия) для репозитория документации
- запустите действие "Release" (Выпуск) и дождитесь его завершения
- готово, обновления должны быть доступны для всех

Если вы хотите сделать прокси с вашего собственного домена на эту документацию, пожалуйста, [воспользуйтесь гайдом из документации](https://diplodoc.com/docs/ru/personal-domain-ya-cloud).
