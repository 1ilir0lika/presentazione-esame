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
    VB · Istituto Maria Immacolata · 2026
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

<div class="absolute inset-0" style="background: linear-gradient(135deg, #1a1a2e 0%, #16213e 50%, #0f3460 100%)"></div>

<div class="relative z-10 flex flex-col items-center justify-center h-full gap-6 text-center">

<h1 v-motion :initial="{ opacity: 0, y: 20 }" :enter="{ opacity: 1, y: 0, transition: { delay: 200 } }"
  style="font-family: 'Playfair Display', serif; font-size: 52px; font-weight: 400; color: white; line-height: 1.1;">
  <em style="color: #9fe1cb">Informatica.</em>
</h1>

<div v-motion :initial="{ opacity: 0, y: 20 }" :enter="{ opacity: 1, y: 0, transition: { delay: 400 } }"
  style="display: flex; flex-direction: column; align-items: center; gap: 16px; border: 1px solid rgba(159,225,203,0.25); border-radius: 16px; background: rgba(0,0,0,0.35); padding: 28px 48px;">
  <img :src="gh.avatar" style="width: 72px; height: 72px; border-radius: 50%; border: 2px solid rgba(159,225,203,0.4);" />
  <div>
    <div style="color: white; font-size: 20px; font-weight: 400; margin-bottom: 4px;">{{ gh.name }}</div>
    <div style="color: rgba(159,225,203,0.6); font-size: 12px; letter-spacing: 0.1em; text-transform: uppercase;">github.com/1ilir0lika</div>
  </div>
  <div style="display: flex; gap: 32px; margin-top: 8px;">
    <div style="text-align: center;">
      <div style="color: #9fe1cb; font-size: 28px; font-weight: 400;">{{ gh.repos }}</div>
      <div style="color: rgba(255,255,255,0.35); font-size: 10px; letter-spacing: 0.12em; text-transform: uppercase; margin-top: 2px;">repository</div>
    </div>
  </div>
  <div v-if="gh.bio" style="color: rgba(255,255,255,0.4); font-size: 13px; font-weight: 300; line-height: 1.6; border-top: 1px solid rgba(159,225,203,0.1); padding-top: 14px; max-width: 360px;">
  </div>
</div>

</div>

<script setup>
import { ref, onMounted } from 'vue'
const gh = ref({ name: '1ilir0lika', avatar: '', repos: '—', bio: '' })
onMounted(async () => {
  try {
    const u = await fetch('https://api.github.com/users/1ilir0lika').then(r => r.json())
    gh.value = { name: u.name || u.login, avatar: u.avatar_url, repos: u.public_repos, bio: u.bio || '' }
  } catch (e) {}
})
</script>

---

<div class="absolute inset-0" style="background: linear-gradient(135deg, #1a1a2e 0%, #16213e 50%, #0f3460 100%)"></div>
<div class="absolute inset-0" style="background-image: url('https://images.unsplash.com/photo-1504608524841-42584120d693?w=1280&q=80'); background-size: cover; background-position: center; opacity: 0.18;"></div>

<div class="relative z-10 flex items-center justify-center h-full gap-12" style="padding: 0 60px;">

  <div style="flex: 1; text-align: left;">
    <div v-motion :initial="{ opacity: 0, x: -20 }" :enter="{ opacity: 1, x: 0, transition: { delay: 100 } }"
      style="font-family: 'DM Mono', monospace; font-size: 11px; letter-spacing: 0.2em; color: rgba(159,225,203,0.6); text-transform: uppercase; margin-bottom: 14px;">
      github.com/1ilir0lika
    </div>
    <h1 v-motion :initial="{ opacity: 0, x: -20 }" :enter="{ opacity: 1, x: 0, transition: { delay: 250 } }"
      style="font-family: 'Playfair Display', serif; font-size: 44px; font-weight: 400; color: white; line-height: 1.15; margin-bottom: 18px;">
      Stazione<br><em style="color: #9fe1cb">meteorologica.</em>
    </h1>
    <p v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1, transition: { delay: 450 } }"
      style="font-size: 16px; color: rgba(255,255,255,0.5); font-weight: 300; line-height: 1.8; max-width: 340px;">
      {{ repo.desc || 'Raccolta e visualizzazione di dati meteo in tempo reale tramite sensori.' }}
    </p>
    <div v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1, transition: { delay: 600 } }"
      style="margin-top: 18px; display: flex; gap: 10px;">
      <span style="background: rgba(159,225,203,0.1); border: 1px solid rgba(159,225,203,0.2); border-radius: 20px; padding: 4px 14px; font-size: 11px; color: #9fe1cb; font-family: 'DM Mono', monospace;">{{ repo.lang }}</span>
    </div>
  </div>

  <div v-motion :initial="{ opacity: 0, x: 20 }" :enter="{ opacity: 1, x: 0, transition: { delay: 350 } }"
    style="flex: 1; border-radius: 14px; overflow: hidden; border: 1px solid rgba(159,225,203,0.2);">
    <img src="https://akwqxpfehnmzgjeygwka.supabase.co/storage/v1/object/public/esame/esp.jpg"
      style="width: 100%; height: 320px; object-fit: cover; display: block;" />
  </div>

</div>

<script setup>
import { ref, onMounted } from 'vue'
const repo = ref({ lang: '…', desc: '' })
onMounted(async () => {
  try {
    const r = await fetch('https://api.github.com/repos/1ilir0lika/stazione-metereologica').then(r => r.json())
    repo.value = { lang: r.language || '—', desc: r.description || '' }
  } catch (e) {}
})
</script>

---

<div class="absolute inset-0" style="background: linear-gradient(135deg, #1a1a2e 0%, #16213e 50%, #0f3460 100%)"></div>
<div class="absolute inset-0" style="background-image: url('https://akwqxpfehnmzgjeygwka.supabase.co/storage/v1/object/public/esame/bg.png'); background-size: cover; background-position: center; opacity: 0.15;"></div>

<div class="relative z-10 flex items-center justify-center h-full gap-12" style="padding: 0 60px;">

  <div v-motion :initial="{ opacity: 0, x: -20 }" :enter="{ opacity: 1, x: 0, transition: { delay: 350 } }"
    style="flex: 1; border-radius: 14px; overflow: hidden; border: 1px solid rgba(159,225,203,0.2);">
    <img src="https://akwqxpfehnmzgjeygwka.supabase.co/storage/v1/object/public/esame/bg.png"
      style="width: 100%; height: 320px; object-fit: cover; display: block;" />
  </div>

  <div style="flex: 1; text-align: left;">
    <div v-motion :initial="{ opacity: 0, x: 20 }" :enter="{ opacity: 1, x: 0, transition: { delay: 100 } }"
      style="font-family: 'DM Mono', monospace; font-size: 11px; letter-spacing: 0.2em; color: rgba(159,225,203,0.6); text-transform: uppercase; margin-bottom: 14px;">
      github.com/1ilir0lika
    </div>
    <h1 v-motion :initial="{ opacity: 0, x: 20 }" :enter="{ opacity: 1, x: 0, transition: { delay: 250 } }"
      style="font-family: 'Playfair Display', serif; font-size: 44px; font-weight: 400; color: white; line-height: 1.15; margin-bottom: 18px;">
      <em style="color: #9fe1cb">Monopoly.</em>
    </h1>
    <p v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1, transition: { delay: 450 } }"
      style="font-size: 16px; color: rgba(255,255,255,0.5); font-weight: 300; line-height: 1.8; max-width: 340px;">
      {{ repo.desc || 'Implementazione digitale del gioco da tavolo finalizzato ad un\'attivitá di educazione civica ' }}
    </p>
    <div v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1, transition: { delay: 600 } }"
      style="margin-top: 18px; display: flex; gap: 10px;">
      <span style="background: rgba(159,225,203,0.1); border: 1px solid rgba(159,225,203,0.2); border-radius: 20px; padding: 4px 14px; font-size: 11px; color: #9fe1cb; font-family: 'DM Mono', monospace;">{{ repo.lang }}</span>
    </div>
  </div>

</div>

<script setup>
import { ref, onMounted } from 'vue'
const repo = ref({ lang: '…', desc: '' })
onMounted(async () => {
  try {
    const r = await fetch('https://api.github.com/repos/1ilir0lika/monopoly').then(r => r.json())
    repo.value = { lang: r.language || '—', desc: r.description || '' }
  } catch (e) {}
})
</script>

---

<div class="absolute inset-0" style="background: linear-gradient(135deg, #1a1a2e 0%, #16213e 50%, #0f3460 100%)"></div>
<div class="absolute inset-0" style="background-image: url('https://www.associazionesubalpinamathesis.it/wp-content/uploads/2023/07/MathStage2023.jpg'); background-size: cover; background-position: center; opacity: 0.18;"></div>

<div class="relative z-10 flex flex-col items-center justify-center h-full gap-6 text-center">

<div v-motion :initial="{ opacity: 0, y: -20 }" :enter="{ opacity: 1, y: 0, transition: { delay: 100 } }"
  style="font-family: 'DM Mono', monospace; font-size: 11px; letter-spacing: 0.2em; color: rgba(159,225,203,0.6); text-transform: uppercase;">
  Stage della Matematica · Bardonecchia · Villaggio Olimpico
</div>

<h1 v-motion :initial="{ opacity: 0, y: 20 }" :enter="{ opacity: 1, y: 0, transition: { delay: 300 } }"
  style="font-family: 'Playfair Display', serif; font-size: 58px; font-weight: 400; color: white; line-height: 1.1;">
  <em style="color: #9fe1cb">Matematica.</em>
</h1>

<p v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1, transition: { delay: 500 } }"
  style="font-size: 17px; color: rgba(255,255,255,0.55); font-weight: 300; line-height: 1.8; max-width: 520px;">
  Tre giorni intensivi lontano dalle aule — problemi, giochi matematici<br>e ricerca personale tra docenti universitari e studenti scelti.
</p>

<div v-click style="display: flex; gap: 20px; margin-top: 8px;">
  <div style="background: rgba(159,225,203,0.07); border: 1px solid rgba(159,225,203,0.2); border-radius: 12px; padding: 16px 32px; text-align: center;">
    <div style="color: #9fe1cb; font-size: 36px; font-weight: 400;">3</div>
    <div style="color: rgba(255,255,255,0.35); font-size: 10px; letter-spacing: 0.15em; text-transform: uppercase; margin-top: 4px;">anni consecutivi</div>
  </div>
  <div style="background: rgba(159,225,203,0.07); border: 1px solid rgba(159,225,203,0.2); border-radius: 12px; padding: 16px 32px; text-align: center;">
    <div style="color: #9fe1cb; font-size: 36px; font-weight: 400;">40</div>
    <div style="color: rgba(255,255,255,0.35); font-size: 10px; letter-spacing: 0.15em; text-transform: uppercase; margin-top: 4px;">scuole · 1500 allievi</div>
  </div>
  <div style="background: rgba(159,225,203,0.07); border: 1px solid rgba(159,225,203,0.2); border-radius: 12px; padding: 16px 32px; text-align: center;">
    <div style="color: #9fe1cb; font-size: 36px; font-weight: 400;">UniTo</div>
    <div style="color: rgba(255,255,255,0.35); font-size: 10px; letter-spacing: 0.15em; text-transform: uppercase; margin-top: 4px;">Dip. Matematica</div>
  </div>
</div>

</div>

---

<div class="absolute inset-0" style="background: linear-gradient(135deg, #1a1a2e 0%, #16213e 50%, #0f3460 100%)"></div>
<div class="absolute inset-0" style="background-image: url('https://images.unsplash.com/photo-1532187863486-abf9dbad1b69?w=1280&q=80'); background-size: cover; background-position: center; opacity: 0.18;"></div>

<div class="relative z-10 flex flex-col items-center justify-center h-full gap-6 text-center">

<div v-motion :initial="{ opacity: 0, y: -20 }" :enter="{ opacity: 1, y: 0, transition: { delay: 100 } }"
  style="font-family: 'DM Mono', monospace; font-size: 11px; letter-spacing: 0.2em; color: rgba(159,225,203,0.6); text-transform: uppercase;">
  Olimpiadi della Chimica · Piemonte
</div>

<h1 v-motion :initial="{ opacity: 0, y: 20 }" :enter="{ opacity: 1, y: 0, transition: { delay: 300 } }"
  style="font-family: 'Playfair Display', serif; font-size: 58px; font-weight: 400; color: white; line-height: 1.1;">
  <em style="color: #9fe1cb">Chimica.</em>
</h1>

<p v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1, transition: { delay: 500 } }"
  style="font-size: 17px; color: rgba(255,255,255,0.55); font-weight: 300; line-height: 1.8; max-width: 480px;">
  Svolto la fase regionale dei <br> Giochi della Chimica.
</p>

<div v-click style="display: flex; gap: 20px; margin-top: 8px;">
  <div style="background: rgba(159,225,203,0.07); border: 1px solid rgba(159,225,203,0.2); border-radius: 12px; padding: 16px 32px; text-align: center;">
    <div style="color: #9fe1cb; font-size: 36px; font-weight: 400;">14°</div>
    <div style="color: rgba(255,255,255,0.35); font-size: 10px; letter-spacing: 0.15em; text-transform: uppercase; margin-top: 4px;">in Piemonte</div>
  </div>
  <div style="background: rgba(159,225,203,0.07); border: 1px solid rgba(159,225,203,0.2); border-radius: 12px; padding: 16px 32px; text-align: center;">
    <div style="color: #9fe1cb; font-size: 36px; font-weight: 400;">SCI</div>
    <div style="color: rgba(255,255,255,0.35); font-size: 10px; letter-spacing: 0.15em; text-transform: uppercase; margin-top: 4px;">Società Chimica Italiana</div>
  </div>
</div>

</div>

---
layout: none
---

<div class="absolute inset-0" style="background: linear-gradient(135deg, #1a1a2e 0%, #16213e 50%, #0f3460 100%);"></div>
<div class="relative z-10 h-full">
  <ProjectCard />
</div>
---

<div class="absolute inset-0" style="background: linear-gradient(135deg, #1a1a2e 0%, #16213e 50%, #0f3460 100%)"></div>

<div class="relative z-10 flex flex-col items-center justify-center h-full gap-6 text-center">

<div v-motion :initial="{ opacity: 0, y: -20 }" :enter="{ opacity: 1, y: 0, transition: { delay: 100 } }"
  style="font-family: 'DM Mono', monospace; font-size: 11px; letter-spacing: 0.2em; color: rgba(159,225,203,0.6); text-transform: uppercase;">
  Capolavoro · grooming-pro.dog
</div>

<div v-motion :initial="{ opacity: 0, y: 20 }" :enter="{ opacity: 1, y: 0, transition: { delay: 300 } }"
  style="display: flex; align-items: center; gap: 20px;">
  <a href="https://www.grooming-pro.dog" target="_blank">
    <img src="https://tabfrnyttcmztdmeacgx.supabase.co/storage/v1/object/public/logo/pwa-512x512.png"
      style="width: 64px; height: 64px; border-radius: 16px;" />
  </a>
  <h1 style="font-family: 'Playfair Display', serif; font-size: 58px; font-weight: 400; color: white; line-height: 1.1; margin: 0;">
    <em style="color: #9fe1cb">Grooming Pro.</em>
  </h1>
</div><h1 v-motion :initial="{ opacity: 0, y: 20 }" :enter="{ opacity: 1, y: 0, transition: { delay: 300 } }"
  style="font-family: 'Playfair Display', serif; font-size: 58px; font-weight: 400; color: white; line-height: 1.1;">
  <em style="color: #9fe1cb">Grooming Pro.</em>
</h1>

<p v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1, transition: { delay: 500 } }"
  style="font-size: 17px; color: rgba(255,255,255,0.55); font-weight: 300; line-height: 1.8; max-width: 520px;">
  Gestionale per toelettatori nato da un'esigenza concreta.<br>
  Pagamenti ricorrenti con Stripe,servizi salvati su SupaBase,<br>
  email di invito e reset password.
</p>

<div v-click style="display: flex; gap: 20px; margin-top: 8px;">
  <div style="background: rgba(159,225,203,0.07); border: 1px solid rgba(159,225,203,0.2); border-radius: 12px; padding: 16px 32px; text-align: center;">
    <div style="color: #9fe1cb; font-size: 36px; font-weight: 400;">Stripe</div>
    <div style="color: rgba(255,255,255,0.35); font-size: 10px; letter-spacing: 0.15em; text-transform: uppercase; margin-top: 4px;">Pagamenti ricorrenti</div>
  </div>
  <div style="background: rgba(159,225,203,0.07); border: 1px solid rgba(159,225,203,0.2); border-radius: 12px; padding: 16px 32px; text-align: center;">
    <div style="color: #9fe1cb; font-size: 36px; font-weight: 400;">SupaBase</div>
    <div style="color: rgba(255,255,255,0.35); font-size: 10px; letter-spacing: 0.15em; text-transform: uppercase; margin-top: 4px;">Gestione servizi</div>
  </div>
  <div style="background: rgba(159,225,203,0.07); border: 1px solid rgba(159,225,203,0.2); border-radius: 12px; padding: 16px 32px; text-align: center;">
    <div style="color: #9fe1cb; font-size: 36px; font-weight: 400;">✉</div>
    <div style="color: rgba(255,255,255,0.35); font-size: 10px; letter-spacing: 0.15em; text-transform: uppercase; margin-top: 4px;">Email automatizzate</div>
  </div>
</div>

</div>

---

<div class="absolute inset-0" style="background: linear-gradient(135deg, #1a1a2e 0%, #16213e 50%, #0f3460 100%)"></div>
<div class="absolute inset-0" style="background-image: url('https://upload.wikimedia.org/wikipedia/commons/thumb/5/5b/Politecnico_di_Torino_%28edificio_principale%29.jpg/1280px-Politecnico_di_Torino_%28edificio_principale%29.jpg'); background-size: cover; background-position: center; opacity: 0.2;"></div>

<div class="relative z-10 flex items-center justify-center h-full gap-14" style="padding: 0 64px;">

  <div style="flex: 1; text-align: left;">
    <div v-motion :initial="{ opacity: 0, x: -20 }" :enter="{ opacity: 1, x: 0, transition: { delay: 100 } }"
      style="font-family: 'DM Mono', monospace; font-size: 11px; letter-spacing: 0.2em; color: rgba(159,225,203,0.6); text-transform: uppercase; margin-bottom: 14px;">
      Politecnico di Torino
    </div>
    <h1 v-motion :initial="{ opacity: 0, x: -20 }" :enter="{ opacity: 1, x: 0, transition: { delay: 250 } }"
      style="font-family: 'Playfair Display', serif; font-size: 44px; font-weight: 400; color: white; line-height: 1.15; margin-bottom: 18px;">
      Matematica<br><em style="color: #9fe1cb">per l'Ingegneria.</em>
    </h1>
    <p v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1, transition: { delay: 400 } }"
      style="font-size: 16px; color: rgba(255,255,255,0.5); font-weight: 300; line-height: 1.8; max-width: 340px;">
      Cinque anni di curiosità convergono qui —<br>dove i problemi diventano progetti.
    </p>
  </div>

  <div v-click style="flex: 1; display: flex; flex-direction: column; gap: 12px;">
    <div v-for="(item, i) in items" :key="i"
      style="background: rgba(159,225,203,0.06); border: 1px solid rgba(159,225,203,0.18); border-radius: 12px; padding: 14px 20px; text-align: left;">
      <div style="color: #9fe1cb; font-size: 13px; font-weight: 400; margin-bottom: 3px;">{{ item.title }}</div>
      <div style="color: rgba(255,255,255,0.4); font-size: 12px; font-weight: 300; line-height: 1.6;">{{ item.desc }}</div>
    </div>
  </div>

</div>

<script setup>
const items = [
  { title: 'Interdisciplinare',   desc: 'Fisica, chimica, informatica e matematica in un unico percorso.' },
  { title: 'Problem solving',     desc: 'Sviluppato durante i 5 anni di scientifico.' },
  { title: 'Progetti concreti',   desc: 'Stazione meteo, gestionali e altri — github.com/1ilir0lika.' },
]
</script>
