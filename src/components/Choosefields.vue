<template>
    <div class="first_step_wrapper">
        <div class="choose_fields_wrapper">
            <h3>Выберите поля:</h3>
            <div class="choose_form">
                <form action="">
                    <label class="container"><input type="checkbox" checked="checked">
                    <span class="checkmark"></span></label>
                    <input type="name" placeholder="Иван">
                    <label class="container"><input type="checkbox" checked="checked">
                    <span class="checkmark"></span></label>
                    <input type="phone" placeholder="+79000000000">
                    <label class="container"><input type="checkbox">
                    <span class="checkmark"></span></label>
                    <input class="passive" type="email" placeholder="example@mail.ru">
                    <button>Связаться со мной!</button>
                </form>
            </div>
        </div>
        <div class="template_wrapper">
            <h3>Шаблон письма:</h3>
            <p class="sender"><span>От кого:</span> О!Почта</p>
            <p class="thema">
                <span class="thema_name">Тема:</span> Новое сообщение от <span class="name">Иван
                    </span> с <span class="site_name">example.com</span>
            </p>
            <p class="template_text">
                Пользователь с именем <span class="name">Иван
                    </span> с номером телефона <span class="phone">+79000000000
                        </span> отправил вам заявку на обратную связь
            </p>
        </div>
    </div>
</template>
<style scope>
    .first_step_wrapper {
        display: inline-block;
    }
    .choose_fields_wrapper {
        width: 700px;
        height: 350px;
        background-color: #13BEBB;
        border-radius: 100px 60px 100px 60px;
        margin-left: 200px;
        margin-top: 40px;
        display: inline-block;
    }
    .template_wrapper {
        width: 700px;
        height: 350px;
        background-color: #13BEBB;
        border-radius: 60px 100px 60px 100px;
        display: inline-block;
        margin-top: 40px;
        margin-left: 70px;
        float: right;
        color: #130D44;
    }
    .first_step_wrapper h3 {
        font-family: Raleway-SemiBold;
        font-size: 36px;
        color: #130D44;
        text-align: center;
        padding-top: 15px;
        margin: 0;
    }
    .choose_form {
        width: 480px;
        height: 250px;
        background-color: #130D44;
        margin-left: 125px;
        margin-top: 20px;
        border-radius: 30px;
        position: relative;
    }
    .choose_form form {
        position: absolute;
        left: 0;
        top: 0;
        right: 0;
        bottom: 0;
        margin: auto;
        display: block;
        width: 400px;
        height: 200px;
    }
    .choose_form form input, button {
        width: 400px;
        height: 35px;
        background-color: #FFF3F3;
        border-radius: 10px;
        border: 1px solid #FFF3F3;
        box-sizing: border-box;
        margin-bottom: 18px;
        outline: none;
        font-family: 'Open Sans';
        font-size: 26px;
        color: #130D44;
        line-height: 35px;
        position: relative;
    }
    .choose_form form input {
        padding-left: 20px;
    }
    .choose_form form button {
        height: 40px;
        font-weight: 600;
        font-size: 27px;
        padding-left: 0;
    }
    .choose_form form input::placeholder {
        font-family: 'Open Sans';
        font-size: 26px;
        color: #130D44;
    }
    .choose_form form .passive {
        background-color: #CECBCB;
        border-color: #CECBCB;
    }
    .choose_form form input.passive::placeholder {
        color: rgba(19, 13, 68, 0.5);
    }
    .container {
        display: block;
        position: relative;
        cursor: pointer;
        -webkit-user-select: none;
        -moz-user-select: none;
        -ms-user-select: none;
        user-select: none;
        width: 0;
        height: 0;
    }
    .container input[type="checkbox"] {
        position: absolute;
        opacity: 0;
        cursor: pointer;
        height: 0;
        width: 0;
    }
    .checkmark {
        width: 30px;
        height: 30px;
        position: absolute;
        left: -120px;
        background-color: rgba(19,13,68, 97);
    }
    .container:hover input[type="checkbox"] ~ .checkmark {
        background-color: rgba(19, 13, 68, 0.5);
    }
    .container input[type="checkbox"]:checked ~ .checkmark {
        background-color: #FFF3F3;
    }
    .checkmark:after {
        content: "";
        position: absolute;
        display: none;
    }
    .container input[type="checkbox"]:checked ~ .checkmark:after {
        display: block;
    }
    .container .checkmark:after {
        background-image: url(../assets/img/check.png);
        width: 40px;
        height: 40px;
        left: 7px;
        bottom: 0;
        background-repeat: no-repeat;
    }
    .template_wrapper p.sender span {
        font-family: 'Open Sans';
        font-size: 24px;
        font-weight: 600;
        padding-left: 60px;
        padding-right: 30px;
    }
    .template_wrapper p.sender, p.thema {
        font-family: 'Open Sans';
        font-size: 22px;
        font-weight: 400;
    }
    .template_wrapper p.thema span.thema_name, span.name {
        font-family: 'Open Sans';
        font-size: 24px;
        font-weight: 600;
    }
    .template_wrapper p.thema span.name {
        font-size: 23px;
        font-family: Raleway-SemiBold;
        font-style: italic;
    }
     .template_wrapper p.thema span.site_name {
        font-size: 23px;
        font-style: italic;
        font-weight: 600;
    }
    .template_wrapper p.thema span.thema_name {
        padding-left: 60px;
        padding-right: 60px;
    }
    .template_wrapper h3 {
        padding-bottom: 20px;
    }
    .template_wrapper p.template_text {
        font-family: Raleway-Regular;
        font-size: 23px;
        padding-left: 60px;
    }
    .template_wrapper p.template_text span {
        font-style: italic;
        font-weight: 600;
    }
</style>
