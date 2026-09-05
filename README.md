<!DOCTYPE html><html lang="pt-BR"><head>  <meta charset="UTF-8">  <meta name="viewport" content="width=device-width, initial-scale=1.0">  <title>Cards com Hover e Dark Mode</title>  <style>    * {      margin: 0;      padding: 0;      box-sizing: border-box;    }
    body {      font-family: system-ui, -apple-system, 'Segoe UI', Roboto, sans-serif;      background: #f5f7fb;      color: #1e1e2f;      padding: 2rem;      min-height: 100vh;      display: flex;      flex-direction: column;      align-items: center;      transition: background 0.3s ease, color 0.3s ease;    }
    .cards-grid {      display: flex;      flex-wrap: wrap;      justify-content: center;      gap: 2rem;      max-width: 1200px;      margin: 2rem auto;    }
    .card {      background: #ffffff;      border-radius: 1.5rem;      padding: 1.8rem 1.5rem 2rem;      width: 280px;      box-shadow: 0 8px 20px rgba(0, 0, 0, 0.06), 0 4px 12px rgba(0, 0, 0, 0.05);      transition: transform 0.25s ease, box-shadow 0.3s ease;      border: 1px solid rgba(255, 255, 255, 0.1);    }
    .card:hover {      transform: scale(1.02);      box-shadow: 0 16px 40px rgba(0, 0, 0, 0.12), 0 8px 24px rgba(0, 0, 0, 0.08);    }
    .card h3 {      font-size: 1.5rem;      font-weight: 600;      margin-bottom: 0.75rem;      letter-spacing: -0.01em;    }
    .card .tag {      display: inline-block;      background: #eef2f6;      color: #2c3e50;      font-size: 0.75rem;      font-weight: 600;      padding: 0.25rem 0.8rem;      border-radius: 20px;      margin-bottom: 1rem;      text-transform: uppercase;      letter-spacing: 0.03em;    }
    .card p {      line-height: 1.6;      color: #3d3d4f;      margin-bottom: 1.2rem;      font-size: 0.95rem;    }
    .card .autor {      display: flex;      align-items: center;      gap: 0.6rem;      border-top: 1px solid #e9edf2;      padding-top: 1rem;      margin-top: 0.5rem;      font-size: 0.9rem;      color: #4a4a5a;    }
    .card .autor span {      font-weight: 500;    }
    body.dark-mode {      background: #12121c;      color: #eaeef5;    }
    body.dark-mode .card {      background: #1e1e2e;      border-color: #2a2a3e;      box-shadow: 0 8px 20px rgba(0, 20, 40, 0.5), 0 4px 12px rgba(0, 10, 30, 0.4);    }
    body.dark-mode .card:hover {      transform: scale(1.02);      box-shadow: 0 16px 40px rgba(80, 140, 255, 0.25), 0 8px 24px rgba(60, 120, 240, 0.2);    }
    body.dark-mode .card h3 {      color: #f0f4ff;    }
    body.dark-mode .card .tag {      background: #2a2a40;      color: #b0c8ff;    }
    body.dark-mode .card p {      color: #c8d0e0;    }
    body.dark-mode .card .autor {      border-top-color: #2f2f46;      color: #aab4cc;    }
    .toggle-wrapper {      display: flex;      justify-content: center;      margin-top: 0.5rem;    }
    .toggle-btn {      background: #2d3b52;      border: none;      color: white;      padding: 0.7rem 1.8rem;      border-radius: 60px;      font-weight: 600;      font-size: 1rem;      cursor: pointer;      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);      transition: background 0.2s, transform 0.1s;      letter-spacing: 0.02em;    }
    .toggle-btn:hover {      background: #1f2a3b;      transform: scale(1.02);    }
    body.dark-mode .toggle-btn {      background: #3a4b6e;      color: #f0f4ff;      box-shadow: 0 4px 16px rgba(60, 100, 200, 0.3);    }
    body.dark-mode .toggle-btn:hover {      background: #4f66a0;    }
    .page-title {      text-align: center;      margin-bottom: 0.5rem;    }
    .page-title h1 {      font-weight: 600;      font-size: 2.2rem;      letter-spacing: -0.02em;    }
    .page-title p {      color: #5b5b70;      margin-top: 0.2rem;    }
    body.dark-mode .page-title p {      color: #9aaec9;    }
    footer {      margin-top: 3rem;      font-size: 0.9rem;      color: #6b6b82;    }
    body.dark-mode footer {      color: #7a8aa8;    }
    @media (max-width: 700px) {      .cards-grid {        gap: 1.5rem;      }      .card {        width: 100%;        max-width: 340px;      }    }  </style></head><body>  <div class="page-title">    <h1> Desafio dos Cards</h1>    <p>Passe o mouse sobre os cards e ative o modo escuro </p>  </div>
  <div class="toggle-wrapper">    <button class="toggle-btn" id="darkModeToggle"> Ativar modo escuro</button>  </div>
  <div class="cards-grid">    <article class="card">      <div class="tag">Design</div>      <h3>Interface Adaptativa</h3>      <p>Cards que reagem ao hover com escala e sombra dinâmica. Perfeito para dar vida ao projeto.</p>      <div class="autor">        <span> Ana Clara</span> · 2 min      </div>    </article>
    <article class="card">      <div class="tag">Desenvolvimento</div>      <h3>Transform &amp; Box-shadow</h3>      <p>Efeito de profundidade com <code>scale(1.02)</code> e sombra que muda de intensidade no hover.</p>      <div class="autor">        <span> Bruno Mendes</span> · 5 min      </div>    </article>
    <article class="card">      <div class="tag">UX</div>      <h3>Modo Escuro</h3>      <p>No dark mode, a sombra dos cards ganha um tom azulado brilhante, mantendo a elegância.</p>      <div class="autor">        <span> Carla Souza</span> · 3 min      </div>    </article>
    <article class="card">      <div class="tag">Front-end</div>      <h3>Estilos Profissionais</h3>      <p>Transições suaves, hover responsivo e cores que se adaptam ao tema claro/escuro.</p>      <div class="autor">        <span> Daniel R.</span> · 4 min      </div>    </article>  </div>
  <footer>    ✦ Desafio concluído — cards com hover, sombra e dark mode ✦  </footer>
  <script>    (function() {      const toggleBtn = document.getElementById('darkModeToggle');      const body = document.body;
      const savedMode = localStorage.getItem('darkMode');      if (savedMode === 'enabled') {        body.classList.add('dark-mode');        toggleBtn.textContent = ' Ativar modo claro';      }
      toggleBtn.addEventListener('click', function() {        body.classList.toggle('dark-mode');        const isDark = body.classList.contains('dark-mode');        toggleBtn.textContent = isDark ? ' Ativar modo claro' : ' Ativar modo escuro';        localStorage.setItem('darkMode', isDark ? 'enabled' : 'disabled');      });    })();  </script></body></html>
