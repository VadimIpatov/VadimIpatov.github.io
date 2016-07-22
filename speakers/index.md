---
layout: page
title: Хотите выступить?
excerpt: 
comments: true
---

Дайте нам знать!
Мы всегда рады видеть новых людей и слушать интересные доклады.

<form action="//getsimpleform.com/messages?form_api_token=64423d75fb4981e03fc6718d53dbda5e" method="post">
  <!-- the redirect_to is optional, the form will redirect to the referrer on submission -->
  <input type='hidden' name='redirect_to' value='http://kosbackend.ru/speakers/thank-you.html' />
  <!-- all your input fields here.... -->
  <p>
  <label for='name'>Ваше имя</label>
  <input type='text' name='name' id='name' required=""/>
  </p>
  <p>
  <label for='email'>E-mail для связи</label>
  <input type='email' name='email' id='email' required=""/>
  </p>
    <p>
  <label for='theme'>Тема доклада</label>
  <input type='text' name='theme' id='theme' required="" />
  </p>
    <p>
  <label for='duration'>Примерная длительность</label>
  <select id="duration" name="duration" required="">
    <option value="15">15 минут</option>
    <option value="30">30 минут</option>
    <option value="45">45 минут</option>
    <option value="60">1 час</option>
    <option value="more">Больше часа</option>
  </select>
  </p>
  <p>
  	<input type='submit' value='Подать заявку' class='btn' />
  </p>
</form>
