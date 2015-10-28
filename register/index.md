---
layout: page
title: Приходите в гости!
comments: true
---

Если вы хотите посетить ближайшее мероприятие, пожалуйста, зарегистрируйтесь. 

Это не обязательно, но ваша заявка позволит
нам лучше спланировать мероприятие, а также лучше узнать наших гостей и в будущем подготовить больше интересных докладов.


<form action="http://getsimpleform.com/messages?form_api_token=2e9c438668c9b50479edcbba97b8e85d" method="post">
  <!-- the redirect_to is optional, the form will redirect to the referrer on submission -->
  <input type='hidden' name='redirect_to' value='http://kosbackend.hub44.net/register/thank-you.html' />
  <!-- all your input fields here.... -->
  <label for='name'>Имя</label>
  <input type='text' name='name' id='name' required=""/>
  <label for='surname'>Фамилия</label>
  <input type='text' name='surname' id='surname' required=""/>
  <label for='email'>E-mail для связи</label>
  <input type='email' name='email' id='email' required="" />
  <label for='work'>Место работы/учебы</label>
  <input type='text' name='work' id='work' required="" />
  <label for='about'>Пара строк о себе (профессиональные интересы, etc...)</label>
  <textarea name='about' id='about' rows='8'></textarea>
  <p>
  	<input type='submit' value='Подать заявку' class='btn' />
  </p>
</form>