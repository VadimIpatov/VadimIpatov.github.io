---
layout: talk
title: "Отладка и профилирование node.js приложений"
modified:
categories: talks
author: olegas
excerpt:
tags: [nodejs, debugging, profiling]
image:
  feature:
talk: meetup2
date: 2016-03-26T16:00:00+04:00
comments: true
share: true
announce:
video:
slides: 
---

* Рабоче-колхозный console.log
* Встроенный отладчик — отлаживаем из консоли, какие есть проблемы (cluster)
* Отладка через node-inspector (кратко все возможности и чуть подробнее о профилировании и анализе кучи — заход на простые утечки через JS)
* Сторонние средства онлайн-мониторинга (когда что-то нужно снять с процесса без возможности подключения инспектором: heapdump, gc-stat, process.memoryUsage())

<iframe width="560" height="315" src="//www.youtube.com/embed/w3gF38bfeCI" frameborder="0" allowfullscreen></iframe>