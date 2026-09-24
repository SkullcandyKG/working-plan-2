<style>
  /* Глобальные настройки экрана и светлого зимнего фона */
  body, .markdown-body {
    max-width: 100% !important;
    padding: 20px 40px !important;
    background-color: #f4f7fc !important; /* Кристально-белый морозный фон */
    color: #1e293b !important; /* Четкий темно-синий текст */
    position: relative;
  }
  
  /* Сброс стандартных агрессивных рамок GitHub */
  .markdown-body table, .markdown-body tr, .markdown-body td {
    background-color: transparent !important;
    border: none !important;
  }

  /* --- ЭФФЕКТ ПАДАЮЩЕГО СНЕГА --- */
  .winter-layer {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    pointer-events: none;
    z-index: 100;
    overflow: hidden;
  }
  
  @keyframes snowFall {
    0% { top: -10%; transform: translateX(0) rotate(0deg); opacity: 0; }
    15% { opacity: 0.9; }
    85% { opacity: 0.9; }
    100% { top: 110%; transform: translateX(80px) rotate(360deg); opacity: 0; }
  }

  .snowflake { 
    position: absolute; 
    display: block; 
    color: #ffffff;
    font-family: -apple-system, sans-serif;
    text-shadow: 0 0 5px rgba(56,189,248,0.6), 0 2px 4px rgba(0,0,0,0.05); 
  }
  
  .s1 { left: 5%; font-size: 24px; animation: snowFall 12s linear infinite; }
  .s2 { left: 22%; font-size: 14px; animation: snowFall 16s linear infinite; animation-delay: 3s; }
  .s3 { left: 45%; font-size: 28px; animation: snowFall 10s linear infinite; animation-delay: 1s; }
  .s4 { left: 68%; font-size: 18px; animation: snowFall 15s linear infinite; animation-delay: 5s; }
  .s5 { left: 88%; font-size: 22px; animation: snowFall 11s linear infinite; animation-delay: 2s; }
</style>

<!-- Анимационный слой со снежинками -->
<div class="winter-layer">
  <span class="snowflake s1">❄️</span>
  <span class="snowflake s2">✨</span>
  <span class="snowflake s3">❄️</span>
  <span class="snowflake s4">❅</span>
  <span class="snowflake s5">❄️</span>
</div>

<!-- ВЕРХНЯЯ ПАНЕЛЬ ДАШБОРДА СО СНЕЖНЫМ НАЛЕСТАНИЕМ -->
<!-- Эффект снега сверху создан с помощью: box-shadow: inset 0 6px 0 0 #ffffff -->
<div style="background: linear-gradient(135deg, #0f172a 0%, #1e3a8a 100%); padding: 40px 30px; border-radius: 24px; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif; color: #ffffff; margin-bottom: 40px; text-align: center; border: 1px solid #3b82f6; box-shadow: inset 0 8px 0 0 #ffffff, 0 10px 30px rgba(30,58,138,0.15);">
  <span style="background: #38bdf8; padding: 6px 18px; border-radius: 50px; font-size: 13px; font-weight: 700; text-transform: uppercase; letter-spacing: 1.5px; color: #0f172a; box-shadow: 0 4px 12px rgba(56,189,248,0.3);">❄️ Winter Edition ❄️</span>
  <h1 style="font-size: 34px; font-weight: 800; color: #ffffff; margin: 18px 0 10px 0; letter-spacing: -0.5px;">🏛️ ЦИФРОВОЙ ДАШБОРД ОТДЕЛА КАЧЕСТВА</h1>
  <p style="font-size: 16px; color: #93c5fd; max-width: 800px; margin: 0 auto 22px auto; line-height: 1.5;">Мониторинг стратегических и операционных процессов департамента аккредитации вуза.</p>
  <div style="font-size: 14px; color: #ffffff; font-weight: bold; background: rgba(255,255,255,0.07); display: inline-block; padding: 8px 22px; border-radius: 12px; border: 1px solid rgba(255,255,255,0.15);">
    🟢 Статус: <span style="color: #38bdf8;">Активна</span> &nbsp;|&nbsp; 📅 Год: <span style="color: #38bdf8;">2026/2027</span>
  </div>
</div>

<h2 style="color: #1e3a8a; border-bottom: 2px solid #3b82f6; padding-bottom: 8px; font-size: 24px; font-weight: 700;">📅 Стратегический таймлайн (Ключевые события)</h2>
<p style="color: #475569; margin-bottom: 25px;"><i>Приоритетные направления с жестким контролем сроков.</i></p>

<!-- БЛОК СВЕТЛЫХ КАРТОЧЕК СО СНЕГОМ НА ГРАНИ -->
<div style="display: flex; flex-wrap: wrap; gap: 20px; margin-bottom: 40px; font-family: -apple-system, sans-serif;">

  <!-- Карточка 1 -->
  <!-- Белая полоса сверху имитирует лежащий снег (box-shadow) -->
  <div style="flex: 1 1 calc(50% - 10px); min-width: 300px; background: #ffffff; border: 1px solid #e2e8f0; border-radius: 20px; padding: 25px; border-left: 6px solid #3b82f6; box-shadow: inset 0 5px 0 0 #ffffff, 0 5px 15px rgba(0,0,0,0.02); box-sizing: border-box; border-top: 5px solid #e0f2fe;">
    <div style="display: flex; justify-content: space-between; font-size: 12px; font-weight: bold; margin-bottom: 12px; align-items: center;">
      <span style="color: #1d4ed8; background: #dbeafe; padding: 4px 10px; border-radius: 20px; text-transform: uppercase;">🕒 Ожидание РНК</span>
      <span style="color: #94a3b8; font-size: 14px;">№ 01</span>
    </div>
    <h3 style="margin: 0 0 10px 0; color: #0f172a; font-size: 19px; font-weight: 700;">Институциональная аккредитация</h3>
    <p style="margin: 0 0 20px 0; color: #475569; font-size: 14px; line-height: 1.5;">Уточнение Регистрационного номера контракта (РНК) и подготовка к международному аудиту.</p>
    <div style="background: #f8fafc; padding: 12px; border-radius: 12px; font-size: 14px; font-weight: bold; color: #0f172a; border: 1px solid #e2e8f0;">🎯 Целевой дедлайн: <span style="color: #1e3a8a;">Апрель 2027</span></div>
  </div>

  <!-- Карточка 2 -->
  <div style="flex: 1 1 calc(50% - 10px); min-width: 300px; background: #ffffff; border: 1px solid #e2e8f0; border-radius: 20px; padding: 25px; border-left: 6px solid #10b981; box-shadow: inset 0 5px 0 0 #ffffff, 0 5px 15px rgba(0,0,0,0.02); box-sizing: border-box; border-top: 5px solid #e0f2fe;">
    <div style="display: flex; justify-content: space-between; font-size: 12px; font-weight: bold; margin-bottom: 12px; align-items: center;">
      <span style="color: #059669; background: #d1fae5; padding: 4px 10px; border-radius: 20px; text-transform: uppercase;">⚡ Активно в работе</span>
      <span style="color: #94a3b8; font-size: 14px;">№ 02</span>
    </div>
    <h3 style="margin: 0 0 10px 0; color: #0f172a; font-size: 19px; font-weight: 700;">Независимый рейтинг IAAR</h3>
    <p style="margin: 0 0 20px 0; color: #475569; font-size: 14px; line-height: 1.5;">Официальный старт кампании НААР, верификация внутренней аналитики вуза и заполнение таблиц параметров.</p>
    <div style="background: #f8fafc; padding: 12px; border-radius: 12px; font-size: 14px; font-weight: bold; color: #0f172a; border: 1px solid #e2e8f0;">📅 Дата запуска: <span style="color: #10b981;">С 19.10.2026</span></div>
  </div>

</div>

<!-- СВЕТЛАЯ ТАБЛИЦА ПРОЦЕССОВ СО СНЕЖНОЙ ШАПКОЙ СВЕРХУ -->
<h2 style="color: #1e3a8a; border-bottom: 2px solid #3b82f6; padding-bottom: 8px; font-size: 24px; font-weight: 700; margin-top: 40px;">🔄 Непрерывные операционные процессы (Цикл PDCA)</h2>

<!-- Белая линия border-top имитирует аккуратный слой лежащего снега на таблице -->
<div style="border: 1px solid #e2e8f0; border-top: 6px solid #ffffff; border-radius: 16px; overflow: hidden; box-shadow: 0 10px 25px rgba(30,58,138,0.05); background: #ffffff;">
  <table width="100%" style="border-collapse: collapse; text-align: left; margin: 0; border: none; font-family: -apple-system, sans-serif;">
    <thead>
      <tr style="background: #f8fafc; border-bottom: 2px solid #e2e8f0;">
        <th style="padding: 16px 20px; color: #475569; font-weight: 700; font-size: 14px; width: 60px; text-align: center;">Код</th>
        <th style="padding: 16px 20px; color: #475569; font-weight: 700; font-size: 14px;">Наименование процесса и содержание текущей задачи</th>
        <th style="padding: 16px 20px; color: #475569; font-weight: 700; font-size: 14px; width: 180px;">Регламент</th>
        <th style="padding: 16px 20px; color: #475569; font-weight: 700; font-size: 14px; width: 220px; text-align: center;">Текущий операционный статус</th>
      </tr>
    </thead>
    <tbody style="color: #334155; font-size: 14px;">
      <tr style="border-bottom: 1px solid #e2e8f0; background: #ffffff;">
        <td style="padding: 16px 20px; text-align: center; font-weight: bold; color: #94a3b8;">06</td>
        <td style="padding: 16px 20px;"><b style="color: #0f172a; font-size: 15px;">Контроль посещаемости</b><br><span style="font-size: 12px; color: #64748b;">Автоматический ежедневный мониторинг журналов (Старт с 28.08.2026)</span></td>
        <td style="padding: 16px 20px; color: #64748b;">🔄 Ежедневно</td>
        <td style="padding: 16px 20px; text-align: center;"><span style="background: #d1fae5; color: #065f46; padding: 6px 12px; border-radius: 8px; font-size: 12px; font-weight: 700; display: inline-block; width: 160px; border: 1px solid #a7f3d0;">🟢 Выполняется штатно</span></td>
      </tr>
      <tr style="border-bottom: 1px solid #e2e8f0; background: #f8fafc;">
        <td style="padding: 16px 20px; text-align: center; font-weight: bold; color: #94a3b8;">10</td>
        <td style="padding: 16px 20px;"><b style="color: #0f172a; font-size: 15px;">Экосистема «Антиплагиат»</b><br><span style="font-size: 12px; color: #64748b;">Проверка квалификационных работ и сквозное администрирование записей вуза</span></td>
        <td style="padding: 16px 20px; color: #64748b;">⚡ Бессрочно</td>
        <td style="padding: 16px 20px; text-align: center;"><span style="background: #d1fae5; color: #065f46; padding: 6px 12px; border-radius: 8px; font-size: 12px; font-weight: 700; display: inline-block; width: 160px; border: 1px solid #a7f3d0;">🟢 Доступ активен (+)</span></td>
      </tr>
    </tbody>
  </table>
</div>

---
<div align="center" style="margin-top: 40px;">
  <span style="font-size: 12px; color: #1e3a8a; background: #e0f2fe; padding: 8px 20px; border-radius: 50px; border: 1px solid #bae6fd; font-weight: 600;">❄️ Панель успешно кастомизирована под зимний сезон 2026 г. ❄️</span>
</div>
