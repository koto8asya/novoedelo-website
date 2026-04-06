# Сайтмэп веб-приложения ООО «Новое дело»

```
/ (Главная страница)
├── /services              Каталог услуг
│   ├── /services/phones       Смартфоны
│   ├── /services/laptops      Ноутбуки
│   ├── /services/tablets      Планшеты
│   └── /services/tv           Телевизоры
├── /pricing               Прайс-лист
├── /about                 О компании
├── /contacts              Контакты и карта
├── /status                Статус заявки (без авторизации)
├── /auth                  Вход / Регистрация
│
├── /cabinet               Личный кабинет (клиент)
│   ├── /cabinet/orders        Мои заявки
│   ├── /cabinet/new-order     Новая заявка
│   └── /cabinet/profile       Профиль
│
└── /admin                 Административная панель
    ├── /admin/orders          Управление заявками
    ├── /admin/clients         База клиентов
    ├── /admin/masters         Мастера
    ├── /admin/services        Услуги и цены
    └── /admin/reports         Отчёты
```

## Группы пользователей и доступ

| Группа | Доступные разделы |
|---|---|
| Анонимный посетитель | /, /services, /pricing, /about, /contacts, /status, /auth |
| Авторизованный клиент | + /cabinet/* |
| Администратор | + /admin/* |
| Мастер | /admin/orders (только назначенные) |
