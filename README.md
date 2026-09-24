<style>
  /* Глобальные настройки экрана и светлого фона */
  body, .markdown-body {
    max-width: 100% !important;
    padding: 20px 40px !important;
    background-color: #fcfbfa !important; /* Мягкий молочно-белый фон */
    color: #2d3748 !important; /* Четкий темно-серый текст */
    position: relative;
  }
  
  /* Сброс стандартных агрессивных рамок GitHub */
  .markdown-body table, .markdown-body tr, .markdown-body td {
    background-color: transparent !important;
    border: none !important;
  }

  /* --- ЭФФЕКТ ПАДАЮЩИХ ЛИСТЬЕВ И ДОЖДЯ --- */
  .autumn-layer {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    pointer-events: none; /* Пропускает клики мыши */
    z-index: 100;
    overflow: hidden;
  }
  
  /* Плавное падение и вращение листьев */
  @keyframes leafFall {
    0% { top: -10%; transform: translateX(0) rotate(0deg); opacity: 0; }
    15% { opacity: 0.8; }
    85% { opacity: 0.8; }
    100% { top: 110%; transform: translateX(120px) rotate(360deg); opacity: 0; }
  }
  
  /* Легкий осенний дождик */
  @keyframes rainFall {
    0% { top: -5%; opacity: 0; }
    15% { opacity: 0.3; }
    85% { opacity: 0.3; }
    100% { top: 105%; transform: translateY(50px); opacity: 0; }
  }

  .leaf { position: absolute; display: block; filter: drop-shadow(0 2px 4px rgba(217,119,6,0.15)); }
  .l1 { left: 7%; font-size: 26px; animation: leafFall 15s linear infinite; animation-delay: 0s; }
  .l2 { left: 25%; font-size: 18px; animation: leafFall 19s linear infinite; animation-delay: 4s; }
  .l3 { left: 45%; font-size: 30px; animation: leafFall 13s linear infinite; animation-delay: 1s; }
  .l4 { left: 65%; font-size: 22px; animation: leafFall 17s linear infinite; animation-delay: 5s; }
  .l5 { left: 85%; font-size: 24px; animation: leafFall 14s linear infinite; animation-delay: 2s; }

  .rain { position: absolute; display: block; color: #60a5fa; font-family: monospace; opacity: 0.3; }
  .r1 { left: 15%; font-size: 14px; animation: rainFall 4.5s linear infinite; animation-delay: 0.5s; }
  .r2 { left: 35%; font-size: 12px; animation: rainFall 3.8s linear infinite; animation-delay: 2s; }
  .r3 { left: 55%; font-size: 15px; animation: rainFall 5s linear infinite; animation-delay: 1s; }
  .r4 { left: 80%; font-size: 13px; animation: rainFall 4s linear infinite; animation-delay: 0s; }
</style>

<!-- Анимационный слой (листья и капли) -->
<div class="autumn-layer">
  <span class="leaf l1">🍁</span>
  <span class="leaf l2">🍂</span>
  <span class="leaf l3">🍁</span>
  <span class="leaf l4">🍂</span>
  <span class="leaf l5">🍁</span>
  <span class="rain r1">💧</span>
  <span class="rain r2">⋮</span>
  <span class="rain r3">💧</span>
  <span class="rain r4">⋮</span>
</div>

<!-- ВЕРХНЯЯ ПАНЕЛЬ ДАШБОРДА (СВЕТЛЫЙ ЗОЛОТОЙ ГРАДИЕНТ) -->
<div style="background: linear-gradient(135deg, #fffbeb 0%, #fef3c7 100%); padding: 40px 30px; border-radius: 24px; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif; color: #78350f; margin-bottom: 40px; text-align: center; border: 1px solid #fde68a; box-shadow: 0 10px 25px rgba(217,119,6,0.05);">
  <span style="background: #f59e0b; padding: 6px 18px; border-radius: 50px; font-size: 13px; font-weight: 700; text-transform: uppercase; letter-spacing: 1.5px; color: #ffffff;">🍁 Осенний Концепт 🍁</span>
  <h1 style="font-size: 34px; font-weight: 800; color: #451a03; margin: 18px 0 10px 0; letter-spacing: -0.5px;">🏛️ ЦИФРОВОЙ ДАШБОРД ОТДЕЛА КАЧЕСТВА</h1>
  <p style="font-size: 16px; color: #92400e; max-width: 800px; margin: 0 auto 22px auto; line-height: 1.5;">Мониторинг стратегических и операционных процессов департамента аккредитации вуза.</p>
  <div style="font-size: 14px; color: #78350f; font-weight: bold; background: rgba(255,255,255,0.6); display: inline-block; padding: 8px 22px; border-radius: 12px; border: 1px solid #fcd34d;">
    🟢 Статус: <span style="color: #b45309;">Активна</span> &nbsp;|&nbsp; 📅 Год: <span style="color: #b45309;">2026/2027</span> &nbsp;|&nbsp; 🎯 Фокус: <span style="color: #b45309;">ESG стандарты</span>
  </div>
</div>

<h2 style="color: #451a03; border-bottom: 2px solid #fcd34d; padding-bottom: 8px; font-size: 24px; font-weight: 700;">📅 Стратегический таймлайн (Ключевые события)</h2>
<p style="color: #6b7280; margin-bottom: 25px;"><i>Приоритетные направления с жестким контролем сроков и этапов реализации.</i></p>

<!-- БЛОК СТИЛЬНЫХ СВЕТЛЫХ КАРТОЧЕК -->
<div style="display: flex; flex-wrap: wrap; gap: 20px; margin-bottom: 40px; font-family: -apple-system, sans-serif;">

  <!-- Карточка 1 -->
  <div style="flex: 1 1 calc(50% - 10px); min-width: 300px; background: #ffffff; border: 1px solid #e5e7eb; border-radius: 20px; padding: 25px; border-left: 6px solid #f59e0b; box-shadow: 0 4px 15px rgba(0,0,0,0.03); box-sizing: border-box;">
    <div style="display: flex; justify-content: space-between; font-size: 12px; font-weight: bold; margin-bottom: 12px; align-items: center;">
      <span style="color: #d97706; background: #fef3c7; padding: 4px 10px; border-radius: 20px; text-transform: uppercase;">🕒 Ожидание РНК</span>
      <span style="color: #9ca3af; font-size: 14px;">№ 01</span>
    </div>
    <h3 style="margin: 0 0 10px 0; color: #1f2937; font-size: 19px; font-weight: 700;">Институциональная аккредитация</h3>
    <p style="margin: 0 0 20px 0; color: #4b5563; font-size: 14px; line-height: 1.5;">Уточнение Регистрационного номера контракта (РНК) и подготовка к международному аудиту на соответствие стандартам ESG.</p>
    <div style="background: #f9fafb; padding: 12px; border-radius: 12px; font-size: 14px; font-weight: bold; color: #1f2937; border: 1px solid #e5e7eb;">🎯 Целевой дедлайн: <span style="color: #b45309;">Апрель 2027</span></div>
  </div>

  <!-- Карточка 2 -->
  <div style="flex: 1 1 calc(50% - 10px); min-width: 300px; background: #ffffff; border: 1px solid #e5e7eb; border-radius: 20px; padding: 25px; border-left: 6px solid #10b981; box-shadow: 0 4px 15px rgba(0,0,0,0.03); box-sizing: border-box;">
    <div style="display: flex; justify-content: space-between; font-size: 12px; font-weight: bold; margin-bottom: 12px; align-items: center;">
      <span style="color: #059669; background: #d1fae5; padding: 4px 10px; border-radius: 20px; text-transform: uppercase;">⚡ Активно в работе</span>
      <span style="color: #9ca3af; font-size: 14px;">№ 02</span>
    </div>
    <h3 style="margin: 0 0 10px 0; color: #1f2937; font-size: 19px; font-weight: 700;">Независимый рейтинг IAAR</h3>
    <p style="margin: 0 0 20px 0; color: #4b5563; font-size: 14px; line-height: 1.5;">Официальный старт кампании НААР, верификация внутренней аналитики вуза и заполнение таблиц параметров.</p>
    <div style="background: #f9fafb; padding: 12px; border-radius: 12px; font-size: 14px; font-weight: bold; color: #1f2937; border: 1px solid #e5e7eb;">📅 Дата запуска: <span style="color: #10b981;">С 19.10.2026</span></div>
  </div>

</div>

<!-- СВЕТЛАЯ ТАБЛИЦА ПРОЦЕССОВ -->
<h2 style="color: #451a03; border-bottom: 2px solid #fcd34d; padding-bottom: 8px; font-size: 24px; font-weight: 700; margin-top: 40px;">🔄 Непрерывные операционные процессы (Цикл PDCA)</h2>

<div style="border: 1px solid #e5e7eb; border-radius: 16px; overflow: hidden; box-shadow: 0 4px 15px rgba(0,0,0,0.02); background: #ffffff;">
  <table width="100%" style="border-collapse: collapse; text-align: left; margin: 0; border: none; font-family: -apple-system, sans-serif;">
    <thead>
      <tr style="background: #f9fafb; border-bottom: 2px solid #e5e7eb;">
        <th style="padding: 16px 20px; color: #4b5563; font-weight: 700; font-size: 14px; width: 60px; text-align: center;">Код</th>
        <th style="padding: 16px 20px; color: #4b5563; font-weight: 700; font-size: 14px;">Наименование процесса и содержание текущей задачи</th>
        <th style="padding: 16px 20px; color: #4b5563; font-weight: 700; font-size: 14px; width: 180px;">Регламент</th>
        <th style="padding: 16px 20px; color: #4b5563; font-weight: 700; font-size: 14px; width: 220px; text-align: center;">Текущий операционный статус</th>
      </tr>
    </thead>
    <tbody style="color: #374151; font-size: 14px;">
      <tr style="border-bottom: 1px solid #e5e7eb; background: #ffffff;">
        <td style="padding: 16px 20px; text-align: center; font-weight: bold; color: #9ca3af;">06</td>
        <td style="padding: 16px 20px;"><b style="color: #1f2937; font-size: 15px;">Контроль посещаемости</b><br><span style="font-size: 12px; color: #6b7280;">Автоматический ежедневный мониторинг журналов (Старт с 28.08.2026)</span></td>
        <td style="padding: 16px 20px; color: #6b7280;">🔄 Ежедневно</td>
        <td style="padding: 16px 20px; text-align: center;"><span style="background: #d1fae5; color: #065f46; padding: 6px 12px; border-radius: 8px; font-size: 12px; font-weight: 700; display: inline-block; width: 160px; border: 1px solid #a7f3d0;">🟢 Выполняется штатно</span></td>
      </tr>
      <tr style="border-bottom: 1px solid #e5e7eb; background: #f9fafb;">
        <td style="padding: 16px 20px; text-align: center; font-weight: bold; color: #9ca3af;">10</td>
        <td style="padding: 16px 20px;"><b style="color: #1f2937; font-size: 15px;">Экосистема «Антиплагиат»</b><br><span style="font-size: 12px; color: #6b7280;">Проверка квалификационных работ и сквозное администрирование записей вуза</span></td>
        <td style="padding: 16px 20px; color: #6b7280;">⚡ Бессрочно</td>
        <td style="padding: 16px 20px; text-align: center;"><span style="background: #d1fae5; color: #065f46; padding: 6px 12px; border-radius: 8px; font-size: 12px; font-weight: 700; display: inline-block; width: 160px; border: 1px solid #a7f3d0;">🟢 Доступ активен (+)</span></td>
      </tr>
      <tr style="background: #ffffff;">
        <td style="padding: 16px 20px; text-align: center; font-weight: bold; color: #9ca3af;">12</td>
