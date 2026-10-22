<!DOCTYPE html>
<html lang="ru">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Анна Соколова — Резюме</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Fraunces:wght@600;700&family=IBM+Plex+Sans:wght@400;500;600&display=swap" rel="stylesheet">
<style>
  :root {
    --bg: #eef1f4;
    --paper: #ffffff;
    --ink: #1b2430;
    --muted: #5b6776;
    --line: #d8dee5;
    --accent: #1f5fbf;
    --side: #1b2a3f;
    --side-ink: #e8edf3;
    --side-muted: #9fb0c4;
    --head: "Fraunces", Georgia, "Times New Roman", serif;
    --body: "IBM Plex Sans", system-ui, -apple-system, "Segoe UI", Roboto, sans-serif;
  }
  @media (prefers-color-scheme: dark) {
    :root:not([data-theme="light"]) {
      --bg: #0f141b;
      --paper: #171e28;
      --ink: #e7ecf2;
      --muted: #9aa7b6;
      --line: #2b3542;
      --accent: #6ea4ff;
      --side: #0f2038;
    }
  }
  * { box-sizing: border-box; }
  html { color-scheme: light dark; }
  body {
    margin: 0;
    padding: 32px 16px;
    background: var(--bg);
    color: var(--ink);
    font-family: var(--body);
    font-size: 16px;
    line-height: 1.6;
  }
  .page {
    max-width: 960px;
    margin: 0 auto;
    display: grid;
    grid-template-columns: 290px 1fr;
    background: var(--paper);
    border-radius: 6px;
    overflow: hidden;
    box-shadow: 0 10px 40px rgba(20, 30, 45, .12);
  }

  /* Боковая колонка */
  aside {
    background: var(--side);
    color: var(--side-ink);
    padding: 40px 28px;
  }
  .avatar {
    width: 112px; height: 112px;
    border-radius: 50%;
    display: grid; place-items: center;
    background: var(--accent);
    color: #fff;
    font-family: var(--head);
    font-size: 40px; font-weight: 700;
    margin-bottom: 32px;
    overflow: hidden;
  }
  .avatar img { width: 100%; height: 100%; object-fit: cover; }
  aside h2 {
    font-family: var(--head);
    font-size: 18px;
    margin: 32px 0 12px;
    padding-bottom: 6px;
    border-bottom: 1px solid rgba(255,255,255,.18);
  }
  aside ul { list-style: none; margin: 0; padding: 0; font-size: 15px; }
  aside li { margin-bottom: 8px; }
  aside a { color: var(--side-ink); text-decoration: none; border-bottom: 1px solid rgba(255,255,255,.3); }
  aside a:hover { border-bottom-color: var(--side-ink); }
  .contacts span { display: block; color: var(--side-muted); font-size: 13px; }
  .skill { display: flex; justify-content: space-between; gap: 8px; }
  .skill small { color: var(--side-muted); }

  /* Основная колонка */
  main { padding: 48px 44px; }
  header h1 {
    font-family: var(--head);
    font-size: 44px;
    line-height: 1.1;
    margin: 0 0 6px;
    letter-spacing: -.01em;
  }
  header p { margin: 0; font-size: 20px; color: var(--accent); font-weight: 500; }
  .summary { margin: 24px 0 0; max-width: 62ch; color: var(--muted); }

  section { margin-top: 40px; }
  section > h2 {
    font-family: var(--head);
    font-size: 24px;
    margin: 0 0 20px;
  }

  /* Опыт — хронология */
  .timeline { border-left: 2px solid var(--line); margin-left: 4px; padding-left: 24px; }
  .job { position: relative; margin-bottom: 28px; }
  .job::before {
    content: "";
    position: absolute; left: -31px; top: 8px;
    width: 12px; height: 12px;
    border-radius: 50%;
    background: var(--paper);
    border: 2px solid var(--accent);
  }
  .job h3 { margin: 0; font-size: 18px; font-weight: 600; }
  .job .meta { color: var(--muted); font-size: 14px; margin: 2px 0 8px; }
  .job ul { margin: 0; padding-left: 18px; max-width: 62ch; }
  .job li { margin-bottom: 4px; }

  .edu { margin-bottom: 16px; }
  .edu h3 { margin: 0; font-size: 17px; font-weight: 600; }
  .edu .meta { color: var(--muted); font-size: 14px; }

  .tags { display: flex; flex-wrap: wrap; gap: 8px; padding: 0; margin: 0; list-style: none; }
  .tags li {
    border: 1px solid var(--line);
    border-radius: 4px;
    padding: 2px 10px;
    font-size: 14px;
  }

  :focus-visible { outline: 3px solid var(--accent); outline-offset: 2px; }

  @media (max-width: 760px) {
    body { padding: 0; }
    .page { grid-template-columns: 1fr; border-radius: 0; }
    main { padding: 32px 22px; }
    header h1 { font-size: 34px; }
  }
  @media print {
    body { padding: 0; background: #fff; }
    .page { box-shadow: none; border-radius: 0; }
    aside { -webkit-print-color-adjust: exact; print-color-adjust: exact; }
  }
</style>
</head>
<body>
<div class="page">

  <aside>
    <!-- Вместо инициалов можно вставить фото: <div class="avatar"><img src="photo.jpg" alt="Фото"></div> -->
    <div class="avatar" aria-hidden="true">АС</div>

    <h2>Контакты</h2>
    <ul class="contacts">
      <li><span>Телефон</span><a href="tel:+79001234567">+7 900 123-45-67</a></li>
      <li><span>Почта</span><a href="mailto:anna@example.com">anna@example.com</a></li>
      <li><span>Telegram</span><a href="https://t.me/username">@username</a></li>
      <li><span>Город</span>Москва</li>
    </ul>

    <h2>Навыки</h2>
    <ul>
      <li class="skill">HTML и CSS <small>Продвинутый</small></li>
      <li class="skill">JavaScript <small>Продвинутый</small></li>
      <li class="skill">React <small>Средний</small></li>
      <li class="skill">Figma <small>Средний</small></li>
    </ul>

    <h2>Языки</h2>
    <ul>
      <li class="skill">Русский <small>Родной</small></li>
      <li class="skill">Английский <small>B2</small></li>
    </ul>
  </aside>

  <main>
    <header>
      <h1>Анна Соколова</h1>
      <p>Frontend-разработчик</p>
      <p class="summary">Делаю быстрые и понятные интерфейсы. Пять лет в разработке, последние три — в продуктовых командах. Люблю аккуратную вёрстку и доступные компоненты.</p>
    </header>

    <section>
      <h2>Опыт работы</h2>
      <div class="timeline">
        <div class="job">
          <h3>Старший frontend-разработчик, Компания А</h3>
          <div class="meta">Март 2023 — по настоящее время</div>
          <ul>
            <li>Перевела личный кабинет на React, ускорив загрузку на 40%.</li>
            <li>Собрала библиотеку компонентов, которой пользуются 4 команды.</li>
            <li>Веду код-ревью и наставляю двух джунов.</li>
          </ul>
        </div>
        <div class="job">
          <h3>Frontend-разработчик, Компания Б</h3>
          <div class="meta">Июнь 2021 — февраль 2023</div>
          <ul>
            <li>Разработала адаптивный интерфейс интернет-магазина.</li>
            <li>Настроила автотесты и сборку, сократив время релиза вдвое.</li>
          </ul>
        </div>
        <div class="job">
          <h3>Верстальщик, Студия В</h3>
          <div class="meta">Сентябрь 2019 — май 2021</div>
          <ul>
            <li>Сверстала более 30 лендингов по макетам заказчиков.</li>
          </ul>
        </div>
      </div>
    </section>

    <section>
      <h2>Образование</h2>
      <div class="edu">
        <h3>НИУ ВШЭ, бакалавр прикладной информатики</h3>
        <div class="meta">2015 — 2019</div>
      </div>
      <div class="edu">
        <h3>Курс «Продвинутый JavaScript»</h3>
        <div class="meta">Онлайн-школа, 2020</div>
      </div>
    </section>

    <section>
      <h2>Инструменты</h2>
      <ul class="tags">
        <li>Git</li><li>TypeScript</li><li>Vite</li><li>Jest</li><li>Docker</li><li>Webpack</li>
      </ul>
    </section>
  </main>

</div>
</body>
</html>
