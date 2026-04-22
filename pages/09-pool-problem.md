---
layout: two-cols
---

## Cosa non funzionava più

<v-clicks>

- Aggiungere un sito: ok — pool config creata ✅
- Aggiungere un **secondo** sito: 💥
- Il pannello non riusciva ad assegnare una porta libera al nuovo pool
- 1 sito → 1 pool → 1 porta univoca per mantenere segregazione docroot & exec user
- Spoiler: con i permessi sbagliati, non riusciva a leggere le config esistenti per capire quale porta assegnare al nuovo pool

</v-clicks>

::right::

<div class="flex items-center justify-center h-full">
  <img src="/site-management-graphic.svg" class="max-h-80 w-auto -mr-24" />
</div>
