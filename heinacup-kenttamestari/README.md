# HeinaCup Kenttämestari – Kuokkala TN

## Mitä ollaan tekemässä

Sovellus **Kuokkala TN** -kentän (Pohjanlahdentie 7, Jyväskylä) toiminnan hallintaan HeinaCup-turnauksessa (26.–28.6.2026).

Kenttä isännöi sarjoja: P2017 (tasot 1–3) ja T2018.

## Sovelluksen tarkoitus

- Kentän otteluvuorojen hallinta ja seuranta (aikataulu, sarjat, joukkueet)
- Tulosten kirjaus kentällä (mobiili)
- Kentän tilanteen reaaliaikainen näkymä (mikä peli menossa, mikä seuraavaksi)
- Mahdollisesti myöhemmin laajennettavissa seuran yleiseen käyttöön

## Tech stack

| Kerros | Ratkaisu | Miksi |
|--------|----------|-------|
| Frontend | Next.js (React) | Moderni, mobiilikäyttöinen, helppo kehittää |
| Backend/API | Next.js API routes + Supabase | Ei erillistä backendia tarvita |
| Tietokanta | Supabase (Postgres) | Ilmainen, CSV-import, reaaliaikainen |
| Hosting | Vercel | Ilmainen, git push = deploy |
| Versionhallinta | GitHub (henk.koht.) | Helppo siirtää seuralle myöhemmin |
| Domain | Voidaan osoittaa domainhotelli.fi:stä Verceliin | Esim. kuokkala.seura.fi tms. |

## Seuraavat askeleet

1. Luo GitHub-repo
2. Supabase-projekti + DB-skeema (ottelut, vuorot, tulokset)
3. Next.js -projektin runko
4. Sheet-datan import Supabaseen
5. Perusnäkymät: päivän aikataulu, tuloskirjaus, tilannenäkymä

## Turnauksen faktat

- **HeinaCup 2026**: 26.–28.6.2026, Jyväskylä & Laukaa
- **340 joukkuetta**, 15 kenttää, ikäluokat 2011–2019
- **Kuokkala TN**: tekonurmi, yksi kenttä
- **Otteluformaatti**: sarjat tasoluokittain (Elite/Kilpa/Haaste/Harraste), 4–6 ottelua/joukkue
- **Järjestäjä**: Palokan Riento
