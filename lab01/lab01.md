# Vaja 1: Varnost posameznikov v kibernetskem prostoru

Kibernetski prostor danes uporabljamo na vsakem vidiku našega življenja — od vsakdanjih komunikacij, nakupovanja, bančništva, do dela in zabave. Posamezniki se v njem znajdemo kot uporabniki, ustvarjalci pa tudi tarče, pogosto pa se ne zavedamo vseh nevarnosti in posledic svojih dejanj.

Cilj vaj pri predmetu Varnost posameznikov v kibernetskem prostoru je študentom približati ključne pojme kibernetske varnosti z vidika posameznika, razviti občutek za tveganja in ranljivosti ter jih opremiti z osnovnimi znanji za varnejšo uporabo sodobnih tehnologij.

# 🧪 Vaja 1: Spoznajmo kibernetski prostor

Prva vaja je namenjena uvodu v kibernetsko varnost ter spoznavanju osnovnih pojmov in izzivov:

- Kdo ali kaj je posameznik v kibernetskem prostoru?
- Kaj pomeni pojem kibernetski prostor in kako ga zaznavamo?
- Kaj razumemo pod pojmom kibernetska varnost?

## 1️⃣ Uvod: Analiza osebne izpostavljenosti v kibernetskem prostoru

Cilji vaje:  
✅ Spoznati osnovne pojme: posameznik, kibernetski prostor, kibernetska varnost, zasebnost.  
✅ Prepoznati osebne podatke in kako so dostopni v spletnem okolju.  
✅ Razumeti, kako sodobne tehnologije vplivajo na varnost in zasebnost posameznika.  

### Varnost in zasebnost

Posameznik v kibernetskem prostoru je vsak uporabnik digitalnih tehnologij in interneta, ki deluje, komunicira ali pušča sledove v digitalnem okolju. To vključuje uporabo naprav (računalniki, telefoni), storitev (spletne strani, aplikacije, družbena omrežja) in omrežij.

Varnost:
Varnost v kibernetskem prostoru pomeni zaščito informacijskih sistemov, omrežij in podatkov pred nepooblaščenim dostopom, napadi, okvarami ali zlorabo. Cilj je zagotoviti zaupnost, celovitost in razpoložljivost podatkov in storitev.
Primer: preprečiti vdor v uporabnikov e-poštni račun.

Zasebnost:
Zasebnost se nanaša na pravico posameznika, da nadzira svoje osebne podatke in način, kako se ti zbirajo, uporabljajo, delijo ali hranijo. Gre za to, koliko informacij o sebi posameznik želi razkriti in komu.
Primer: pravica, da spletna platforma brez soglasja ne deli uporabnikovih podatkov z oglaševalci.

## 2️⃣ Aktivnost: Analiza osebne izpostavljenosti

V brskalniku odprite način incognito/private in poiščite informacije o sebi (npr. preko iskalnikov in storitev za preverjanje izpostavljenosti):
- Poiščite svoje ime in priimek v Googlu.
- Preverite morebitne javne profile (Facebook, LinkedIn, Instagram, forumi).
- Uporabite orodja za preverjanje izpostavljenosti (HaveIBeenPwned, OSINTLeak)
- Orodja: PimEyes, haveibeenpwned, OSINTLeak

### Google dorking/hacking

Google Dorking (imenovan tudi Google Hacking) je tehnika, pri kateri uporabimo napredne iskalne operatorje v Googlu (ali drugih iskalnikih), da najdemo informacije, ki niso namenjene javnosti, a so kljub temu dostopne prek spleta.

Ne gre za vdor v sisteme, temveč za izkoriščanje napačno konfiguriranih spletnih strani, strežnikov ali aplikacij, kjer so datoteke, dokumenti ali celo gesla javno objavljena, a skrita pred običajnimi uporabniki.

### 📘 Primeri Google Dork iskalnih poizvedb

| Iskalna poizvedba                       | Kaj najde?                                        |
|----------------------------------------|---------------------------------------------------|
| `filetype:pdf site:gov.si`             | PDF dokumenti na slovenskih vladnih straneh       |
| `intitle:"index of" passwords`         | Mape z imenom "index of" in datotekami z gesli    |
| `inurl:admin login`                    | Strani z možnostjo prijave v administracijo       |
| `site:pastebin.com password`           | Objave z gesli na Pastebin                        |
| `"confidential" filetype:pdf`          | Dokumenti z oznako "confidential" v PDF obliki    |
| `ext:sql intext:"password"`            | Javne SQL datoteke, ki vsebujejo gesla            |
| `intitle:"webcamXP 5"`                 | Nezaščiteni vmesniki IP kamer                     |
| `inurl:/phpinfo.php`                   | Javne PHP konfiguracijske datoteke                |
| `filetype:env intext:DB_PASSWORD`      | Javne `.env` datoteke z gesli do baz              |
| `site:*.* inurl:/config.json`          | Javne konfiguracijske datoteke aplikacij          |

Google Dorking ni nezakonit, dokler ne posegamo v zaščitene sisteme. Vendar pa najdenih informacij ne smemo zlorabiti, shranjevati brez dovoljenja ali javno razkrivati.

Google sicer omogoča tudi uporabo Google Alerts, ki ga lahko uporabimo za nastavitev opozoril za omembe imena.

## 3️⃣ Refleksija in analiza

- Zapišite kratko poročilo o tem katere podatke ste našli.
- Kakšno potencialno tveganje predstavljajo?
- Zapišite primer črnega scenarija kako bi nekomu ti podatki lahko prišli prav na primeru osebne izpostavljenosti.
- Kako bi ocenili svojo osebno varnost/zasebnost?