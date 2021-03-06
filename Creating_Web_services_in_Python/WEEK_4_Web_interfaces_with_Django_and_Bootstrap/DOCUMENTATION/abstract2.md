## Полезные ссылки и дополнительные материалы
Туториал создание первого Django приложения (https://docs.djangoproject.com/en/1.11/intro/tutorial01/)

Созданный проект (https://github.com/alexopryshko/coursera_blog)

## Материалы по роутингу и устройство view:
* https://docs.djangoproject.com/en/1.11/ref/request-response/
* https://docs.djangoproject.com/en/1.11/topics/http/urls/
* https://docs.djangoproject.com/en/1.11/topics/http/views/
* https://docs.djangoproject.com/en/1.11/topics/http/decorators/
## Материалы по шаблонизации:
* https://docs.djangoproject.com/en/1.11/topics/templates/
* https://docs.djangoproject.com/en/1.11/ref/templates/builtins/
* https://docs.djangoproject.com/en/1.11/howto/custom-template-tags/
* https://docs.djangoproject.com/en/1.11/ref/settings/
Различия Django 1.11 и 2.0
В курсе рассмотрена версия Django 1.11, так как является стандартом технологии и многие существующие проекты написаны на более ранних версиях, которые несущественно отличаются от версии 1.11.

Важное замечание: поддержка  Python3.7 в Django1.11 появилась только в версии 1.11.17. Поэтому, если вы используете Python версии 3.7 выполняйте установку Django с указанием версии:
```Python
pip3 install django == 1.11.17
```

Тем не менее, рассмотрим отличия версии Django 2.0 от Django 1.11:
* Django 2.0 поддерживает Python 3.4, 3.5 и 3.6. Django 1.11.x является последней, которая поддерживает Python 2.7.
* Упрощенный routing. Новая функция django.urls.path() упрощает синтаксис роутинга. Например:
```Python
# django 1.11
url(r'^articles/(?P<year>[0-9]{4})/$', views.year_archive)

# django 2.0
path('articles/<int:year>/', views.year_archive)
```
* Адаптированный под мобильные устройства раздел администрирования
* Window выражения

Полный список изменений - https://docs.djangoproject.com/en/2.0/releases/2.0/
For more:https://django.cowhite.com/blog/working-with-url-get-post-parameters-in-django/
