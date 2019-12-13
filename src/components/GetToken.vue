<template>
    <div class="get_token_wrapper">
        <form action="" class="get_token_form">
            <input type="text" placeholder="Email">
            <input type="text" placeholder="Пароль">
            <label for="">Согласен с правилами использования сервиса
                <input type="checkbox">
            </label>
            <button>Зарегистрироваться</button>
        </form>
    </div>
</template>
<style scope>
    .get_token_wrapper {
        position: relative;
        width: 1480px;
        height: 250px;
        display: block;
        background-color: #13BEBB;
        text-align: center;
        margin: auto;
        border: 1px solid #13BEBB;
        box-sizing: border-box;
        border-radius: 100px 60px 100px 60px;
        margin-top: 40px;
    }
    .get_token_wrapper input {
        width: 320px;
        height: 50px;
        background-color: #130D44;
        border: 1px solid #130D44;
        box-sizing: border-box;
        border-radius: 40px 20px 40px 20px;
        color: #FFF3F3;
        font-family: 'Open Sans';
        font-size: 26px;
        padding-left: 30px;
        margin-right: 80px;
    }
    .get_token_wrapper button {
        width: 320px;
        height: 50px;
        background-color: #130D44;
        border: 1px solid #130D44;
        box-sizing: border-box;
        border-radius: 40px 20px 40px 20px;
        color: #FFF3F3;
        font-family: 'Open Sans';
        font-size: 26px;
        text-align: center;

    }
    .get_token_wrapper input::placeholder {
        font-family: 'Open Sans';
        font-size: 26px;
        color: #FFF3F3;
    }
    .get_token_wrapper input[type="checkbox"] {
        width: 30px;
        height: 30px;
        position: absolute;
        left: -5px;
        top: -5px;
        background-color: #FFF3F3;
    }
    .get_token_wrapper label {
        font-size: 14px;
        color: #FFF3F3;
        width: 200px;
        display: inline-block;
        height: 30px;
        line-height: 14px;
        position: relative;
    }
    .get_token_wrapper form {
        display: block;
        width: 1480px;
        height: 50px;
        margin: 0 auto;
        position: absolute;
        left: 0;
        top: 50%;
        transform: translateY(-50%);
    }
</style>
