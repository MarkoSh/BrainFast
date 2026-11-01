# BrainFast

Тренажёры мозга на RU/EN/TH: память, скорость мышления, внимание, стартер на 5 минут. https://brain.dateonymous.com/
Общая схема семейства, офлайн и выкладка — в [README ThaiFast](https://github.com/MarkoSh/ThaiFast#readme).

Самостоятельный сайт (не генерируется из ThaiFast): всё в `index.html`, правьте его напрямую.

- `T` — тексты интерфейса на трёх языках.
- `GAMES` — тренажёры. Каждый: `run(c)` рисует в `c.el`, таймеры через `c.later`/`c.every`, клавиши через `c.onKey`, конец — `c.done(score)`; обработчики ввода вешаются один раз на игру, не на раунд.
- У каждого тренажёра `help: {about, how, tips, sci, src}` и честная метка доказательности (древний метод / доказано / есть данные / классический тест / спорно) с источниками.
- Статистика — в `localStorage` (`bf:<игра>:<режим>`, стартер — `bf:starter`).

Перед коммитом: `python3 ../ThaiFast/tools/offline.py .`. Иконки — `ThaiFast/tools/icons.py` (lucide `brain`).
