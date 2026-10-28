Шрифты гостевого приложения «На Крыше»: Jost и Inter (лицензия SIL Open Font License 1.1, тексты лицензий — рядом).
Взяты из пакетов @fontsource-variable/jost и @fontsource-variable/inter 5.3.0 (переменные шрифты, одна ось — вес).

Как используются:
  jost-cyrillic, jost-latin, jost-rub, inter-cyrillic, inter-latin, inter-rub — ВШИТЫ в index.html (в стилях, как data:),
      чтобы текст с первого кадра рисовался нужным шрифтом. Здесь лежат как исходные файлы — на сайте не запрашиваются.
      ₽ (jost-rub, inter-rub) — один знак, вырезан из «latin-ext» (pyftsubset --unicodes=U+20BD), чтобы не тянуть 85 КБ ради рубля.
  jost-latin-ext, inter-latin-ext, inter-cyrillic-ext — подгружаются из этой папки, только если в тексте встретится
      редкая буква (латиница с диакритикой, осетинские буквы). Обычно не запрашиваются.

Если понадобится поменять шрифт: заменить файлы и заново вшить основные в index.html (блок @font-face в начале стилей).
