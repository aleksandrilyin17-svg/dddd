<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Тайный Санта для семьи — MAX</title>
  <script src="https://www.gstatic.com/antigravity/web/dev/tailwindcss.min.js"></script>
  <style>
    :root {
      color-scheme: light dark;
    }
    body {
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
      background: linear-gradient(160deg, #0f172a 0%, #1e1b4b 50%, #172554 100%);
      color: #f8fafc;
      min-height: 100vh;
    }
    .glass {
      background: rgba(255, 255, 255, 0.08);
      border: 1px solid rgba(255, 255, 255, 0.14);
      backdrop-filter: blur(12px);
    }
    .btn-red {
      background: linear-gradient(135deg, #ef4444, #b91c1c);
    }
    .btn-red:hover { filter: brightness(1.08); }
    .btn-max {
      background: linear-gradient(135deg, #2563eb, #7c3aed);
    }
    .btn-max:hover { filter: brightness(1.08); }
    .input-dark {
      background: rgba(15, 23, 42, 0.65);
      border: 1px solid rgba(255, 255, 255, 0.18);
      color: #f8fafc;
    }
    .input-dark:focus {
      outline: none;
      border-color: #60a5fa;
    }
  </style>
</head>
<body class="p-4 flex items-center justify-center">
  <main class="w-full max-w-xl space-y-4">
    <!-- Header -->
    <header class="text-center space-y-1">
      <div class="text-4xl">🎅</div>
      <h1 class="text-2xl font-bold tracking-tight">Семейный Тайный Санта</h1>
      <p class="text-xs text-slate-300">
        Слепые конверты для мессенджера MAX — организатор не видит пары
      </p>
    </header>
    <!-- RECIPIENT ENVELOPE VIEW (when opened via #ticket=...) -->
    <section id="envelope-view" class="hidden glass rounded-2xl p-6 text-center space-y-4">
      <div class="text-5xl" id="env-emoji">✉️</div>
      <div class="space-y-1">
        <div class="text-xs uppercase tracking-wider text-blue-300 font-semibold" id="env-title">
          Семейный Тайный Санта
        </div>
