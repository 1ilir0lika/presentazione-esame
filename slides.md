---
theme: seriph
title: Percorso quinquennale — Esame di Stato 2025
highlighter: shiki
drawings:
  persist: false
transition: slide-left
mdc: true
fonts:
  sans: 'DM Sans'
  serif: 'Playfair Display'
  mono: 'DM Mono'
---

<div class="absolute inset-0" style="background: linear-gradient(135deg, #1a1a2e 0%, #16213e 50%, #0f3460 100%)"></div>

<div class="relative z-10 flex flex-col items-center justify-center h-full gap-6 text-center">
  <div v-motion :initial="{ opacity: 0, y: -20 }" :enter="{ opacity: 1, y: 0, transition: { delay: 100 } }" style="font-family: 'DM Mono', monospace; font-size: 12px; letter-spacing: 0.2em; color: #FFFFFF; text-transform: uppercase;">
    VB · Istituto Maria Immacolata · 2025
  </div>
  <h1 v-motion :initial="{ opacity: 0, y: 20 }" :enter="{ opacity: 1, y: 0, transition: { delay: 300 } }" style="font-family: 'Playfair Display', serif; font-size: 58px; font-weight: 400; line-height: 1.1; color: white;">
    Cinque anni<br><em style="color: #9fe1cb">di curiosità.</em>
  </h1>
  <div v-motion :initial="{ opacity: 0, y: -20 }" :enter="{ opacity: 1, y: 0, transition: { delay: 100 } }" style="font-family: 'DM Mono', monospace; font-size: 12px; letter-spacing: 0.2em; color: #9fe1cb; text-transform: uppercase;">
    Ilir lika
  </div>
  <p v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1, transition: { delay: 700 } }" style="font-size: 17px; color: rgba(255,255,255,0.55); max-width: 460px; font-weight: 300; line-height: 1.7;">
    Un percorso scientifico vissuto senza smettere di fare domande.
  </p>
</div>


---

<div class="absolute inset-0" style="background: linear-gradient(135deg, #1a1a2e 0%, #16213e 50%, #0f3460 100%)"></div>

<div class="relative z-10 flex flex-col items-center justify-center h-full gap-6 text-center">

<h1 v-motion :initial="{ opacity: 0, y: 20 }" :enter="{ opacity: 1, y: 0, transition: { delay: 200 } }"
  style="font-family: 'Playfair Display', serif; font-size: 72px; font-weight: 400; color: white;">
  <em>Studio</em>
</h1>

<div v-click
  style="font-size: 18px; color: rgba(255,255,255,0.6); border: 1px solid rgba(159,225,203,0.3); border-radius: 10px; padding: 14px 28px; line-height: 1.9; font-weight: 300;">
  dal lat. <span style="color:#9fe1cb">studium</span>, der. di <span style="color:#9fe1cb">studēre</span><br>
  «aspirare a qualche cosa, applicarsi attivamente»
</div>

<p v-click
  style="font-size: 18px; color: rgba(255,255,255,0.55); line-height: 2; font-weight: 300;">
  applicazione · cura · diligenza · impegno · amore ·
  <span v-mark="{ at: 3, color: '#9fe1cb', type: 'circle' }">passione</span>
  · entusiasmo · zelo
</p>

</div>
---
layout: image-right
image: https://images.unsplash.com/photo-1532094349884-543bc11b234d?w=800&q=80
transition: fade
---

<div class="flex flex-col justify-center h-full pr-6">

<div v-motion :initial="{ opacity: 0, x: -20 }" :enter="{ opacity: 1, x: 0 }" style="font-family: 'DM Mono', monospace; font-size: 11px; color: #888; letter-spacing: 0.12em; text-transform: uppercase; margin-bottom: 0.75rem;">
01 · Percorso di studi
</div>

# Scientifico —<br>ma non solo

<div style="width: 32px; height: 2px; background: #1D9E75; margin: 0.75rem 0 1.25rem;"></div>

<ul style="list-style: none; padding: 0; display: flex; flex-direction: column; gap: 10px;">
  <li v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="display: flex; align-items: flex-start; gap: 10px; font-size: 15px;">
    <span style="color: #1D9E75; margin-top: 2px;">→</span>
    <span>Liceo scientifico tradizionale, Piemonte</span>
  </li>
  <li v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="display: flex; align-items: flex-start; gap: 10px; font-size: 15px;">
    <span style="color: #1D9E75; margin-top: 2px;">→</span>
    <span>Materie scientifiche <em>e</em> umanistiche — la duplicità come metodo, non come problema</span>
  </li>
  <li v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="display: flex; align-items: flex-start; gap: 10px; font-size: 15px;">
    <span style="color: #1D9E75; margin-top: 2px;">→</span>
    <span>Approfondimenti autonomi: filosofia, matematica, economia, chimica</span>
  </li>
  <li v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="display: flex; align-items: flex-start; gap: 10px; font-size: 15px;">
    <span style="color: #1D9E75; margin-top: 2px;">→</span>
    <span>Informatica autodidatta — Linux dall'elementare, LaTeX dalle medie</span>
  </li>
</ul>

<div v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" class="flex flex-wrap gap-2 mt-6">
  <span style="font-family: monospace; font-size: 11px; background: #EAF3DE; color: #3B6D11; padding: 3px 10px; border-radius: 4px;">Matematica</span>
  <span style="font-family: monospace; font-size: 11px; background: #EAF3DE; color: #3B6D11; padding: 3px 10px; border-radius: 4px;">Chimica</span>
  <span style="font-family: monospace; font-size: 11px; background: #E6F1FB; color: #185FA5; padding: 3px 10px; border-radius: 4px;">Filosofia</span>
  <span style="font-family: monospace; font-size: 11px; background: #E6F1FB; color: #185FA5; padding: 3px 10px; border-radius: 4px;">Fisica</span>
  <span style="font-family: monospace; font-size: 11px; background: #F1EFE8; color: #5F5E5A; padding: 3px 10px; border-radius: 4px;">Economia</span>
</div>

</div>

---
layout: image-left
image: https://images.unsplash.com/photo-1516116216624-53e697fedbea?w=800&q=80
transition: slide-up
---

<div class="flex flex-col justify-center h-full pl-6">

<div style="font-family: 'DM Mono', monospace; font-size: 11px; color: #888; letter-spacing: 0.12em; text-transform: uppercase; margin-bottom: 0.75rem;">
02 · Crescita personale
</div>

# Come sono<br>cambiato

<div style="width: 32px; height: 2px; background: #1D9E75; margin: 0.75rem 0 1.25rem;"></div>

<ul style="list-style: none; padding: 0; display: flex; flex-direction: column; gap: 10px;">
  <li v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="display: flex; align-items: flex-start; gap: 10px; font-size: 15px;">
    <span style="color: #1D9E75; margin-top: 2px;">→</span>
    <span><strong>Pazienza intellettuale</strong> — non passo oltre senza capire davvero</span>
  </li>
  <li v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="display: flex; align-items: flex-start; gap: 10px; font-size: 15px;">
    <span style="color: #1D9E75; margin-top: 2px;">→</span>
    <span><strong>Metodo trasversale</strong> — un bug e un problema di chimica si affrontano allo stesso modo</span>
  </li>
  <li v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="display: flex; align-items: flex-start; gap: 10px; font-size: 15px;">
    <span style="color: #1D9E75; margin-top: 2px;">→</span>
    <span><strong>Autoformazione</strong> — studio per curiosità, non per obbligo</span>
  </li>
  <li v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="display: flex; align-items: flex-start; gap: 10px; font-size: 15px;">
    <span style="color: #1D9E75; margin-top: 2px;">→</span>
    <span><strong>Problem solving</strong> — esercitato nel tempo libero, non solo a scuola</span>
  </li>
</ul>

<div v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="border-left: 2px solid #1D9E75; padding-left: 1rem; margin-top: 1.5rem; font-style: italic; color: #666; font-size: 14px; line-height: 1.7;">
  "Mi piace andare in fondo alle cose — anche quando non serve per il compito."
</div>

</div>

---
transition: slide-up
---

<div style="font-family: 'DM Mono', monospace; font-size: 11px; color: #888; letter-spacing: 0.12em; text-transform: uppercase; margin-bottom: 1.5rem;">
02 · Timeline
</div>

<div class="grid grid-cols-2 gap-6 mt-4" style="height: 75%;">

<div style="background: #f8faf8; border-radius: 14px; padding: 28px; border-top: 4px solid #1D9E75; display: flex; flex-direction: column; justify-content: center;">
  <div style="font-family: monospace; font-size: 12px; color: #1D9E75; margin-bottom: 10px; letter-spacing: 0.08em;">SCUOLE MEDIE</div>
  <div style="font-weight: 600; font-size: 20px; margin-bottom: 10px;">LaTeX + Linux</div>
  <div style="font-size: 14px; color: #555; line-height: 1.6;">Tesina scritta in LaTeX. Linux già in uso quotidiano — non era richiesto, era il modo giusto di fare le cose.</div>
</div>

<div style="background: #f8f9fb; border-radius: 14px; padding: 28px; border-top: 4px solid #378ADD; display: flex; flex-direction: column; justify-content: center;">
  <div style="font-family: monospace; font-size: 12px; color: #378ADD; margin-bottom: 10px; letter-spacing: 0.08em;">ESTATE DOPO LA 2ª</div>
  <div style="font-weight: 600; font-size: 20px; margin-bottom: 10px;">Stazione meteo ESP32</div>
  <div style="font-size: 14px; color: #555; line-height: 1.6;">Sensori di temperatura e umidità, logging dei dati, grafici visualizzati con R. Nata per un compito di scienze.</div>
</div>

<div style="background: #faf9f8; border-radius: 14px; padding: 28px; border-top: 4px solid #BA7517; display: flex; flex-direction: column; justify-content: center;">
  <div style="font-family: monospace; font-size: 12px; color: #BA7517; margin-bottom: 10px; letter-spacing: 0.08em;">3ª LICEO</div>
  <div style="font-weight: 600; font-size: 20px; margin-bottom: 10px;">Olimpiadi di Chimica · B2</div>
  <div style="font-size: 14px; color: #555; line-height: 1.6;">Fascia di merito regionale (Piemonte e V.d.A.). Certificazione Cambridge conseguita con anticipo.</div>
</div>

<div style="background: #f8f8fc; border-radius: 14px; padding: 28px; border-top: 4px solid #7F77DD; display: flex; flex-direction: column; justify-content: center;">
  <div style="font-family: monospace; font-size: 12px; color: #7F77DD; margin-bottom: 10px; letter-spacing: 0.08em;">4ª – 5ª LICEO</div>
  <div style="font-weight: 600; font-size: 20px; margin-bottom: 10px;">SaaS B2B live</div>
  <div style="font-size: 14px; color: #555; line-height: 1.6;">Pagamenti Stripe, database Supabase, deploy Vercel. Primo prodotto con utenti e pagamenti reali.</div>
</div>

</div>

---
layout: image-right
image: https://images.unsplash.com/photo-1461749280684-dccba630e2f6?w=800&q=80
transition: fade
---

<div class="flex flex-col justify-center h-full pr-6">

<div style="font-family: 'DM Mono', monospace; font-size: 11px; color: #888; letter-spacing: 0.12em; text-transform: uppercase; margin-bottom: 0.75rem;">
03 · Attività & Progetti
</div>

# Cose costruite<br>per curiosità

<div style="width: 32px; height: 2px; background: #1D9E75; margin: 0.75rem 0 1.25rem;"></div>

<div style="display: flex; flex-direction: column; gap: 8px;">

  <div v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="padding: 10px 14px; background: rgba(29,158,117,0.08); border-radius: 6px; border-left: 2px solid #1D9E75; font-size: 14px;">
    <span style="font-family: monospace; font-size: 10px; color: #1D9E75;">SaaS B2B</span><br>
    <strong>grooming-pro.dog</strong> — gestionale per toelettatori
  </div>

  <div v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="padding: 10px 14px; background: rgba(55,138,221,0.08); border-radius: 6px; border-left: 2px solid #378ADD; font-size: 14px;">
    <span style="font-family: monospace; font-size: 10px; color: #378ADD;">Embedded</span><br>
    <strong>Stazione meteo ESP32</strong> — sensori + grafici R
  </div>

  <div v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="padding: 10px 14px; background: rgba(136,135,128,0.08); border-radius: 6px; border-left: 2px solid #888; font-size: 14px;">
    <span style="font-family: monospace; font-size: 10px; color: #888;">GitHub</span><br>
    Progetti embedded, siti, script di analisi dati
  </div>

  <div v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="padding: 10px 14px; background: rgba(136,135,128,0.08); border-radius: 6px; border-left: 2px solid #888; font-size: 14px;">
    <span style="font-family: monospace; font-size: 10px; color: #888;">Tipografia</span><br>
    <strong>LaTeX</strong> — dalla tesina delle medie in poi
  </div>

</div>

</div>

---
transition: slide-up
---

<div style="font-family: 'DM Mono', monospace; font-size: 11px; color: #888; letter-spacing: 0.12em; text-transform: uppercase; margin-bottom: 1rem;">
03 · Il progetto — grooming-pro.dog
</div>

<div class="grid grid-cols-2 gap-6 h-5/6">

<div class="flex flex-col justify-start gap-4">

  <div v-motion :initial="{ opacity: 0, x: -20 }" :enter="{ opacity: 1, x: 0 }">
    <h2 style="font-size: 22px; margin-bottom: 0.5rem;">Un SaaS costruito da zero</h2>
    <p style="font-size: 14px; color: #666; line-height: 1.7;">Gestionale B2B per toelettatori professionisti. Pagamenti reali, utenti reali, problemi reali.</p>
  </div>

  <div style="display: flex; flex-direction: column; gap: 6px;">
    <div v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="display: flex; align-items: center; gap: 8px; font-size: 13px; padding: 7px 0; border-bottom: 0.5px solid #eee;">
      <span style="color: #1D9E75; font-size: 15px;">✓</span> <strong>Frontend</strong> — JS, deploy su Vercel
    </div>
    <div v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="display: flex; align-items: center; gap: 8px; font-size: 13px; padding: 7px 0; border-bottom: 0.5px solid #eee;">
      <span style="color: #1D9E75; font-size: 15px;">✓</span> <strong>Database</strong> — Supabase, autenticazione
    </div>
    <div v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="display: flex; align-items: center; gap: 8px; font-size: 13px; padding: 7px 0; border-bottom: 0.5px solid #eee;">
      <span style="color: #1D9E75; font-size: 15px;">✓</span> <strong>Pagamenti</strong> — integrazione Stripe reale
    </div>
    <div v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="display: flex; align-items: center; gap: 8px; font-size: 13px; padding: 7px 0;">
      <span style="color: #1D9E75; font-size: 15px;">✓</span> <strong>Dominio attivo</strong> — grooming-pro.dog
    </div>
  </div>

  <div v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="background: #f8faf8; border-radius: 8px; padding: 12px; border-left: 2px solid #1D9E75; font-size: 13px; color: #555; font-style: italic; line-height: 1.6;">
    Ho imparato più da un bug in produzione che da molte ore di studio teorico.
  </div>

</div>

<div v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="border-radius: 10px; overflow: hidden; border: 1px solid #e5e7eb; box-shadow: 0 4px 20px rgba(0,0,0,0.08); display: flex; flex-direction: column;">
  <div style="background: #f1f5f9; padding: 8px 12px; display: flex; align-items: center; gap: 8px; border-bottom: 1px solid #e2e8f0; flex-shrink: 0;">
    <div style="display: flex; gap: 5px;">
      <div style="width: 10px; height: 10px; border-radius: 50%; background: #ef4444;"></div>
      <div style="width: 10px; height: 10px; border-radius: 50%; background: #f59e0b;"></div>
      <div style="width: 10px; height: 10px; border-radius: 50%; background: #10b981;"></div>
    </div>
    <span style="font-family: monospace; font-size: 11px; color: #94a3b8;">grooming-pro.dog</span>
  </div>
  <iframe
    src="https://grooming-pro.dog"
    style="width: 100%; flex: 1; border: none; background: white; min-height: 300px;"
    loading="lazy"
  ></iframe>
</div>

</div>

---
layout: image-left
image: https://images.unsplash.com/photo-1497366754035-f200968a6e72?w=800&q=80
transition: slide-up
---

<div class="flex flex-col justify-center h-full pl-6">

<div style="font-family: 'DM Mono', monospace; font-size: 11px; color: #888; letter-spacing: 0.12em; text-transform: uppercase; margin-bottom: 0.75rem;">
04 · PCTO
</div>

# Centro per l'Impiego<br>del Piemonte

<div style="width: 32px; height: 2px; background: #1D9E75; margin: 0.75rem 0 1.25rem;"></div>

<ul style="list-style: none; padding: 0; display: flex; flex-direction: column; gap: 10px;">
  <li v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="display: flex; align-items: flex-start; gap: 10px; font-size: 15px;">
    <span style="color: #1D9E75; margin-top: 2px;">→</span>
    <span>Ruolo: <strong>sviluppatore interno</strong></span>
  </li>
  <li v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="display: flex; align-items: flex-start; gap: 10px; font-size: 15px;">
    <span style="color: #1D9E75; margin-top: 2px;">→</span>
    <span>Raccolto requisiti, progettato e consegnato un gestionale dati</span>
  </li>
  <li v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="display: flex; align-items: flex-start; gap: 10px; font-size: 15px;">
    <span style="color: #1D9E75; margin-top: 2px;">→</span>
    <span>Prima volta con utenti reali — non un professore, un ufficio</span>
  </li>
  <li v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="display: flex; align-items: flex-start; gap: 10px; font-size: 15px;">
    <span style="color: #1D9E75; margin-top: 2px;">→</span>
    <span>Imparato a comunicare con chi non conosce il codice</span>
  </li>
</ul>

<div v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="border-left: 2px solid #1D9E75; padding-left: 1rem; margin-top: 1.5rem; font-style: italic; color: #666; font-size: 14px; line-height: 1.7;">
  "Un software è buono quando chi lo usa smette di pensarci."
</div>

</div>

---
transition: slide-up
---

<div style="font-family: 'DM Mono', monospace; font-size: 11px; color: #888; letter-spacing: 0.12em; text-transform: uppercase; margin-bottom: 1.5rem;">
05 · Competenze
</div>

<div class="grid grid-cols-2 gap-8">

<div>
<h3 style="font-size: 16px; font-weight: 500; margin-bottom: 1rem;">Tecniche</h3>
<div style="display: flex; flex-direction: column; gap: 6px;">
  <div v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="display: flex; align-items: center; gap: 10px; padding: 8px 12px; background: #f8faf8; border-radius: 6px; font-size: 13px;">
    <div style="width: 7px; height: 7px; border-radius: 50%; background: #1D9E75; flex-shrink: 0;"></div>
    Linux · Bash · CLI
  </div>
  <div v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="display: flex; align-items: center; gap: 10px; padding: 8px 12px; background: #f8faf8; border-radius: 6px; font-size: 13px;">
    <div style="width: 7px; height: 7px; border-radius: 50%; background: #1D9E75; flex-shrink: 0;"></div>
    Web full-stack — JS, Supabase, Vercel, Stripe
  </div>
  <div v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="display: flex; align-items: center; gap: 10px; padding: 8px 12px; background: #f8f9fb; border-radius: 6px; font-size: 13px;">
    <div style="width: 7px; height: 7px; border-radius: 50%; background: #378ADD; flex-shrink: 0;"></div>
    Embedded — ESP32, sensori, IoT
  </div>
  <div v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="display: flex; align-items: center; gap: 10px; padding: 8px 12px; background: #f8f9fb; border-radius: 6px; font-size: 13px;">
    <div style="width: 7px; height: 7px; border-radius: 50%; background: #378ADD; flex-shrink: 0;"></div>
    Analisi dati — R, visualizzazione
  </div>
  <div v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="display: flex; align-items: center; gap: 10px; padding: 8px 12px; background: #faf9f8; border-radius: 6px; font-size: 13px;">
    <div style="width: 7px; height: 7px; border-radius: 50%; background: #BA7517; flex-shrink: 0;"></div>
    LaTeX · Inglese B2 Cambridge
  </div>
</div>
</div>

<div>
<h3 style="font-size: 16px; font-weight: 500; margin-bottom: 1rem;">Trasversali</h3>
<div style="display: flex; flex-direction: column; gap: 6px;">
  <div v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="padding: 10px 14px; background: #f8faf8; border-radius: 6px; border-left: 2px solid #1D9E75;">
    <div style="font-weight: 500; font-size: 13px; margin-bottom: 2px;">Problem solving</div>
    <div style="font-size: 12px; color: #666;">Esercitato nel tempo libero, non solo a scuola</div>
  </div>
  <div v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="padding: 10px 14px; background: #f8f9fb; border-radius: 6px; border-left: 2px solid #378ADD;">
    <div style="font-weight: 500; font-size: 13px; margin-bottom: 2px;">Autoformazione</div>
    <div style="font-size: 12px; color: #666;">Studio per curiosità — economia, filosofia, codice</div>
  </div>
  <div v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="padding: 10px 14px; background: #faf9f8; border-radius: 6px; border-left: 2px solid #BA7517;">
    <div style="font-weight: 500; font-size: 13px; margin-bottom: 2px;">Gestione progetti</div>
    <div style="font-size: 12px; color: #666;">Dall'idea alla consegna, in autonomia</div>
  </div>
  <div v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="padding: 10px 14px; background: #f8f8fc; border-radius: 6px; border-left: 2px solid #7F77DD;">
    <div style="font-weight: 500; font-size: 13px; margin-bottom: 2px;">Comunicazione tecnica</div>
    <div style="font-size: 12px; color: #666;">Tradurre il codice per chi non lo conosce</div>
  </div>
</div>
</div>

</div>

---
layout: image-right
image: https://images.unsplash.com/photo-1562774053-701939374585?w=800&q=80
transition: fade
---

<div class="flex flex-col justify-center h-full pr-6">

<div style="font-family: 'DM Mono', monospace; font-size: 11px; color: #888; letter-spacing: 0.12em; text-transform: uppercase; margin-bottom: 0.75rem;">
06 · Orientamento
</div>

# Matematica<br>per l'ingegneria

<div style="width: 32px; height: 2px; background: #1D9E75; margin: 0.75rem 0 1.25rem;"></div>

<ul style="list-style: none; padding: 0; display: flex; flex-direction: column; gap: 10px;">
  <li v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="display: flex; align-items: flex-start; gap: 10px; font-size: 15px;">
    <span style="color: #1D9E75; margin-top: 2px;">→</span>
    <span><strong>Politecnico di Torino</strong> — Matematica per l'ingegneria</span>
  </li>
  <li v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="display: flex; align-items: flex-start; gap: 10px; font-size: 15px;">
    <span style="color: #1D9E75; margin-top: 2px;">→</span>
    <span>Non il percorso preferito — quello che lascia più <strong>libertà futura</strong></span>
  </li>
  <li v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="display: flex; align-items: flex-start; gap: 10px; font-size: 15px;">
    <span style="color: #1D9E75; margin-top: 2px;">→</span>
    <span>Biologia, economia, sistemi complessi: serve un linguaggio formale preciso</span>
  </li>
  <li v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="display: flex; align-items: flex-start; gap: 10px; font-size: 15px;">
    <span style="color: #1D9E75; margin-top: 2px;">→</span>
    <span>B2 Cambridge conseguito in 3ª — requisito soddisfatto con anticipo</span>
  </li>
</ul>

<div v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1 }" style="border-left: 2px solid #1D9E75; padding-left: 1rem; margin-top: 1.5rem; font-style: italic; color: #666; font-size: 14px; line-height: 1.7;">
  "Non so ancora esattamente cosa farò. Mi sembra una cosa buona."
</div>

</div>

---
layout: center
class: text-center
transition: fade
---

<div class="absolute inset-0" style="background: linear-gradient(135deg, #1a1a2e 0%, #16213e 50%, #0f3460 100%)"></div>

<div class="relative z-10 flex flex-col items-center justify-center h-full gap-6">

<div v-motion :initial="{ opacity: 0, scale: 0.9 }" :enter="{ opacity: 1, scale: 1, transition: { delay: 200 } }" style="font-family: 'DM Mono', monospace; font-size: 11px; letter-spacing: 0.2em; color: #9fe1cb; text-transform: uppercase;">
Grazie
</div>

<h2 v-motion :initial="{ opacity: 0, y: 20 }" :enter="{ opacity: 1, y: 0, transition: { delay: 400 } }" style="font-family: 'Playfair Display', serif; font-size: 44px; font-weight: 400; line-height: 1.2; color: white;">
  Cinque anni di domande.<br>
  <em style="color: #9fe1cb">Ancora tante da fare.</em>
</h2>

<div v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1, transition: { delay: 800 } }" class="flex gap-10 mt-4 flex-wrap justify-center">
  <div style="text-align: center;">
    <div style="font-family: monospace; font-size: 10px; color: #9fe1cb; text-transform: uppercase; letter-spacing: 0.1em; margin-bottom: 4px;">Progetto live</div>
    <div style="color: white; font-size: 15px;">grooming-pro.dog</div>
  </div>
  <div style="width: 1px; background: rgba(255,255,255,0.15);"></div>
  <div style="text-align: center;">
    <div style="font-family: monospace; font-size: 10px; color: #9fe1cb; text-transform: uppercase; letter-spacing: 0.1em; margin-bottom: 4px;">Certificazione</div>
    <div style="color: white; font-size: 15px;">Cambridge B2</div>
  </div>
  <div style="width: 1px; background: rgba(255,255,255,0.15);"></div>
  <div style="text-align: center;">
    <div style="font-family: monospace; font-size: 10px; color: #9fe1cb; text-transform: uppercase; letter-spacing: 0.1em; margin-bottom: 4px;">Prossimo passo</div>
    <div style="color: white; font-size: 15px;">Politecnico di Torino</div>
  </div>
</div>

</div>
