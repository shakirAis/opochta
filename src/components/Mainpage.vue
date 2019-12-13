<template>
    <div class="main">
        <div class="slogan">
            <h1>Как создать форму обратной  связи за 5 минут?</h1>
            <p>без смс и с регистрацией</p>
        </div>
        <div class="steps">
            <div class="first_step step">
                <img src="../assets/img/fill.png" alt="Шаг первый">
                <h2><span> Шаг 1:</span> настройте форму</h2>
            </div>
            <Choosefields></Choosefields>
            <div class="second_step step">
                <img src="../assets/img/forms.png" alt="Шаг второй">
                <h2><span> Шаг 2:</span> получите токен</h2>
            </div>
            <GetToken></GetToken>
            <div class="third_step step">
                <img src="../assets/img/code.png" alt="Шаг третий">
                <h2><span> Шаг 3:</span> вставьте код формы в ваш проект</h2>
            </div>
            <CodeSample></CodeSample>
        </div>
    </div>
</template>
<script>
import Choosefields from './Choosefields';
import GetToken from './GetToken';
import CodeSample from './CodeSample';

export default {
  name: 'Mainpage',
  components: {
    Choosefields,
    GetToken,
    CodeSample,
  },
};
</script>
<style scoped>
.slogan h1 {
    margin-top: 110px;
    margin-bottom: 0;
    display: inline-block;
    text-align: center;
    width: 100%;
    font-size: 56px;
    letter-spacing: -2px;
    font-family: Raleway-Regular;
    text-transform: uppercase;
    font-variant-numeric: lining-nums;
    font-weight: 400;
}
.slogan p {
    font-family: 'Open Sans';
    display: inline-block;
    width: 100%;
    text-align: center;
    color: #FF7400;
    font-size: 40px;
    letter-spacing: -3px;
    line-height: 70px;
    margin: 0;
}
.steps {
    margin-top: 130px;
}
.steps .step {
    height: 100px;
    display: inline-table;
}
.steps .step img {
    height: 100px;
    margin-left: 300px;
    display: inline-block;
}
.steps .step h2 {
    display: table-cell;
    font-family: Raleway-Regular;
    font-size: 42px;
    font-weight: 400;
    line-height: 50px;
    margin: 0;
    vertical-align: middle;
    padding-left: 30px;
}
.steps .step h2 span {
    font-family: Raleway-SemiBold;
    text-transform: uppercase;
    padding-right: 20px;
}
.second_step, .third_step {
    margin-top: 50px;
}
</style>
