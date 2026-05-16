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
    {{ gh.bio }}
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
    <img src="https://images.unsplash.com/photo-1504608524841-42584120d693?w=640&q=80"
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
<div class="absolute inset-0" style="background-image: url('https://images.unsplash.com/photo-1611996575749-79a3a250f948?w=1280&q=80'); background-size: cover; background-position: center; opacity: 0.15;"></div>

<div class="relative z-10 flex items-center justify-center h-full gap-12" style="padding: 0 60px;">

  <div v-motion :initial="{ opacity: 0, x: -20 }" :enter="{ opacity: 1, x: 0, transition: { delay: 350 } }"
    style="flex: 1; border-radius: 14px; overflow: hidden; border: 1px solid rgba(159,225,203,0.2);">
    <img src="https://images.unsplash.com/photo-1611996575749-79a3a250f948?w=640&q=80"
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
      {{ repo.desc || 'Implementazione digitale del classico gioco da tavolo in codice.' }}
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
<div class="absolute inset-0" style="background-image: url('https://images.unsplash.com/photo-1551582045-6ec9c11d8697?w=1280&q=80'); background-size: cover; background-position: center; opacity: 0.18;"></div>

<div class="relative z-10 flex flex-col items-center justify-center h-full gap-6 text-center">

<div v-motion :initial="{ opacity: 0, y: -20 }" :enter="{ opacity: 1, y: 0, transition: { delay: 100 } }"
  style="font-family: 'DM Mono', monospace; font-size: 11px; letter-spacing: 0.2em; color: rgba(159,225,203,0.6); text-transform: uppercase;">
  Stage della Matematica · Bardonecchia
</div>

<h1 v-motion :initial="{ opacity: 0, y: 20 }" :enter="{ opacity: 1, y: 0, transition: { delay: 300 } }"
  style="font-family: 'Playfair Display', serif; font-size: 58px; font-weight: 400; color: white; line-height: 1.1;">
  <em style="color: #9fe1cb">Matematica.</em>
</h1>

<p v-motion :initial="{ opacity: 0 }" :enter="{ opacity: 1, transition: { delay: 500 } }"
  style="font-size: 17px; color: rgba(255,255,255,0.55); font-weight: 300; line-height: 1.8; max-width: 480px;">
  Tre anni di seguito sulle Alpi —<br>tra dimostrazioni, problemi aperti e neve.
</p>

<div v-click style="display: flex; gap: 20px; margin-top: 8px;">
  <div style="background: rgba(159,225,203,0.07); border: 1px solid rgba(159,225,203,0.2); border-radius: 12px; padding: 16px 32px; text-align: center;">
    <div style="color: #9fe1cb; font-size: 36px; font-weight: 400;">3</div>
    <div style="color: rgba(255,255,255,0.35); font-size: 10px; letter-spacing: 0.15em; text-transform: uppercase; margin-top: 4px;">anni consecutivi</div>
  </div>
  <div style="background: rgba(159,225,203,0.07); border: 1px solid rgba(159,225,203,0.2); border-radius: 12px; padding: 16px 32px; text-align: center;">
    <div style="color: #9fe1cb; font-size: 36px; font-weight: 400;">1312</div>
    <div style="color: rgba(255,255,255,0.35); font-size: 10px; letter-spacing: 0.15em; text-transform: uppercase; margin-top: 4px;">metri · Alta Val di Susa</div>
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
  Selezionato tra i migliori studenti del Piemonte<br>nella competizione nazionale.
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