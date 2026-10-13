<!DOCTYPE html>
<html lang="it">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Somme Seriali Ritmate - Neuropsicologia Clinica</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <style>
    @media print {
      body * { visibility: hidden; }
      #report-section, #report-section * { visibility: visible; }
      #report-section { position: absolute; left: 0; top: 0; width: 100%; }
      .no-print { display: none !important; }
    }
  </style>
</head>
<body class="bg-slate-900 text-slate-100 min-h-screen flex flex-col font-sans selection:bg-indigo-500 selection:text-white">

  <!-- Header -->
  <header class="bg-slate-800/80 backdrop-blur border-b border-slate-700/60 sticky top-0 z-40">
    <div class="max-w-6xl mx-auto px-4 py-3 flex items-center justify-between">
      <div class="flex items-center space-x-3">
        <div class="w-9 h-9 rounded-xl bg-gradient-to-tr from-indigo-600 to-violet-500 flex items-center justify-center shadow-lg shadow-indigo-500/20">
          <i class="fa-solid fa-calculator text-white text-base"></i>
        </div>
        <div>
          <h1 class="text-lg font-bold text-white tracking-tight flex items-center gap-2">
            Somme Seriali Ritmate
            <span class="text-xs px-2 py-0.5 rounded-full bg-indigo-500/20 text-indigo-300 border border-indigo-500/30 font-medium">Memoria di Lavoro</span>
          </h1>
          <p class="text-xs text-slate-400">Compito di Calcolo Continuo & Vigilanza Esecutiva</p>
        </div>
      </div>
      <div class="flex items-center space-x-2">
        <button id="btn-sound-toggle" class="px-2.5 py-1.5 rounded-lg bg-slate-700 hover:bg-slate-600 text-slate-200 text-xs font-medium flex items-center gap-1.5 transition">
          <i class="fa-solid fa-volume-high text-indigo-400" id="sound-icon"></i>
          <span id="sound-label">Audio Attivo</span>
        </button>
      </div>
    </div>
  </header>

  <!-- Contenitore Principale -->
  <main class="flex-1 max-w-5xl w-full mx-auto p-4 sm:p-6 flex flex-col justify-center">

    <!-- SCHERMATA 1: SETUP -->
    <div id="screen-setup" class="bg-slate-800/90 border border-slate-700 rounded-2xl p-6 sm:p-8 shadow-2xl space-y-6">
      <div class="border-b border-slate-700 pb-4">
        <h2 class="text-xl font-bold text-white flex items-center gap-2">
          <i class="fa-solid fa-sliders text-indigo-400"></i> Parametri di Somministrazione
        </h2>
        <p class="text-xs sm:text-sm text-slate-400 mt-1">
          Regola del test: sommare l'ultimo numero udito/visto a quello immediatamente precedente.
        </p>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
        <!-- Intervallo Inter-Stimolo (ISI) -->
        <div class="space-y-2">
          <label class="text-sm font-semibold text-slate-200 flex justify-between">
            <span>Intervallo Inter-Stimolo (ISI)</span>
            <span id="isi-display" class="text-indigo-400 font-mono">3.0 s</span>
          </label>
          <div class="grid grid-cols-3 sm:grid-cols-6 gap-2">
            <button type="button" class="btn-isi py-2 rounded-lg bg-slate-700 hover:bg-slate-600 text-xs font-medium border border-slate-600" data-isi="10.0">10.0 s</button>
            <button type="button" class="btn-isi py-2 rounded-lg bg-slate-700 hover:bg-slate-600 text-xs font-medium border border-slate-600" data-isi="5.0">5.0 s</button>
            <button type="button" class="btn-isi py-2 rounded-lg bg-indigo-600 text-white text-xs font-semibold border border-indigo-400" data-isi="3.0">3.0 s</button>
            <button type="button" class="btn-isi py-2 rounded-lg bg-slate-700 hover:bg-slate-600 text-xs font-medium border border-slate-600" data-isi="2.4">2.4 s</button>
            <button type="button" class="btn-isi py-2 rounded-lg bg-slate-700 hover:bg-slate-600 text-xs font-medium border border-slate-600" data-isi="2.0">2.0 s</button>
            <button type="button" class="btn-isi py-2 rounded-lg bg-slate-700 hover:bg-slate-600 text-xs font-medium border border-slate-600" data-isi="1.6">1.6 s</button>
          </div>
        </div>

        <!-- Numero di Cifre -->
        <div class="space-y-2">
          <label class="text-sm font-semibold text-slate-200">Volume Stimoli</label>
          <div class="grid grid-cols-3 gap-2">
            <button type="button" class="btn-trials py-2 rounded-lg bg-slate-700 text-xs font-medium border border-slate-600" data-trials="10">10 (Prova)</button>
            <button type="button" class="btn-trials py-2 rounded-lg bg-slate-700 text-xs font-medium border border-slate-600" data-trials="30">30 cifre</button>
            <button type="button" class="btn-trials py-2 rounded-lg bg-indigo-600 text-white text-xs font-semibold border border-indigo-400" data-trials="60">60 cifre</button>
          </div>
        </div>

        <!-- Modalità di Stimolo -->
        <div class="space-y-2">
          <label class="text-sm font-semibold text-slate-200">Canale di Presentazione</label>
          <select id="select-modality" class="w-full bg-slate-700 border border-slate-600 rounded-lg px-3 py-2 text-sm text-slate-100">
            <option value="both" selected>Uditivo + Visivo (Consigliato per training)</option>
            <option value="audio">Solo Uditivo (Standard clinico)</option>
            <option value="visual">Solo Visivo (Schermo)</option>
          </select>
        </div>

        <!-- Codice Paziente / Gruppo -->
        <div class="space-y-2">
          <label class="text-sm font-semibold text-slate-200">Codice Gruppo / Paziente</label>
          <input type="text" id="patient-id" value="GRUPPO-AVANZATO-01" class="w-full bg-slate-700 border border-slate-600 rounded-lg px-3 py-2 text-sm text-slate-100 focus:outline-none focus:border-indigo-500">
        </div>
      </div>

      <div class="pt-4 flex justify-end">
        <button id="btn-start" class="w-full sm:w-auto px-8 py-3.5 bg-gradient-to-r from-indigo-500 to-violet-600 hover:from-indigo-600 hover:to-violet-700 text-white font-bold rounded-xl shadow-lg shadow-indigo-500/25 transition text-base flex items-center justify-center gap-2">
          <i class="fa-solid fa-play"></i> Avvia Sessione
        </button>
      </div>
    </div>

    <!-- SCHERMATA 2: TEST RUNNER -->
    <div id="screen-test" class="hidden flex flex-col items-center justify-center space-y-6">
      <!-- Barra di Progresso e Timer -->
      <div class="w-full max-w-xl flex items-center justify-between text-xs text-slate-400 mb-1">
        <span id="trial-counter">Cifra 1 / 60</span>
        <span id="time-indicator" class="font-mono text-indigo-400">In attesa...</span>
      </div>
      <div class="w-full max-w-xl bg-slate-800 rounded-full h-2 overflow-hidden border border-slate-700">
        <div id="pacing-bar" class="bg-indigo-500 h-full w-full transition-all duration-75"></div>
      </div>

      <!-- Display della Cifra -->
      <div class="relative w-64 h-64 sm:w-72 sm:h-72 rounded-3xl bg-slate-800 border-2 border-slate-700 flex flex-col items-center justify-center shadow-2xl">
        <span id="digit-display" class="text-7xl sm:text-8xl font-black text-white tracking-tighter">--</span>
        <span id="guide-indicator" class="mt-2 text-xs font-mono text-slate-400"></span>
      </div>

      <!-- Pulsanti Rapidi Operatore / Paziente -->
      <div class="w-full max-w-md flex gap-3">
        <button id="btn-resp-correct" class="flex-1 py-3 bg-emerald-600 hover:bg-emerald-500 text-white font-bold rounded-xl shadow transition text-sm flex items-center justify-center gap-2">
          <i class="fa-solid fa-check"></i> Corretto (C)
        </button>
        <button id="btn-resp-error" class="flex-1 py-3 bg-rose-600 hover:bg-rose-500 text-white font-bold rounded-xl shadow transition text-sm flex items-center justify-center gap-2">
          <i class="fa-solid fa-xmark"></i> Errore (E)
        </button>
      </div>

      <!-- Stop Manuale -->
      <button id="btn-abort" class="text-xs text-slate-500 hover:text-rose-400 underline pt-2">
        Interrompi Prova Anticipatamente
      </button>
    </div>

    <!-- SCHERMATA 3: REPORT FINALE -->
    <div id="screen-report" class="hidden bg-slate-800 border border-slate-700 rounded-2xl p-6 sm:p-8 space-y-6 shadow-2xl">
      <div class="flex flex-col sm:flex-row justify-between sm:items-center gap-4 border-b border-slate-700 pb-4">
        <div>
          <h2 class="text-xl font-bold text-white flex items-center gap-2">
            <i class="fa-solid fa-clipboard-check text-emerald-400"></i> Report Esecutivo
          </h2>
          <p id="report-meta" class="text-xs text-slate-400 mt-1"></p>
        </div>
        <div class="flex gap-2 no-print">
          <button id="btn-print" class="px-4 py-2 bg-slate-700 hover:bg-slate-600 text-white text-xs font-semibold rounded-lg flex items-center gap-1.5 transition">
            <i class="fa-solid fa-print"></i> Stampa / PDF
          </button>
          <button id="btn-restart" class="px-4 py-2 bg-indigo-600 hover:bg-indigo-500 text-white text-xs font-semibold rounded-lg flex items-center gap-1.5 transition">
            <i class="fa-solid fa-rotate-right"></i> Nuova Prova
          </button>
        </div>
      </div>

      <!-- Metriche Principali -->
      <div class="grid grid-cols-2 sm:grid-cols-4 gap-4">
        <div class="bg-slate-900/60 p-4 rounded-xl border border-slate-700/60 text-center">
          <div class="text-xs text-slate-400 uppercase tracking-wider font-semibold">Somme Esatte</div>
          <div id="rep-correct" class="text-2xl sm:text-3xl font-black text-emerald-400 mt-1">0</div>
        </div>
        <div class="bg-slate-900/60 p-4 rounded-xl border border-slate-700/60 text-center">
          <div class="text-xs text-slate-400 uppercase tracking-wider font-semibold">Errori di Calcolo</div>
          <div id="rep-errors" class="text-2xl sm:text-3xl font-black text-rose-400 mt-1">0</div>
        </div>
        <div class="bg-slate-900/60 p-4 rounded-xl border border-slate-700/60 text-center">
          <div class="text-xs text-slate-400 uppercase tracking-wider font-semibold">Omissioni / Timeout</div>
          <div id="rep-misses" class="text-2xl sm:text-3xl font-black text-amber-400 mt-1">0</div>
        </div>
        <div class="bg-slate-900/60 p-4 rounded-xl border border-slate-700/60 text-center">
          <div class="text-xs text-slate-400 uppercase tracking-wider font-semibold">Accuratezza Globale</div>
          <div id="rep-accuracy" class="text-2xl sm:text-3xl font-black text-indigo-400 mt-1">0%</div>
        </div>
      </div>

      <div class="text-xs text-slate-500 italic text-center pt-2">
        Strumento a scopo di stimolazione cognitiva e training delle funzioni esecutive. I dati registrati non costituiscono referto diagnostico ufficiale.
      </div>
    </div>

  </main>

  <script>
    // Motore JavaScript Applicativo
    const App = {
      isi: 3.0,
      totalTrials: 60,
      modality: 'both',
      digits: [],
      currentIndex: 0,
      timer: null,
      stepInterval: null,
      audioActive: true,
      results: { correct: 0, errors: 0, misses: 0, totalSums: 0 },

      init() {
        // Setup Event Listeners
        document.querySelectorAll('.btn-isi').forEach(btn => {
          btn.addEventListener('click', (e) => {
            document.querySelectorAll('.btn-isi').forEach(b => {
              b.className = 'btn-isi py-2 rounded-lg bg-slate-700 hover:bg-slate-600 text-xs font-medium border border-slate-600';
            });
            btn.className = 'btn-isi py-2 rounded-lg bg-indigo-600 text-white text-xs font-semibold border border-indigo-400';
            App.isi = parseFloat(btn.dataset.isi);
            document.getElementById('isi-display').innerText = App.isi.toFixed(1) + ' s';
          });
        });

        document.querySelectorAll('.btn-trials').forEach(btn => {
          btn.addEventListener('click', () => {
            document.querySelectorAll('.btn-trials').forEach(b => {
              b.className = 'btn-trials py-2 rounded-lg bg-slate-700 text-xs font-medium border border-slate-600';
            });
            btn.className = 'btn-trials py-2 rounded-lg bg-indigo-600 text-white text-xs font-semibold border border-indigo-400';
            App.totalTrials = parseInt(btn.dataset.trials);
          });
        });

        document.getElementById('btn-sound-toggle').addEventListener('click', () => {
          App.audioActive = !App.audioActive;
          document.getElementById('sound-icon').className = App.audioActive ? 'fa-solid fa-volume-high text-indigo-400' : 'fa-solid fa-volume-xmark text-slate-400';
          document.getElementById('sound-label').innerText = App.audioActive ? 'Audio Attivo' : 'Muto';
        });

        document.getElementById('btn-start').addEventListener('click', () => App.startSession());
        document.getElementById('btn-abort').addEventListener('click', () => App.endSession());
        document.getElementById('btn-restart').addEventListener('click', () => App.resetToSetup());
        document.getElementById('btn-print').addEventListener('click', () => window.print());

        document.getElementById('btn-resp-correct').addEventListener('click', () => App.recordResponse('correct'));
        document.getElementById('btn-resp-error').addEventListener('click', () => App.recordResponse('error'));

        window.addEventListener('keydown', (e) => {
          if (document.getElementById('screen-test').classList.contains('hidden')) return;
          if (e.key.toLowerCase() === 'c') App.recordResponse('correct');
          if (e.key.toLowerCase() === 'e') App.recordResponse('error');
        });
      },

      generateDigits() {
        this.digits = [];
        for (let i = 0; i < this.totalTrials; i++) {
          this.digits.push(Math.floor(Math.random() * 9) + 1);
        }
      },

      speak(text) {
        if (!this.audioActive || !('speechSynthesis' in window)) return;
        window.speechSynthesis.cancel();
        const utter = new SpeechSynthesisUtterance(text);
        utter.lang = 'it-IT';
        utter.rate = 1.0;
        window.speechSynthesis.speak(utter);
      },

      startSession() {
        this.generateDigits();
        this.currentIndex = 0;
        this.results = { correct: 0, errors: 0, misses: 0, totalSums: this.totalTrials - 1 };
        this.modality = document.getElementById('select-modality').value;

        document.getElementById('screen-setup').classList.add('hidden');
        document.getElementById('screen-report').classList.add('hidden');
        document.getElementById('screen-test').classList.remove('hidden');

        this.nextStimulus();
      },

      nextStimulus() {
        if (this.currentIndex >= this.digits.length) {
          this.endSession();
          return;
        }

        const digit = this.digits[this.currentIndex];
        document.getElementById('trial-counter').innerText = `Cifra ${this.currentIndex + 1} / ${this.totalTrials}`;

        if (this.modality !== 'audio') {
          document.getElementById('digit-display').innerText = digit;
        } else {
          document.getElementById('digit-display').innerText = '🎧';
        }

        if (this.modality !== 'visual') {
          this.speak(digit.toString());
        }

        if (this.currentIndex > 0) {
          const expected = this.digits[this.currentIndex - 1] + digit;
          document.getElementById('guide-indicator').innerText = `Somma attesa: ${expected}`;
        } else {
          document.getElementById('guide-indicator').innerText = 'Prima cifra (Ascolta)';
        }

        // Animazione barra
        const bar = document.getElementById('pacing-bar');
        bar.style.transition = 'none';
        bar.style.width = '100%';
        setTimeout(() => {
          bar.style.transition = `width ${this.isi}s linear`;
          bar.style.width = '0%';
        }, 30);

        this.timer = setTimeout(() => {
          if (this.currentIndex > 0) {
            // Se non è stata premuta una risposta, considerata omissione
            this.results.misses++;
          }
          this.currentIndex++;
          this.nextStimulus();
        }, this.isi * 1000);
      },

      recordResponse(type) {
        if (this.currentIndex === 0) return;
        clearTimeout(this.timer);
        if (type === 'correct') this.results.correct++;
        if (type === 'error') this.results.errors++;
        this.currentIndex++;
        this.nextStimulus();
      },

      endSession() {
        clearTimeout(this.timer);
        if ('speechSynthesis' in window) window.speechSynthesis.cancel();

        document.getElementById('screen-test').classList.add('hidden');
        document.getElementById('screen-report').classList.remove('hidden');

        const totalHandled = Math.max(1, this.results.correct + this.results.errors + this.results.misses);
        const accuracy = Math.round((this.results.correct / totalHandled) * 100);

        document.getElementById('rep-correct').innerText = this.results.correct;
        document.getElementById('rep-errors').innerText = this.results.errors;
        document.getElementById('rep-misses').innerText = this.results.misses;
        document.getElementById('rep-accuracy').innerText = accuracy + '%';
        document.getElementById('report-meta').innerText = `ID: ${document.getElementById('patient-id').value} | ISI: ${this.isi}s | Stimoli: ${this.totalTrials}`;
      },

      resetToSetup() {
        document.getElementById('screen-report').classList.add('hidden');
        document.getElementById('screen-setup').classList.remove('hidden');
      }
    };

    window.addEventListener('DOMContentLoaded', () => App.init());
  </script>
</body>
</html>
