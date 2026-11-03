# Sito Dott. Francesco Maria Filardi — Osteopata (bozza)

Sito one-page statico: un solo `index.html` (CSS e JS inclusi) e le foto in `images/`.
Nessuna build: Vercel pubblica i file così come sono a ogni push su `main`.

## Lavorarci da un altro dispositivo

```bash
git clone https://github.com/andreawebstudio/francesco-maria-filardi.git
cd francesco-maria-filardi
```

Apri `index.html` nel browser (o usa `.claude/launch.json` nell'app Claude per l'anteprima locale),
modifica, poi:

```bash
git add -A
git commit -m "Descrizione della modifica"
git push
```

Dopo il push Vercel aggiorna il sito in automatico.

## Prima della pubblicazione definitiva

- Togliere il blocco `noindex` in `vercel.json` (ora la bozza non viene indicizzata dai motori di ricerca).
- Collegare il form contatti a un servizio di invio reale (ora apre il programma di posta).
- Creare `privacy-policy.html` e `cookie-policy.html`.
- Verificare iscrizione ROI, dati professionali e fiscali (commenti `DA VERIFICARE` / `TODO` in `index.html`).
- Aggiungere `canonical`, `og:url` e un URL assoluto per `og:image` con il dominio definitivo.
- Sostituire il segnaposto rotondo in "Chi sono" con la foto autentica.
