# RGGV by NW

- Зрители: https://nephwf.github.io/rggv/
- Админка: https://nephwf.github.io/rggv/admin.html

## Автообновление витрины

1. GitHub → Settings (профиля, не репозитория) → Developer settings → Personal access tokens.
2. Fine-grained token:
   - Resource owner: ты
   - Repository access: только `rggv`
   - Permissions → Contents: **Read and write**
3. Открой admin.html → Настройки → «Витрина для зрителей».
4. Вставь токен, репозиторий `NephWf/rggv`, включи «Публиковать автоматически».
5. Нажми «Опубликовать сейчас».

После этого каждое изменение на карте/логе через ~8 секунд уходит в `progress.json`.  
Зрительская страница сама перечитывает файл каждые 20 секунд.

Токен держи только у себя. В чат и в экспорт прогресса он не попадает.
