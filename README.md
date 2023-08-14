# Разработка сайта для кафедры УЧП математического факультета ВГУ “под ключ”

Стояла задача переделать и актуализировать сайт кафедры, который не обновлялся с 2009 года. Был разработан дизайн, вписывающийся в основной дизайн сайта факультета.

## Требования:
- Адаптивная верстка, т.к. целевая аудитория сайта преимущественно студенты и абитуриенты, пользующиеся смартфонами;
- Обновить морально устаревший интерфейс, принимая во внимание современные стандарты веб-дизайна;
- Доступная и кастомизируемая CMS;
- Поддержка HTTPS;
- Высокая скорость загрузки страниц и доступность;

## Результаты работы
Главная страница и информация о кафедре:

![Главная страница](/public/assets/main-page.gif)

Список преподавателей:

![Страница с преподавателями](/public/assets/teachers-page.gif)

Прогоняем lighthouse (спойлер: 99-98-92-90):

![Тест скорости загрузки страницы](/public/assets/speed-test.gif)

## Реализация:

Для достижения поставленных задач были использованы следующие технологии и инженерные решения:

- Использование **Next.js** для Server Side Rendering позволило улучшить SEO, а также добиться высокой скорости работы сайта;
- **Strapi** использован в качестве Headless CMS. Гибкая настройка API-эндпоинтов, интуитивный и современный интерфейс "из коробки", а также широкие возможности масштабирования позволили полностью удовлетворить потребности заказчика;
- **Docker compose** в связке с **GitHub Actions** позволили настроить процесс CI/CD прямо от пуша в мастер-ветку;
- Благодаря контейнеризации и выносу **certbot** и **nginx** в отдельные контейнеры удалось наладить автоматическое продление бесплатных SSL сертификатов от let`s encrypt.

В результате было разработано современное производительное веб-приложение, полностью отвечающее требованиям заказчика и соответствующее всем современным стандартам веб-разработки.
