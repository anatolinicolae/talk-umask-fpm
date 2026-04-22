---
layout: two-cols
---

## `umask` crash course

<v-clicks>

- Maschera per la creazione dei file
- Filtro o negazione permessi da assegnare ai file finali in base alla richiesta dei programmi
- Viene definito in `/etc/login.defs` e sourced da parte di `pam_umask`
- `027` è il default per Debian/Ubuntu in devsec.os_hardening

</v-clicks>

::right::

<div class="flex items-center justify-center h-full -mr-12">
    <img src="/umask.png" class="mh-full w-auto" />
</div>
