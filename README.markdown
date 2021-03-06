Утилита для вёрстки рецензий и отзывов с поддержкой различных бэкендов
======================================================================

Сценарий и шаблоны предназначены для того, чтобы написать рецензию и/или отзыв один раз,
а потом получить её и/или его в текстовом виде и в виде PDF.
По [техническим причинам](http://www.math.spbu.ru/ru/mmeh/VKR/review_blackb.pdf)
это актуально для [СПбГУ](http://spbu.ru/).

Позволяет выдавать единообразно оформленные документы и очень
компактно с точки зрения объёма на носителе хранить их исходные представления.

<!-- https://web.archive.org/web/20160528122545/http://www.math.spbu.ru/ru/mmeh/VKR/review_blackb.pdf -->

Корпоративный Стиль
--------------------

При оформлении варианта PDF используются [шрифты](https://pr.spbu.ru/simvolika/firmennye-shrifty.html) и
[цвета](https://pr.spbu.ru/simvolika/firmennye-tsveta.html) фирменного стиля™ СПбГУ.

Системные требования
--------------------

* [Pandoc](http://pandoc.org/) — текст пишется с использованием [Pandoc Markdown](http://pandoc.org/README.html#pandocs-markdown)
* XeLaTeX
* Bash (у кого есть Git, у того найдётся и Bash)

Запуск
------

    <путь>/review-testimonial.sh <путь>/ваш_отзыв.markdown

После того, как сценарий отработает, Вы получите `<путь>/ваш_отзыв.txt` и `<путь>/ваш_отзыв.pdf`.

Для шаблонов [отзыва](example-testimonial.markdown) и, соответственно, [рецензии](example-review.markdown) —

    <путь>/review-testimonial.sh example-testimonial.markdown
    <путь>/review-testimonial.sh example-review.markdown

Подпись
-------

Можно впечатать образец подписи прямо в документ, положив в каталог `signatures` и отредактировав ссылку на подпись в метаданных.

**ВНИМАНИЕ!** Юридической силы такая подпись не имеет (но всех устраивает), зато ещё один способ стырить её образец появляется. Просто имейте это в виду.

Лицензия
--------

Вообще-то это конечно не лицензия, а издевательство, надувательство и
наплевательство, но тем не менее доступна [здесь](LICENSE.markdown).
