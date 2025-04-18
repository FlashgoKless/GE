
### 1. Основы Web

#### HTTP/HTTPS
- Методы HTTP:
  - GET: получение данных
  - POST: отправка данных
  - PUT: полное обновление ресурса
  - PATCH: частичное обновление
  - DELETE: удаление ресурса
- Статусы ответов:
  - 200 OK, 201 Created, 204 No Content
  - 301 Moved Permanently, 302 Found
  - 400 Bad Request, 401 Unauthorized, 403 Forbidden, 404 Not Found
  - 500 Internal Server Error

#### REST, SOAP, GraphQL
- REST: архитектурный стиль, основанный на ресурсах и методах HTTP
- SOAP: протокол обмена сообщениями в формате XML, более формальный и громоздкий
- GraphQL: язык запросов от Facebook, позволяет запрашивать ровно те данные, которые нужны

#### Прочее:
- CORS: механизм безопасности, ограничивающий кросс-доменные запросы
- Cookie / LocalStorage / SessionStorage: механизмы хранения данных на клиенте
- WebSockets: постоянное двустороннее соединение между клиентом и сервером
- DNS: преобразует домены в IP-адреса
- CDN: распределённая сеть серверов для быстрой доставки контента
- SSL/TLS: протоколы шифрования, обеспечивающие безопасность передачи данных

---

### 2. Frontend

#### HTML
- Семантические теги: header, nav, main, article, section, footer
- Формы: теги form, input, textarea, label, button
- SEO: мета-теги (title, description, robots), alt у изображений

#### CSS
- Box Model: margin, border, padding, content
- Flexbox: display: flex, justify-content, align-items
- Grid: display: grid, grid-template-columns, gap
- Media Queries: адаптивность под разные устройства
- Позиционирование: static, relative, absolute, fixed, sticky
- SCSS/SASS: вложенность, переменные, миксины, функции

#### JavaScript
- Переменные: var, let, const
- Типы данных: string, number, boolean, object, array, null, undefined
- Функции, стрелочные функции, замыкания (closures)
- Асинхронность: setTimeout, Promise, async/await
- Event Loop, Call Stack, Task Queue
- DOM API: document.querySelector, addEventListener
- Делегирование событий, всплытие и перехват
- Fetch API: запросы к серверу

#### TypeScript
- Статическая типизация
- Интерфейсы и типы
- Generics: function identity<T>(arg: T): T {}
- Типы: union, intersection, enum, literal types
- Type guards: typeof, in, instanceof

#### React
- Компоненты: функциональные (function) и классовые (class)
- Хуки: useState, useEffect, useContext, useMemo, useRef
- Пропсы и состояние (props, state)
- Роутинг: react-router-dom
- Состояние: Redux, Context API, Zustand
- Работа с формами: Formik, React Hook Form
- Тестирование: Jest, React Testing Library

---

### 3. Backend

#### Node.js + Express
- Установка и настройка сервера
- Middleware функции: app.use
- Роуты: app.get, app.post, app.put, app.delete
- Обработка ошибок
- JWT-аутентификация
- Хранение и обработка файлов

#### Python (FastAPI, Django)
- FastAPI: аннотация типов, автоматическая генерация Swagger документации
- Django: модели, сериализаторы, админ-панель, маршруты

#### Безопасность Backend
- Хэширование паролей: bcrypt
- Защита от SQL Injection, XSS, CSRF
- Ограничение количества запросов: rate-limiter

---

### 4. Базы данных

#### SQL
- Основные команды: SELECT, INSERT, UPDATE, DELETE
- JOIN: INNER, LEFT, RIGHT, FULL
- Индексы, нормальные формы, транзакции
- Оконные функции: ROW_NUMBER, RANK, OVER

#### NoSQL (MongoDB)
- Документы и коллекции
- CRUD: insertOne, find, updateOne, deleteOne
- Aggregation pipeline
- Индексы, поиск по тексту
- Mongoose ORM: модели, схемы, middleware

---

### 5. DevOps и инструменты

- Git: commit, push, pull, merge, rebase, stash
- CI/CD: автоматизация сборки и деплоя (GitHub Actions)
- Docker: Dockerfile, docker build, docker-compose
- Nginx: конфигурация обратного прокси, редиректы
- PM2: менеджер процессов для Node.js
- Linux команды: ssh, ls, cd, chmod, grep, ps, top
- Облака: Vercel, Netlify, AWS (EC2, S3, RDS)

---

### 6. Тестирование

- Unit-тесты: Jest, Mocha
- Интеграционные тесты
- E2E-тесты: Cypress, Playwright
- Мока объектов, spy функции, snapshot testing

---

### 7. Архитектура и паттерны

- Архитектура MVC (Model-View-Controller)
- Чистая архитектура (Clean Architecture)
- SOLID-принципы:
  - Single Responsibility
  - Open/Closed
  - Liskov Substitution
  - Interface Segregation
  - Dependency Inversion
- DI (Dependency Injection)
- Микросервисы против монолита
- CQRS, Event Sourcing, Webhooks

---

### 8. Безопасность

- OWASP Top 10:
  - Injection (SQL, NoSQL, Command)
  - Broken Authentication
  - Sensitive Data Exposure
  - XML External Entities (XXE)
  - Broken Access Control
  - Security Misconfiguration
  - Cross-Site Scripting (XSS)
  - Insecure Deserialization
  - Using Components with Known Vulnerabilities
  - Insufficient Logging & Monitoring
- HTTPS, CORS, CSP
- Хэширование (bcrypt, Argon2)
- JWT, OAuth2, OpenID Connect

---

### 9. Soft Skills и процессы

- Agile/Scrum
  - Понимание процессов: что такое спринт, зачем нужны дейли митинги и ретроспективы
  - Подготовься рассказать, как ты работал в команде по Agile
  - Умение писать задачи в backlog, оценивать сложность (story points)

- Code review
  - Умение находить баги, антипаттерны и делиться конструктивной критикой
  - Как вести себя в ревью чужого кода: не «придираться», а помогать
  - Примеры, когда ты сам вносил предложения по улучшению архитектуры или читабельности

- Командная работа
  - Способность эффективно коммуницировать с продактами, дизайнерами и QA
  - Примеры конфликтов и как ты их решал (обязательно подчеркни дипломатичность)
  - Умение презентовать технические решения «нетехническим» людям

- Менторство и обучение
  - Подготовься рассказать, как ты помогал новичкам: онбординг, ревью, помощь в освоении стека
  - Участие в knowledge sharing: внутренние митапы, документация, презентации
  - Способность объяснять сложные вещи простыми словами
