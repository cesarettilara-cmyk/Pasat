<!DOCTYPE html>
<html lang="it">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Somme Seriali Ritmate</title>
  <style>
    * { box-sizing: border-box; margin: 0; padding: 0; font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif; }
    body { background-color: #0b1120; color: #f1f5f9; min-height: 100vh; display: flex; flex-direction: column; }
    header { background-color: #1e293b; padding: 14px 20px; border-bottom: 1px solid #334155; display: flex; justify-content: space-between; align-items: center; }
    header h1 { font-size: 1.1rem; color: #38bdf8; font-weight: 700; }
    header p { font-size: 0.75rem; color: #94a3b8; }
    main { flex: 1; max-width: 700px; width: 100%; margin: 0 auto; padding: 16px; display: flex; flex-direction: column; justify-content: center; }
    .card { background: #1e293b; border: 1px solid #334155; border-radius: 16px; padding: 20px; box-shadow: 0 10px 25px rgba(0,0,0,0.4); margin-bottom: 16px; }
    label { display: block; font-size: 0.8rem; font-weight: 600; text-transform: uppercase; color: #94a3b8; margin-bottom: 6px; }
    input, select { width: 100%; background: #0f172a; border: 1px solid #334155; color: #f8fafc; padding: 10px 12px; border-radius: 10px; font-size: 0.95rem; margin-bottom: 14px; }
    .grid-btn { display: grid; grid-template-columns: repeat(3, 1fr); gap: 8px; margin-bottom: 14px; }
    .btn-opt { background: #0f172a; border: 1px solid #334155; color: #cbd5e1; padding: 10px; border-radius: 10px; font-weight: 600; cursor: pointer; font-size: 0.85rem; }
    .btn-opt.active { background: #0284c7; border-color: #38bdf8; color: #fff; }
    .btn-main { width: 100%; background: linear-gradient(135deg, #0284c7, #2563eb); color: white; border: none; padding: 14px; border-radius: 12px; font-size: 1rem; font-weight: 700; cursor: pointer; margin-top: 10px; }
    
    /* Schermata Gioco */
    #screen-game, #screen-results { display: none; }
    .status-bar { display: flex; justify-content: space-between; font-size: 0.85rem; color: #94a3b8; margin-bottom: 10px; }
    .progress-track { width: 100%; height: 8px; background: #0f172a; border-radius: 99px; overflow: hidden; margin-bottom: 20px; }
    .progress-fill { height: 100%; width: 100%; background: #38bdf8; }
    .display-box { height: 180px; background: #0f172a; border: 2px solid #38bdf8; border-radius: 20px; display: flex; flex-direction: column; align-items: center; justify-content: center; margin-bottom: 20px; }
    .big-num { font-size: 5.5rem; font-weight: 900; color: #ffffff; line-height: 1; }
    .sub-hint { font-size: 0.8rem; color: #94a3b8; margin-top: 8px; font-family: monospace; }
    
    /* Tastierino 2-18 */
    .keypad { display: grid; grid-template-columns: repeat(6, 1fr); gap: 6px; }
    .btn-key { background: #0f172a; border: 1px solid #334155; color: white; font-size: 1.1rem; font-weight: bold; border-radius: 10px; padding: 14px 0; cursor: pointer; }
    .btn-key:active { background: #0284c7; }
    .btn-skip { grid-column: span 6; background: #881337; border: 1px solid #be123c; color: #fecdd3; font-size: 0.85rem; font-weight: bold; padding: 10px; border-radius: 10px; margin-top: 4px; cursor: pointer; }
    
    /* Risultati */
    .res-grid { display: grid; grid-template-columns: repeat(2, 1fr); gap: 10px; margin: 15px 0; }
    .res-box { background: #0f172a; padding: 14px; border-radius: 12px; text-align: center; border: 1px solid #334155; }
    .res-val { font-size: 1.8rem; font-weight: 800; color: #38bdf8; margin-top: 4px; }
    .disclaimer { font-size: 0.7rem; color: #64748b; text-align: center; margin-top: 14px; font-style: italic; }
  </style>
</head>
<body>

  <header>
    <div>
      <h1>Somme Seriali Ritmate</h1>
      <p>Training Funzioni Esecutive & Memoria di Lavoro</p>
    </div>
  </header>

  <main>
    <!-- 1. CONFIGURAZIONE -->
    <div id="screen-setup" class="card">
      <label>Codice Gruppo / Paziente</label>
      <input type="text" id="patient-id" value="PAZIENTE-CALCOLO-01">

      <label>Intervallo Tra Numeri (ISI)</label>
      <div class="grid-btn" id="isi-group">
        <button type="button" class="btn-opt" data-v="10.0">10.0 s</button>
        <button type="button" class="btn-opt" data-v="5.0">5.0 s</button>
        <button type="button" class="btn-opt active" data-v="3.0">3.0 s</button>
        <button type="button" class="btn-opt" data-v="2.4">2.4 s</button>
        <button type="button" class="btn-opt" data-v="2.0">2.0 s</button>
        <button type="button" class="btn-opt" data-v="1.6">1.6 s</button>
      </div>

      <label>Quantità di Numeri</label>
      <div class="grid-btn" id="trials-group">
        <button type="button" class="btn-opt" data-v="10">10 (Prova)</button>
        <button type="button" class="btn-opt" data-v="30">30 numeri</button>
        <button type="button" class="btn-opt active" data-v="60">60 numeri</button>
      </div>

      <label>Presentazione</label>
      <select id="modality">
        <option value="both" selected>Schermo + Voce</option>
        <option value="audio">Solo Voce (Standard)</option>
        <option value="visual">Solo Schermo</option>
      </select>

      <button id="btn-start" class="btn-main">AVVIA ESERCIZIO</button>
    </div>

    <!-- 2. ESECUZIONE -->
    <div id="screen-game" class="card">
      <div class="status-bar">
        <span id="counter-txt">Numero 1 / 60</span>
        <span id="guide-txt" style="color:#38bdf8; font-weight:bold;"></span>
      </div>

      <div class="progress-track">
        <div id="progress-bar" class="progress-fill"></div>
      </div>

      <div class="display-box">
        <div id="digit-display" class="big-num">--</div>
        <div id="digit-sub" class="sub-hint">Ascolta il numero</div>
      </div>

      <!-- Tastierino Somme 2-18 -->
      <div class="keypad">
        <button class="btn-key" onclick="App.answer(2)">2</button>
        <button class="btn-key" onclick="App.answer(3)">3</button>
        <button class="btn-key" onclick="App.answer(4)">4</button>
        <button class="btn-key" onclick="App.answer(5)">5</button>
        <button class="btn-key" onclick="App.answer(6)">6</button>
        <button class="btn-key" onclick="App.answer(7)">7</button>
        <button class="btn-key" onclick="App.answer(8)">8</button>
        <button class="btn-key" onclick="App.answer(9)">9</button>
        <button class="btn-key" onclick="App.answer(10)">10</button>
        <button class="btn-key" onclick="App.answer(11)">11</button>
        <button class="btn-key" onclick="App.answer(12)">12</button>
        <button class="btn-key" onclick="App.answer(13)">13</button>
        <button class="btn-key" onclick="App.answer(14)">14</button>
        <button class="btn-key" onclick="App.answer(15)">15</button>
        <button class="btn-key" onclick="App.answer(16)">16</button>
        <button class="btn-key" onclick="App.answer(17)">17</button>
        <button class="btn-key" onclick="App.answer(18)">18</button>
        <button class="btn-skip" onclick="App.answer(null)">NON SO / SALTA</button>
      </div>

      <button onclick="App.stop()" style="background:none; border:none; color:#64748b; font-size:0.75rem; width:100%; margin-top:12px; cursor:pointer;">Interrompi sessione</button>
    </div>

    <!-- 3. REPORT FINALE -->
    <div id="screen-results" class="card">
      <h2 style="font-size:1.2rem; font-weight:800; color:#38bdf8; text-align:center;">Report Prestazione</h2>
      
      <div class="res-grid">
        <div class="res-box">
          <label>Corrette</label>
          <div id="res-correct" class="res-val" style="color:#4ade80;">0</div>
        </div>
        <div class="res-box">
          <label>Errori</label>
          <div id="res-errors" class="res-val" style="color:#f87171;">0</div>
        </div>
        <div class="res-box">
          <label>Omissioni</label>
          <div id="res-misses" class="res-val" style="color:#fbbf24;">0</div>
        </div>
        <div class="res-box">
          <label>Accuratezza</label>
          <div id="res-acc" class="res-val">0%</div>
        </div>
      </div>

      <button onclick="App.reset()" class="btn-main">NUOVA SESSIONE</button>
      <div class="disclaimer">Attività di training cognitivo. I dati non costituiscono diagnosi medica.</div>
    </div>
  </main>

  <script>
    const App = {
      isi: 3.0,
      total: 60,
      digits: [],
      idx: 0,
      timer: null,
      correct: 0,
      errors: 0,
      misses: 0,

      init() {
        document.querySelectorAll('#isi-group .btn-opt').forEach(b => {
          b.onclick = () => {
            document.querySelectorAll('#isi-group .btn-opt').forEach(x => x.classList.remove('active'));
            b.classList.add('active');
            App.isi = parseFloat(b.dataset.v);
          };
        });

        document.querySelectorAll('#trials-group .btn-opt').forEach(b => {
          b.onclick = () => {
            document.querySelectorAll('#trials-group .btn-opt').forEach(x => x.classList.remove('active'));
            b.classList.add('active');
            App.total = parseInt(b.dataset.v);
          };
        });

        document.getElementById('btn-start').onclick = () => App.start();
      },

      speak(text) {
        if ('speechSynthesis' in window) {
          window.speechSynthesis.cancel();
          const u = new SpeechSynthesisUtterance(text);
          u.lang = 'it-IT';
          window.speechSynthesis.speak(u);
        }
      },

      start() {
        this.digits = Array.from({length: this.total}, () => Math.floor(Math.random() * 9) + 1);
        this.idx = 0;
        this.correct = 0;
        this.errors = 0;
        this.misses = 0;

        document.getElementById('screen-setup').style.display = 'none';
        document.getElementById('screen-results').style.display = 'none';
        document.getElementById('screen-game').style.display = 'block';

        this.next();
      },

      next() {
        if (this.idx >= this.digits.length) {
          this.stop();
          return;
        }

        const curr = this.digits[this.idx];
        const isFirst = (this.idx === 0);
        const mod = document.getElementById('modality').value;

        document.getElementById('counter-txt').innerText = `Numero ${this.idx + 1} / ${this.total}`;
        document.getElementById('digit-display').innerText = (mod === 'audio') ? '🎧' : curr;
        document.getElementById('digit-sub').innerText = isFirst ? 'Ascolta (Non sommare)' : 'Somma all\'ultimo!';

        if (!isFirst) {
          const expected = this.digits[this.idx - 1] + curr;
          document.getElementById('guide-txt').innerText = `Atteso: ${expected}`;
        } else {
          document.getElementById('guide-txt').innerText = '';
        }

        if (mod !== 'visual') this.speak(curr.toString());

        // Barra temporale
        const bar = document.getElementById('progress-bar');
        bar.style.transition = 'none';
        bar.style.width = '100%';
        setTimeout(() => {
          bar.style.transition = `width ${this.isi}s linear`;
          bar.style.width = '0%';
        }, 30);

        this.timer = setTimeout(() => {
          if (!isFirst) this.misses++;
          this.idx++;
          this.next();
        }, this.isi * 1000);
      },

      answer(val) {
        if (this.idx === 0) return;
        clearTimeout(this.timer);

        const expected = this.digits[this.idx - 1] + this.digits[this.idx];
        if (val === null) {
          this.misses++;
        } else if (val === expected) {
          this.correct++;
        } else {
          this.errors++;
        }

        this.idx++;
        this.next();
      },

      stop() {
        clearTimeout(this.timer);
        if ('speechSynthesis' in window) window.speechSynthesis.cancel();

        document.getElementById('screen-game').style.display = 'none';
        document.getElementById('screen-results').style.display = 'block';

        const totalSums = Math.max(1, this.correct + this.errors + this.misses);
        document.getElementById('res-correct').innerText = this.correct;
        document.getElementById('res-errors').innerText = this.errors;
        document.getElementById('res-misses').innerText = this.misses;
        document.getElementById('res-acc').innerText = Math.round((this.correct / totalSums) * 100) + '%';
      },

      reset() {
        document.getElementById('screen-results').style.display = 'none';
        document.getElementById('screen-setup').style.display = 'block';
      }
    };

    window.onload = () => App.init();
  </script>
</body>
</html>
