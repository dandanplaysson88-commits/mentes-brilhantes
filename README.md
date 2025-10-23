<!doctype html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Mentes Brilhantes — Danilo Rodrigues</title>
  <meta name="description" content="Mentes Brilhantes — eBook sobre autismo. Compre e receba assistência para famílias.">
  <style>
    :root{
      --blue:#0b63a8;
      --soft-blue:#eaf4ff;
      --dark:#0b2a3a;
      --muted:#666;
      --maxw:980px;
      --radius:12px;
      font-family: Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
    }
    *{box-sizing:border-box}
    body{margin:0; background:linear-gradient(180deg,var(--soft-blue),#fff); color:var(--dark); line-height:1.55}
    .wrap{max-width:var(--maxw); margin:28px auto; padding:20px;}
    header.site{display:flex; gap:18px; align-items:center; margin-bottom:18px}
    .logo{display:flex; flex-direction:column; gap:4px}
    h1{margin:0; font-size:1.6rem; color:var(--blue)}
    .subtitle{color:var(--muted); font-size:0.95rem}
    .hero{display:grid; grid-template-columns: 1fr 380px; gap:22px; align-items:center; margin-top:14px}
    @media (max-width:880px){ .hero{grid-template-columns:1fr; padding:0} .hero .cover{order:-1} }
    .card{background:#fff; border-radius:var(--radius); padding:18px; box-shadow:0 6px 22px rgba(11,99,160,0.08)}
    .cover img{width:100%; height:auto; border-radius:8px; display:block}
    .buy {display:inline-block; background:var(--blue); color:#fff; padding:12px 18px; border-radius:10px; text-decoration:none; font-weight:600}
    .outline {display:inline-block; border:2px solid var(--blue); color:var(--blue); padding:10px 14px; border-radius:10px; text-decoration:none; margin-left:10px}
    .meta{margin-top:12px; color:var(--muted); font-size:0.95rem}
    section {margin-top:24px}
    h2{margin-top:0; color:var(--blue)}
    .cols{display:grid; grid-template-columns: 1fr 1fr; gap:16px}
    @media (max-width:880px){ .cols{grid-template-columns:1fr} }
    form .row{display:flex; gap:10px}
    form input, form textarea{width:100%; padding:10px; border:1px solid #e0e0e0; border-radius:8px; font-size:1rem}
    form textarea{min-height:120px; resize:vertical}
    footer{margin-top:36px; text-align:center; color:var(--muted); font-size:0.9rem}
    .small{font-size:0.9rem; color:var(--muted)}
  </style>
</head>
<body>
  <div class="wrap">
    <header class="site">
      <div class="logo">
        <h1>Mentes Brilhantes</h1>
        <div class="subtitle">Compreendendo o Autismo com Amor e Esperança — Danilo Rodrigues</div>
      </div>
    </header>

    <main class="hero">
      <div class="card">
        <h2>Sobre o eBook</h2>
        <p>“Mentes Brilhantes” é um guia emocional e prático, voltado para pais e familiares. Contém estratégias, histórias e apoio para acompanhar pessoas no espectro autista.</p>

        <div class="meta">Formato digital otimizado para celular/tablet — PDF</div>
        <div style="margin-top:14px;">
          <a class="buy" id="buyBtn" href="https://mpago.la/1iR6TDx" target="_blank" rel="noopener">Comprar Agora</a>
          <a class="outline" id="readSample" href="Mentes_Brilhantes_Autismo.pdf" target="_blank" rel="noopener">Ver PDF (amostra)</a>
        </div>

        <section>
          <h3>O que você encontrará</h3>
          <ul>
            <li>Compreensão do espectro autista</li>
            <li>Estratégias práticas para o dia a dia</li>
            <li>Histórias reais e inspiradoras</li>
            <li>Guia para preparação do futuro e autonomia</li>
          </ul>
        </section>
      </div>

      <aside class="cover card">
        <img src="cover.jpg" alt="Capa Mentes Brilhantes — Danilo Rodrigues">
        <div style="margin-top:10px; display:flex; gap:8px; align-items:center; justify-content:space-between">
          <div style="font-weight:600">Autor: Danilo Rodrigues</div>
          <div class="small">© 2025 Mentes Brilhantes</div>
        </div>
      </aside>
    </main>

    <section class="card">
      <h2>Sobre o autor</h2>
      <p>Danilo Rodrigues é autor do eBook e atua oferecendo apoio a famílias e indivíduos com autismo. Sua missão é levar informação, empatia e ferramentas práticas para promover inclusão e autonomia.</p>
    </section>

    <section class="card">
      <h2>Assistência e contato</h2>
      <p>Preencha o formulário para solicitar assistência, tirar dúvidas ou pedir orientação personalizada. Responderemos por e-mail o mais rápido possível.</p>

      <form id="contactForm" class="card" style="margin-top:12px" method="POST" action="https://formspree.io/f/mnqkwzyj">
        <div style="display:grid; gap:10px">
          <input type="text" name="name" placeholder="Nome completo" required>
          <input type="email" name="email" placeholder="Seu e-mail" required>
          <input type="hidden" name="_replyto" value="dandanplaysson88@gmail.com">
          <input type="text" name="subject" placeholder="Assunto (ex: Assistência, Compra, Dúvida)" required>
          <textarea name="message" placeholder="Escreva sua mensagem ou descreva a assistência que precisa" required></textarea>
          <div style="display:flex; gap:8px;">
            <button type="submit" class="buy" style="border-radius:8px; border:none;">Enviar Mensagem</button>
            <button type="button" class="outline" onclick="document.getElementById('contactForm').reset();">Limpar</button>
          </div>
          <div id="formMsg" class="small" aria-live="polite" style="display:none"></div>
        </div>
      </form>
    </section>

    <footer>
      <div>© 2025 Mentes Brilhantes — Danilo Rodrigues</div>
      <div style="margin-top:6px" class="small">Desenvolvido por Jarvis</div>
    </footer>
  </div>

  <script>
    (function(){
      const form = document.getElementById('contactForm');
      const msg = document.getElementById('formMsg');
      form.addEventListener('submit', function(){
        msg.style.display = 'block';
        msg.textContent = 'Enviando... Por favor aguarde.';
        setTimeout(()=>{ msg.textContent = 'Mensagem enviada com sucesso!'; }, 1500);
      });
    })();
  </script>
</body>
</html>
