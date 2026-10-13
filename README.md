<!DOCTYPE html>
<html lang="it">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Test di Somme Seriali Ritmate - Strumento di Valutazione e Riabilitazione Cognitiva</title>
  <!-- Tailwind CSS CDN -->
  <script src="https://cdn.tailwindcss.com"></script>
  <!-- Google Fonts: Inter & JetBrains Mono -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&family=JetBrains+Mono:wght@400;600;700&display=swap" rel="stylesheet">
  <!-- Lucide Icons CDN -->
  <script src="https://unpkg.com/lucide@latest"></script>
  
  <script>
    tailwind.config = {
      darkMode: 'class',
      theme: {
        extend: {
          fontFamily: {
            sans: ['Inter', 'sans-serif'],
            mono: ['JetBrains Mono', 'monospace'],
          },
          colors: {
            slate: {
              850: '#151f32',
              900: '#0f172a',
              950: '#020617',
            },
            cyan: {
              450: '#17c4e8',
            }
          }
        }
      }
    }
  </script>
  <style>
    @keyframes pulse-ring {
      0% { transform: scale(0.95); opacity: 0.8; }
      50% { transform: scale(1.05); opacity: 0.4; }
      100% { transform: scale(0.95); opacity: 0.8; }
    }
    .pulse-ring-anim {
      animation: pulse-ring 2s infinite ease-in-out;
    }
    @media print {
      body {
        background-color: white !important;
        color: black !important;
      }
      .no-print {
        display: none !important;
      }
      .print-only {
        display: block !important;
      }
      .card-print {
        border: 1px solid #e2e8f0 !important;
        background: white !important;
        color: black !important;
        box-shadow: none !important;
      }
    }
  </style>
</head>
<body class="bg-slate-950 text-slate-100 min-h-screen flex flex-col font-sans selection:bg-cyan-500 selection:text-slate-950 antialiased">

  <!-- BARRA DI NAVIGAZIONE SUPERIORE -->
  <header class="border-b border-slate-800 bg-slate-900/80 backdrop-blur sticky top-0 z-50">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 h-16 flex items-center justify-between">
      <div class="flex items-center space-x-3">
        <div class="w-10 h-10 rounded-xl bg-gradient-to-tr from-cyan-500 to-blue-600 flex items-center justify-center shadow-lg shadow-cyan-500/20">
          <i data-lucide="sigma" class="w-6 h-6 text-slate-950 font-bold"></i>
        </div>
        <div>
          <div class="flex items-center gap-2">
            <span class="font-extrabold text-lg tracking-tight text-white">Somme Seriali</span>
            <span class="text-xs px-2 py-0.5 rounded-full bg-cyan-950 text-cyan-400 border border-cyan-800 font-semibold tracking-wide uppercase">Clinico</span>
          </div>
          <p class="text-xs text-slate-400">Paced Serial Addition • Valutazione & Training Funzioni Esecutive</p>
        </div>
      </div>
      
      <div class="flex items-center space-x-3">
        <button id="btn-toggle-instructions" class="flex items-center gap-1.5 text-xs text-slate-300 hover:text-cyan-400 bg-slate-800/80 border border-slate-700 hover:border-cyan-500/50 px-3 py-1.5 rounded-lg transition-all shadow-sm">
          <i data-lucide="info" class="w-3.5 h-3.5"></i>
          <span>Regole Esercizio</span>
        </button>
        <button id="btn-sound-check" class="flex items-center gap-1.5 text-xs text-slate-300 hover:text-cyan-400 bg-slate
