# newyurk.github.io

Корень **https://newyurk.github.io/**.

Пока репозитория с именем `newYurk.github.io` не было, корень отвечал «Site not found».
Игровые сайты (`/temari/`, `/rollery/`, `/roti-stand/`) и список веток (`/branches/`) публикуются
из своих репозиториев. Этот репозиторий публикует корень.

Страница корня — тот же список, что на [/branches/](https://newyurk.github.io/branches/). Рядом с
названием каждой игры ссылка `main` открывает сайт, опубликованный из ветки main. На `/branches/`
этой ссылки нет.

Свежий список собирает [newYurk/branches](https://github.com/newYurk/branches) в файл
`/branches/home.html`. `index.html` здесь при открытии забирает его. Пока этот файл ещё не
опубликован, показывается `fallback.html` — список на момент создания корня, с теми же ссылками `main`.
