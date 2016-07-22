---
layout: page
title: Приходите в гости!
comments: true
---

Если вы хотите посетить ближайшее мероприятие, пожалуйста, зарегистрируйтесь. 
Это позволит нам лучше спланировать встречу, узнать наших гостей и в будущем подготовить больше интересных докладов.


<form action="//getsimpleform.com/messages?form_api_token=64423d75fb4981e03fc6718d53dbda5e" method="post">
  <!-- the redirect_to is optional, the form will redirect to the referrer on submission -->
  <input type='hidden' name='redirect_to' value='http://kosbackend.ru/register/thank-you.html' />
  <!-- all your input fields here.... -->
  <p>
  <label for='name'>Имя</label>
  <input type='text' name='name' id='name' required=""/>
  </p>
  <p>
  <label for='surname'>Фамилия</label>
  <input type='text' name='surname' id='surname' required=""/>
  </p>
  <p>
  <label for='email'>E-mail для связи</label>
  <input type='email' name='email' id='email' required="" />
  </p>
  <p>
  <label for='work'>Место работы/учебы</label>
  <input type='text' name='work' id='work' required="" />
  </p>
  <label for='position'>Должность</label>
  <input type='text' name='position' id='position' required="" />
  </p>
  <p>
  <input type='checkbox' name='afterparty' id='afterparty' /> <b>Пойду на afterparty</b>
  </p>
  <p>
  	<input type='submit' value='Подать заявку' class='btn' />
  </p>
  <br>
  <p><a class="fa fa-calendar" href="webcal://kosbackend.ru/register/kosbackend.ics"> Создать напоминание в календаре</a></p>
</form>