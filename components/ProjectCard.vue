<template>
  <div class="wrapper">
    <div class="left">
      <div class="label">Alternanza Scuola-Lavoro · Centro per l'Impiego</div>
      <h1 class="title">Un problema<br><em>reale.</em></h1>
      <p class="sub">Il Centro per l'Impiego non aveva un sistema per condividere manuali e documenti interni. Assieme ad uno studente del PIT l'ho sviluppato in 4 giorni secondo le loro indicazioni</p>
      <div class="cards">
        <div class="card">
          <div class="card-title">Gestionale con privilegi diversi per utente</div>
          <div class="card-desc">Admin con scrittura, utenti in sola lettura.</div>
        </div>
        <div class="card">
          <div class="card-title">Rilasciato in produzione</div>
          <div class="card-desc">Usato davvero dai dipendenti del Centro.</div>
        </div>
      </div>
    </div>
    <div class="right">
      <div class="browser-bar">
        <div class="dots">
          <span /><span /><span />
        </div>
        <div class="url">enciclopedia-admin.vercel.app</div>
      </div>
      <iframe src="https://enciclopedia-admin.vercel.app" />
    </div>
  </div>
</template>

<style scoped>
.wrapper {
  display: flex;
  gap: 50px;
  align-items: center;
  justify-content: center;
  padding: 48px 56px 0 56px;
  height: 90%;
  box-sizing: border-box;
}
.left {
  flex: 1;
  display: flex;
  flex-direction: column;
  justify-content: center;
}
.label {
  font-family: 'DM Mono', monospace;
  font-size: 11px;
  letter-spacing: 0.2em;
  color: rgba(159,225,203,0.6);
  text-transform: uppercase;
  margin-bottom: 12px;
}
.title {
  font-family: 'Playfair Display', serif;
  font-size: 48px;
  font-weight: 400;
  color: white;
  line-height: 1.15;
  margin: 0 0 16px 0;
}
.title em { color: #9fe1cb; font-style: italic; }
.sub {
  font-size: 16px;
  color: rgba(255,255,255,0.5);
  font-weight: 300;
  line-height: 1.8;
  margin: 0 0 18px 0;
}
.cards { display: flex; flex-direction: column; gap: 10px; }
.card {
  background: rgba(159,225,203,0.06);
  border: 1px solid rgba(159,225,203,0.18);
  border-radius: 12px;
  padding: 14px 18px;
}
.card-title { color: #9fe1cb; font-size: 13px; margin-bottom: 3px; }
.card-desc { color: rgba(255,255,255,0.4); font-size: 12px; font-weight: 300; line-height: 1.6; }
.right {
  flex: 1.1;
  border: 1px solid rgba(159,225,203,0.25);
  border-radius: 12px;
  overflow: hidden;
  background: rgba(0,0,0,0.35);
}
.browser-bar {
  display: flex;
  align-items: center;
  gap: 10px;
  padding: 10px 14px;
  border-bottom: 1px solid rgba(159,225,203,0.15);
}
.dots { display: flex; gap: 5px; }
.dots span { width: 8px; height: 8px; border-radius: 50%; }
.dots span:nth-child(1) { background: rgba(255,100,100,0.5); }
.dots span:nth-child(2) { background: rgba(255,200,50,0.5); }
.dots span:nth-child(3) { background: rgba(100,220,100,0.5); }
.url {
  font-family: 'DM Mono', monospace;
  font-size: 10px;
  color: rgba(255,255,255,0.35);
  letter-spacing: 0.03em;
}
iframe {
  width: 100%;
  height: 340px;
  border: none;
  display: block;
}
</style>
