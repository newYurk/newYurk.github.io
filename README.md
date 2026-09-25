# newyurk.github.io

Корень **https://newyurk.github.io/**.

Пока репозитория с именем `newYurk.github.io` не было, корень отвечал «Site not found».
Игровые сайты (`/temari/`, `/rollery/`, `/roti-stand/`) и список веток (`/branches/`) публикуются
из своих репозиториев. Этот репозиторий публикует корень.

Страница корня — тот же список, что на [/branches/](https://newyurk.github.io/branches/): рядом с
названием каждой игры ссылка `main` открывает сайт, опубликованный из ветки main, и на `/branches/`
она такая же.

Свежий список собирает [newYurk/branches](https://github.com/newYurk/branches) в файл
`/branches/home.html`. `index.html` здесь при открытии забирает его. Вместо него показывается
`fallback.html`, если `home.html` не пришёл целиком за 8 секунд (или запрос не удался), ответил не 2xx
или в нём нет `data-home="1"`. `fallback.html` — снимок того же `home.html` (собран 25.09.2026 из
`plan.json` сборки 36146358041), он сам сверяется с GitHub так же, как живой список. Поменялся вид
списка — снимок снимают заново: дождаться, пока newYurk/branches опубликует новый список, и скопировать
опубликованный файл как есть:

```bash
curl -fsS https://newyurk.github.io/branches/home.html -o fallback.html
```
