Мы предлагаем вам разработать бота, который позволит сохранять места для будущего посещения.

Например, вы идете по улице, видите отличный ресторан, и хотите не забыть в него зайти в свободный вечер. Вам нужно каким-то образом отправить название места и его адрес, возможно приложить фотографию.

В будущем, вы можете обратиться к боту и либо просто просмотреть список мест, которые вы раньше сохраняли, либо отправить текущее местоположение и получить самое ближайшее место.

Для разработки этого бота вам будет необходимо сделать хранилище данных: базу даных или файлы. Вам также нужно использовать команды для ботов и обмен сообщений с разным типом вложений.

Бот должен реагировать на три команды:
* /add – добавление нового места;
* /list – отображение добавленных мест;
Вы можете реализовать один из двух уровней сложности команды /add:

* /reset позволяет пользователю удалить все его добавленные локации (помним про GDPR)
* указание адреса ресторана сразу в сообщении команды, в один шаг;
* пошаговое добавление места, с добавлением фото и локации.
Команда /list в базовом варианте должна показывать 10 последних добавленных мест.

Расширенная версия бота должна возвращать места в радиусе 500 метров при отправке локации, или возвращать сообщение об отсутствии добавленных мест. Расчёт расстояния можно производить при помощи удобного Google Maps APIs.

Не забудьте учитывать пользователя, который добавляет места и возвращать ему только его сохраненные места.

Своего бота вы должны загрузить на сервис Heroku. Имейте в виду, что файлы сохраненные вашим ботом как локальные, будут уничтожены при остановке контейнера, поэтому для длительного хранения нужно подключить какую-нибудь SQL или NoSQL базу данных и использовать её.

Также не стесняйтесь проявлять фантазию! Помимо описанных в задании возможностей, бот может реализовывать намного больше функционала.

## Review criteria:
Для проверки работоспособности бота нужно будет начать с ним чат в мессенджере Telegram, проверить возможность добавить новое место с помощью команды /add, возможность получить добавленные места с помощью команды /list и возможность удалить все сохранённые места при помощи команды /reset.

В расширенной версии также нужно проверить возможность пошагового добавления места при помощи команды /add и возможность получения мест в радиусе 500 метров, при отправке локации.s