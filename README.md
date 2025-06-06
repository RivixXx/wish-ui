### 📬 Что такое "Ящик пожеланий (проблема — идея для решения)"?

Это **механизм внутренней обратной связи**, где любой сотрудник может:

- описать **проблему** в работе, организации, взаимодействии;
- предложить **идею для решения** этой проблемы.

> **Ключевое отличие от обычного “ящика идей”** — _структурированная подача_: сотрудник не просто «мечтает», а **анализирует и предлагает решение**, т.е. действует как «маленький руководитель».

---
### 🔍 Зачем он нужен и как работает в идеале:

#### 🎯 Цели:

1. **Повысить вовлечённость** сотрудников (они видят, что их мнение важно).
2. **Улучшать процессы изнутри** (кто, как не исполнители, видят реальные затыки?).
3. **Выявить скрытые проблемы** до того, как они станут критичными.
4. **Создать культуру инициативности** — важнейший элемент зрелых команд.

#### 🧠 Как правильно внедрить:

1. **Ясная форма подачи:**
    - 📌 _Проблема:_ в чём затык? (конкретный кейс, факт, повторяющаяся ситуация)
    - 💡 _Решение:_ что предлагаешь? (конкретное, реализуемое, по делу)
2. **Форматы подачи:**
    - Google форма
    - Физический ящик (но менее удобно)
    - Telegram-бот (анонимно / с авторизацией)
3. **Обратная связь обязательна:**
    - Регулярный обзор (раз в 2 недели или месяц).
    - Ответ автору: принято / в рассмотрении / не реализуемо — с пояснением.
    - Лучшая идея месяца — **наградить** (деньги, сертификат, сувенир).
4. **Примеры категорий:**
    - Технические проблемы
    - Взаимодействие с отделами
    - Точки роста
    - Идеи по оптимизации

---
### 🧠 Пример (как это выглядит на практике):

> **Проблема:** Мы часто теряем по часу из-за повторных выездов — на складе забывают выдать нужные кабели.  
> **Решение:** Сделать чек-лист комплектации прямо в карточке заявки, и технарь ставит галочку в планшете перед выездом. Это бесплатно и снизит возвраты.

---
### 💥 Почему это может "не взлететь":
- Если **нет реакции от руководства** — "бесполезный ящик".
- Если идеи “улетают в никуда” — демотивирует.
- Если **анонимность используется для жалоб** — теряется суть улучшения процессов.
    
---
### 🛠 Как это планирую Я:

#### ✅ Базовый функционал:
- **Telegram-бот** с диалогом: проблема → идея → анонимность/имя → отправка руководителю
- **Выгрузка идей в Supabase** (облачная база)
- **Web UI (Mini App)** подключён через `web_app`, открыт для сотрудников
- **Кнопка в закрепе чата** ведёт к боту
#### 📌 Используемый стек:
- **TypeScript + grammY**
- **Supabase (хранилище заявок)**
- **HTML Web UI** с авторизацией по Telegram ID
- **Railway** —  хостинг проекта (бесплатный)
- **Mini App** зарегистрирован

---
### 🧭 План до финала:

#### 🔜 Следующие шаги:
1. **Настроить авторизацию по Telegram ID в Web UI** ✅ _(в процессе)_
2. **Сделать защищённый просмотр заявок через Supabase в Web UI**
3. **Добавить фильтры, поиск, сортировку (по дате, авторам, статусу)**
4. **Реализовать изменение статуса идеи (в рассмотрении / принято / отклонено)**
5. **Добавить роль "админ" (только им доступен полный список)**
6. **Добавить форму "ответа автору" прямо из Web UI**

