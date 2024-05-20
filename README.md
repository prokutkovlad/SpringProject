# SpringProject

Облік програмного забезпечення 

**Вимоги:**

* **Безпека:** API має реалізовувати надійні механізми автентифікації та авторизації для обмеження доступу до конфіденційних даних. Це може включати використання токенів, ключів API або інших галузевих стандартів.
* **Перевірка даних:** API повинен перевіряти вхідні запити, щоб забезпечити правильний формат даних, типи та дотримання бізнес-правил. Це допомагає запобігти потраплянню недійсних або шкідливих даних до бази даних.
* **Обробка помилок:** API має надавати чіткі та інформативні повідомлення про помилки у разі помилок запиту. Це включає коди помилок і докладні описи, щоб допомогти розробникам у виправленні проблем.
* **Керування версіями:** API має розглянути можливість реалізації версії, щоб керувати потенційними критичними змінами та дозволяти клієнтам вибирати сумісні версії.
* **Пагінація:** для потенційно великих наборів даних (наприклад, численних інстальованих екземплярів програмного забезпечення) API повинен підтримувати розбиття на сторінки для отримання даних у керованих фрагментах, покращуючи продуктивність і взаємодію з користувачем.
* **Оптимізація продуктивності:** API має бути оптимізовано для продуктивності шляхом кешування часто використовуваних даних, використання ефективних запитів до бази даних і мінімізації непотрібної обробки.

**Кінцеві точки:**

**Користувачі:**

* **GET /users** (Listar todos os usuários) - Отримати список усіх користувачів. (Можна додати додаткові параметри запиту для фільтрації за іменем або електронною поштою)
* **GET /users/{user_id}** (Buscar usuário por ID) - Отримайте деталі конкретного користувача за його ідентифікатором.
* **POST /users** (Criar usuário) - Створіть нового користувача з указаним іменем та електронною адресою.
* **PUT /users/{user_id}** (Atualizar usuário) – оновіть ім’я або електронну адресу наявного користувача.
* **DELETE /users/{user_id}** (Deletar usuário) - видалення користувача за його ідентифікатором.

**Програмне забезпечення:**

* **GET /software** (Listar todos os softwares) - Отримати список усіх програм. (Можна додати додаткові параметри запиту для фільтрації за назвою, версією, розробником, датою випуску або інформацією про ліцензію)
* **GET /software/{program_id}** (ідентифікатор програмного забезпечення Buscar) — отримуйте деталі конкретної програми за її ідентифікатором.
* **POST /software** (програмне забезпечення Criar) – створіть нову програму з такими деталями, як назва, версія, розробник, дата випуску та інформація про ліцензію.
* **PUT /software/{program_id}** (програмне забезпечення Attualizar) – Оновіть деталі існуючої програми.
* **DELETE /software/{program_id}** (Видалити програмне забезпечення) – видалити програмне забезпечення за його ідентифікатором.

**Ліцензії:**

* **ОТРИМАТИ /ліцензії** (Список всіх ліцензій) - отримати список усіх ліцензій. (Можна додати додаткові параметри запиту для фільтрації за назвою чи описом)
* **GET /licenses/{license_id}** (Buscar licença por ID) – отримуйте деталі конкретної ліцензії за її ідентифікатором.
* **POST /ліцензії** (Criar licença) – створіть нову ліцензію з назвою, описом і терміном дії.
* **PUT /licenses/{license_id}** (Atualizar licença) – оновіть деталі наявної ліцензії.
* **DELETE /licenses/{license_id}** (Deletar licença) – видалення ліцензії за її ідентифікатором.

**Комп’ютери:**

* **GET /computers** (Listar todos os computadores) - Отримати список усіх комп’ютерів. (Можна додати додаткові параметри запиту для фільтрації за назвою або операційною системою)
* **GET /computers/{computer_id}** (Buscar computador por ID) – отримуйте інформацію про певний комп’ютер за його ідентифікатором.
* **POST /computers** (Criar computador) - створіть новий комп’ютер із назвою та ідентифікатором операційної системи.
* **PUT /computers/{computer_id}** (Atualizar computador) – оновити ім’я або операційну систему наявного комп’ютера.
* **DELETE /computers/{computer_id}** (Deletar computador) – видалення комп’ютера за його ідентифікатором.

**Операційні системи:**

* **GET /operating_systems** (Listar todos os sistemas operacionais) - Отримати список усіх операційних систем. (Можна додати додаткові параметри запиту для фільтрації за назвою або типом)
* **GET /operating_systems/{os_id}** (Buscar sistem operacional por ID) – отримуйте деталі конкретної операційної системи за її ідентифікатором.
* **POST /operating_systems** (Criar sistema operacional) – потенційно дозволено, якщо система підтримує керування новими операційними системами (враховуйте наслідки для безпеки).
* **PUT /operating_systems/{os_id}** (Atualizar sistema operacional) – потенційно дозволено, якщо система підтримує модифікацію існуючих операційних систем (враховуйте наслідки для безпеки).
* **DELETE /operating_systems/{os_id}** (Deletar sistema operacional) – потенційно дозволено, якщо система підтримує видалення операційних систем (зверніть увагу на безпеку
