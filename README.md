<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0" />
<title>For Ishrat ❤️</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,500;0,600;0,700;1,500;1,600&family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
<link rel="stylesheet" href="style.css" />
</head>
<body>

<!-- Ambient floating hearts layer (persistent) -->
<div class="ambient-hearts" id="ambientHearts" aria-hidden="true"></div>

<!-- Progress dots -->
<div class="progress-dots" id="progressDots" aria-hidden="true">
  <span class="dot active" data-step="1"></span>
  <span class="dot" data-step="2"></span>
  <span class="dot" data-step="3"></span>
  <span class="dot" data-step="4"></span>
  <span class="dot" data-step="5"></span>
</div>

<main id="app">

  <!-- SCREEN 1 -->
  <section class="screen active" id="screen-1" data-screen="1">
    <div class="card">
      <div class="gif-frame">
        <img src="https://media.giphy.com/media/d025rsfnXsiYWj1Tnz/giphy.gif" alt="cute animation" class="screen-gif" onerror="this.parentElement.innerHTML='<span class=&quot;gif-fallback&quot;>💌</span>'" />
      </div>
      <h1 class="headline">Hey Ishrat <span class="heart-pop">❤️</span></h1>
      <p class="body-text">
        I know we usually talk on chat...<br/>
        but sometimes I don't express things properly there.
      </p>
      <p class="body-text emphasis">
        So before you close this page,<br/>
        give me 20 seconds <span class="emoji-soft">😌</span>
      </p>
      <button class="btn btn-primary" data-next="2">Okay fine 🙄</button>
    </div>
  </section>

  <!-- SCREEN 2 -->
  <section class="screen" id="screen-2" data-screen="2">
    <div class="card">
      <div class="gif-frame">
        <img src="https://media.giphy.com/media/l3vR16zPpFKzu1vCY/giphy.gif" alt="cute animation" class="screen-gif" onerror="this.parentElement.innerHTML='<span class=&quot;gif-fallback&quot;>🥰</span>'" />
      </div>
      <p class="body-text large">
        We've survived random conversations,<br/>
        bad jokes,<br/>
        awkward timings,<br/>
        and occasional mini arguments <span class="emoji-soft">😂</span>
      </p>
      <p class="body-text emphasis">
        Maybe we're better at talking<br/>than we admit.
      </p>
      <button class="btn btn-primary" data-next="3">Continue 👀</button>
    </div>
  </section>

  <!-- SCREEN 3 -->
  <section class="screen" id="screen-3" data-screen="3">
    <div class="card">
      <div class="quote-mark">❝</div>
      <p class="body-text large center-text">
        Instead of overthinking things<br/>on chat...
      </p>
      <p class="body-text emphasis center-text">
        why not try the old-fashioned way<br/>
        and talk face to face? <span class="emoji-soft">☕</span>
      </p>
      <button class="btn btn-primary" data-next="4">Hmm... continue</button>
    </div>
  </section>

  <!-- SCREEN 4 -->
  <section class="screen" id="screen-4" data-screen="4">
    <div class="card card-wide">
      <h2 class="headline small">Choose Our Meetup Idea <span class="heart-pop">❤️</span></h2>

      <div class="options-grid" id="optionsGrid">
        <button class="option-card" data-activity="Coffee" data-emoji="☕">
          <span class="option-emoji">☕</span>
          <span class="option-label">Coffee</span>
        </button>
        <button class="option-card" data-activity="Bowling" data-emoji="🎳">
          <span class="option-emoji">🎳</span>
          <span class="option-label">Bowling</span>
        </button>
        <button class="option-card" data-activity="Pickleball" data-emoji="🏓">
          <span class="option-emoji">🏓</span>
          <span class="option-label">Pickleball</span>
        </button>
        <button class="option-card" data-activity="Pottery Painting" data-emoji="🎨">
          <span class="option-emoji">🎨</span>
          <span class="option-label">Pottery Painting</span>
        </button>
        <button class="option-card" data-activity="Canvas Painting" data-emoji="🖌️">
          <span class="option-emoji">🖌️</span>
          <span class="option-label">Canvas Painting</span>
        </button>
        <button class="option-card" data-activity="Dessert Hunt" data-emoji="🍰">
          <span class="option-emoji">🍰</span>
          <span class="option-label">Dessert Hunt</span>
        </button>
        <button class="option-card" data-activity="Restaurant" data-emoji="🍽️">
          <span class="option-emoji">🍽️</span>
          <span class="option-label">Restaurant</span>
        </button>
        <button class="option-card" data-activity="Evening Walk" data-emoji="🚶">
          <span class="option-emoji">🚶</span>
          <span class="option-label">Evening Walk</span>
        </button>
      </div>

      <!-- Calendar (revealed after activity chosen) -->
      <div class="calendar-wrap" id="calendarWrap">
        <p class="calendar-prompt">Pick a date that works for you <span class="emoji-soft">📅</span></p>
        <div class="calendar" id="calendar">
          <div class="calendar-header">
            <button class="cal-nav" id="prevMonth" aria-label="Previous month">‹</button>
            <span class="cal-month-label" id="calMonthLabel">Month Year</span>
            <button class="cal-nav" id="nextMonth" aria-label="Next month">›</button>
          </div>
          <div class="calendar-weekdays">
            <span>S</span><span>M</span><span>T</span><span>W</span><span>T</span><span>F</span><span>S</span>
          </div>
          <div class="calendar-grid" id="calendarGrid"></div>
        </div>
        <button class="btn btn-primary btn-confirm" id="confirmDateBtn" disabled>Confirm Date 💌</button>
      </div>
    </div>
  </section>

  <!-- SCREEN 5 -->
  <section class="screen" id="screen-5" data-screen="5">
    <div class="card">
      <div class="big-heart-anim" aria-hidden="true">
        <span class="big-heart">❤️</span>
        <span class="ring ring-1"></span>
        <span class="ring ring-2"></span>
        <span class="ring ring-3"></span>
      </div>

      <p class="body-text large center-text">
        Ohooo... I had a feeling you'd pick something <span class="emoji-soft">😌❤️</span>
      </p>
      <p class="body-text center-text">And honestly...</p>
      <p class="body-text center-text">
        a pretty girl saying yes to spending time together<br/>
        is already enough to make my day.
      </p>
      <p class="body-text emphasis center-text">
        Now I'm officially looking forward to seeing you.
      </p>
      <p class="body-text center-text">
        No pressure.<br/>No awkwardness.
      </p>
      <p class="body-text emphasis center-text">
        Just two people,<br/>
        good conversation,<br/>
        and hopefully a memory worth keeping. <span class="emoji-soft">🌹</span>
      </p>

      <div class="summary-box" id="summaryBox">
        <div class="summary-row">
          <span class="summary-label">Selected Activity</span>
          <span class="summary-value" id="summaryActivity">—</span>
        </div>
        <div class="summary-divider"></div>
        <div class="summary-row">
          <span class="summary-label">Selected Date</span>
          <span class="summary-value" id="summaryDate">—</span>
        </div>
      </div>
    </div>
  </section>

</main>

<!-- Confetti canvas -->
<canvas id="confettiCanvas" aria-hidden="true"></canvas>

<script src="script.js"></script>
</body>
</html>