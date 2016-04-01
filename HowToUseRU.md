# Введение #

В интернете часто задают вопрос: **_как добавить комментарии Disqus к моему сайту, сделанному в Google Sites?_**

[Disqus](http://disqus.com) предоставляет решение "из коробки" для некоторых  блог-платформ и сервисов, но не для Google Sites.

А вот простое готовое решение.


# Google Sites + Disqus #

  1. Зарегистрируйте свой сайт на Disqus, чтобы получить "короткое имя" (shortname): https://disqus.com/admin/signup (можете прочитать  [здесь](http://help.disqus.com/customer/portal/articles/466208-what-s-a-shortname-) что это такое).
  1. Откройте страницу вашего сайта в Google Sites, на которую вы хотите добавить комментарии Disqus, в режиме редактирования и поместите курсор туда, где должны быть комментарии.
  1. В левом верхнем углу выберите пункт меню **Вставить -> Дополнительные гаджеты...**.
  1. В открывшемся диалоге выберите **Добавить гаджет по URL** и вставьте этот URL: https://google-sites-disqus.googlecode.com/git/disqus-gadget.xml (или скачайте этот файл и захостите его где-нибудь у себя).
  1. Откроется диалог с параметрами гаджета. Заполните: [Disqus shortname](http://help.disqus.com/customer/portal/articles/472098-javascript-configuration-variables#disqus_shortname) (обязательно), [Discus URL](http://help.disqus.com/customer/portal/articles/472098-javascript-configuration-variables#disqus_url) (настоятельно рекомендуется), [Discus identifier](http://help.disqus.com/customer/portal/articles/472098-javascript-configuration-variables#disqus_identifier) (настоятельно рекомендуется), [Disqus title](http://help.disqus.com/customer/portal/articles/472098-javascript-configuration-variables#disqus_title) (рекомендуется).
  1. Можете нажать предпросмотр или завершить вставку гаджета.

Вы можете посмотреть процесс в [обучающем видеоролике (на английском)](http://vimeo.com/67653417), который разместил Doug Saunders в  [своём блоге](https://sites.google.com/site/wilderitrt/news/addingpubliccommentstoagooglesite).

## Предупреждение: ##
Как только откроется предпросмотр гаджета Disqus, на сервисе Disqus будет создано новое обсуждение, как если бы гаджет показывался на странице вашего сайта с выбранными параметрами.

## Откуда брать параметры ##
**Short name** (обязательный) - ID вашего сайта, вы получаете его при регистрации сайта в консоли Disqus

**Disqus url** (настоятельно рекомендуется) - URL страницы, которой будет относиться дискуссия - по этому URL, например, можно будет перейти из уведомлений о новых сообщениях в почте. Если не указан, то будет подставлен URL страницы, на которой в первый раз отработал скрипт. Если вы его не укажете, то, например, при открытии предпросмотра гаджета туда может быть записан мусор.

**Disqus identifier** (настоятельно рекомендуется) - ID дискуссии однозначно определяет дискуссию. Т.е. для разного набора комментариев необходимо указывать разные ID. Для новой дискуссии просто придумайте новый ID, например _page1_, _page2_, _super-page123_ и т.п. Если дискусии с указанным ID не существует, то при первом обращении она будет создана. Если указать существующий ID, то будет загружена существующая дискуссия, даже если URL будет указан другой. Обратите внимание, что пустой Disqus ID - это тоже ID, т.е. при указании пустого ID на разных страницах будет загружен один и тот же набор комментариев!

**Disqus title** (рекомендуется) - заголовок, с которым дискуссия будет зарегистрирована, если её еще не существует. Если не указать, будет использован заголовок страницы.

## Совместимость ##
Проверена совместимость со следующими браузерами (в других тоже должно работать, но в этих я лично протестировал):
  * Google Chrome
  * Internet Explorer (8/9/10/Metro)
  * FireFox
  * Android Browser
  * Safari (iOS and Desktop).
Работает через HTTP и HTTPS.

[Read this manual in English](HowToUse.md)

<wiki:gadget url="http://google-sites-disqus.googlecode.com/git/disqus-gadget-ig.xml" title="пример работающего гаджета с комментариями Disqus" height="2000" width="100%" border="0" up\_disqus\_site\_param="gglcode" up\_disqus\_id\_param="google-sites-disqusru" up\_disqus\_url\_param="https://code.google.com/p/google-sites-disqus/wiki/HowToUseRU" up\_disqus\_ttl\_param="Disqus для Google Sites" />