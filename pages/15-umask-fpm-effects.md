---
layout: two-cols
---

## `umask` e pool PHP-FPM

<v-clicks>

- viene applicata la maschera `027`
- l'accesso di `others` viene totalmente rimosso
- il processo del pannello non può più leggere i file
- viene caricato l'ultimo file `.conf` leggibile
- viene calcolata una porta già in uso, non avendo contesto completo
- all'avvio del pool non si riesce a bindare su una porta già in uso
- `502 Bad Gateway` 😇💥

</v-clicks>

::right::

<div class="flex flex-col items-center justify-center h-full -mr-12">
    <img src="/umask-def.png" class="mh-full w-auto" />
    <img src="/umask-default.png" class="h-auto w-full" />
</div>
