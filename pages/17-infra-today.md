---
layout: two-cols
---

<div class="flex flex-col h-full">

## Stato dell'infra ad oggi

<v-clicks class="flex-grow">

- Processo un po' più serio e consolidato con `uv` insieme ad Ansible + mitogen per ⚡
- Nuove feature come migrazioni one-time forward-only
- Coda di run pipeline e trigger su changes specifiche per singolo workflow
- Nuovi componenti come OpenTofu nel loop per provisioning di istanze
- Pool PHP-FPM che non si lamentano più 😇

</v-clicks>

<a href="https://github.com/thundersquared/infrastructure">github.com/thundersquared/infrastructure</a>

</div>

::right::

<div class="flex items-center justify-center h-full -mr-12">
    <img src="/pipelines.png" class="h-full w-full" />
</div>
