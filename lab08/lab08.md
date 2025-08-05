
# 🧩 Vaja 8: MetaOSINT – Kaj vse razkrije slika?

## 🎯 Namen vaje

Ta vaja je namenjena raziskovanju informacij, ki jih lahko razkrijemo s pomočjo **metapodatkov v slikah (EXIF)**. Udeleženci bodo s pomočjo spletnih orodij analizirali fotografijo in ugotavljali njeno lokacijo, čas nastanka, napravo in druge skrite podatke.

## ✅ Cilji vaje

- Razumeti pomen metapodatkov v digitalnih slikah.
- Uporabiti OSINT orodja za analizo EXIF podatkov.
- Oceniti tveganja, povezana z deljenjem slik na spletu.
- Razviti kritično razmišljanje o zasebnosti in digitalnih sledeh.

---

## 🖼️ Primer slike

Uporabi testno sliko z vključenimi EXIF podatki – lahko izbereš eno izmed teh zbirk:

- [https://github.com/ianare/exif-samples](https://github.com/ianare/exif-samples)
- Ali pa sliko z lastnim mobilnim telefonom (poskrbi, da ima vključeno lokacijo).

---

## 🔍 Orodja za analizo EXIF metapodatkov

1. 🌍 [https://www.pic2map.com/](https://www.pic2map.com/)
2. 🔧 [https://exif.tools/](https://exif.tools/)

---

## 📝 Navodila za izvedbo

1. **Izberi sliko z EXIF podatki**
   - Naj bo to slika, ki je bila posneta z mobilno napravo z omogočeno lokacijo.

2. **Naloži sliko v spletno orodje**
   - Odpri [https://pic2map.com](https://pic2map.com) ali [https://exif.tools](https://exif.tools)
   - Naloži svojo testno sliko.
   - Oglej si rezultate analize: GPS, datum, čas, naprava, orientacija itd.

3. **Analiziraj lokacijo**
   - Če so prikazane koordinate, jih prilepi v Google Maps ali OpenStreetMap in preveri dejansko lokacijo.
   - Primerjaj ali se lokacija ujema z realnostjo.

4. **Analiziraj čas in napravo**
   - Kdaj je bila slika posneta?
   - S katero napravo?
   - So prisotni drugi zanimivi podatki (npr. orientacija, programska oprema itd.)?

---

## 📄 Poročilo (oddaja)

Odgovori na naslednja vprašanja:

1. Kakšna je bila natančna lokacija (koordinate in naslov)?
2. Kdaj je bila slika posneta?
3. Katere druge metapodatke si zaznal?
4. Kaj te je presenetilo?
5. Kaj bi priporočal osebi, ki redno objavlja slike na spletu?

---

## 💬 Refleksija

- Ali bi moral vsak pred objavo slike odstraniti EXIF podatke?
- Kako se lahko zaščitimo pred zlorabo takšnih informacij?
- Ali si že kdaj objavil sliko, ki je vsebovala takšne metapodatke? Kakšen bi bil tvoj odziv danes?

---

## 🛠️ Dodatno

- Poskusi uporabiti orodje `exiftool` lokalno v terminalu:
```bash
exiftool tvoja_slika.jpg
```

---

## 📌 Pomembno

Namen vaje ni kršiti zasebnosti drugih, temveč **ozavestiti, kako hitro in preprosto je razkriti podatke iz slike** ter se posledično **naučiti varne rabe digitalnih vsebin**.

---

## 🧼 Kako odstraniti EXIF metapodatke

Če želiš pred objavo slike odstraniti vse metapodatke, imaš več možnosti:

### 🖥️ Z uporabo `exiftool` (ukazna vrstica)

1. Namesti orodje:
```bash
sudo apt install libimage-exiftool-perl   # Debian/Ubuntu
brew install exiftool                     # macOS
```

2. Za odstranitev vseh metapodatkov iz slike (ustvari kopijo):
```bash
exiftool -all= slika.jpg
```

3. Če želiš prepisati obstoječo datoteko:
```bash
exiftool -all= -overwrite_original slika.jpg
```

---

### 🌐 Spletna orodja (za hitre primere)

- [https://www.verexif.com/en/](https://www.verexif.com/en/)
- [https://www.exifremove.com/](https://www.exifremove.com/)

⚠️ Opozorilo: Ne uporabljaj spletnih orodij za občutljive slike.

---

### 🪟 Windows

- Desni klik na sliko → **Properties** → **Details**
- Klik **Remove Properties and Personal Information**

---

### 📱 Mobilni telefoni

**Android**:
- Photo Exif Editor
- Scrambled Exif (F-Droid)

**iOS**:
- Metapho
- Exif Metadata
