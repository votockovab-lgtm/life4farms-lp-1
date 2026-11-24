# LIFE4FARMS – zástupná landing page

Statický web (jeden HTML soubor s CSS a JS), připravený pro GitHub Pages.

- `lp/index.html` – landing page (česky)
- `lp/img/` – logo a fotka nebe
- `foto/`, `loga/` – fotky a loga, na které stránka odkazuje relativně (`../foto/…`, `../loga/…`), proto musí ležet vedle složky `lp/`
- `index.html` – přesměrování z kořene webu na `lp/`
- `.nojekyll` – GitHub Pages nemá soubory zpracovávat Jekyllem

## Nasazení

1. Nahrajte obsah této složky do kořene repozitáře.
2. Settings → Pages → Source: „Deploy from a branch“, větev `main`, složka `/ (root)`.
3. Web poběží na `https://<uživatel>.github.io/<repozitář>/` (kořen přesměruje na `/lp/`).

Pokud stránku přidáváte do existujícího repozitáře `life4farms_2`, kde už jsou `foto/` a `loga/`, stačí nahrát složku `lp/` a kořenový `index.html` vynechat.

Stránka má zatím `<meta name="robots" content="noindex">`, aby ji vyhledávače neindexovaly. Před ostrým spuštěním ji odstraňte.
