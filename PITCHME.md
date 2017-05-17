## Tilelook | VBL | VR/AR

---

# Tilelook Design Tool

---

### PC běžného uživatele
- Intel  i3 / i5, 3. nebo 4. generace (ročník 2013+)
- Intel HD 4000 nebo novější (ročník 2013+)
- nVidia GeForce 340 nebo novější (ročník 2010+)
- 4GB > 8GB RAM
- FullHD rozlišení 1980x1050
- Operační systém Windows 7 / 10

---?image=assets/asus_eee.jpg

---

### Extrémní PC
- Asus EEE PC
  - Intel Atom 1.6GHz, Intel GMA 900, 1GB RAM, 1024x600, Windows XP

---

### Extrémní PC
- Intel Xeon (více fyzických jader)
- nVidia GeForce 1080Ti
- 32GB RAM
- 4K rozlišení 3840x2160
- Windows 10

---

### Legacy kód
3 roky vývoje před naším příchodem

quick fixy, časově závislý kód (Thread.sleep()), nulový refaktoring, UnsupportedOperationException, až 30% mrtvý kód, 0 testů

přepsat či refaktorovat ?

---?image=assets/legacy_code.jpg

---

### Zneužití uživateli
Uživatelsky přívětivý nástroj pro design místností (koupelen) se zaměřením na rozmístění kachlíků

Napojení na 3D Warehouse umožňuje stahovat Sketchup modely
 - desítky až stovky tisíc polygonů na objekt

---?image=assets/design_tool_0.jpg

---

---?image=assets/design_tool_1.png

---

---?image=assets/design_tool_2.jpg

---

---?image=assets/design_tool_3.jpg

---

### Java a certifikáty
Operační systém obsahuje seznam důvěryhodných certifikačních autorit

Java má svůj vlastní

Aktualizační process založený na HTTPS komunikaci

---

### Výběr technologií

Futures / promises
 - spaghetti kód + Thread.sleep(2500ms)
 - vlastní knihovna futures / promises
 - rxJava
 - CompletableFuture (Java 7)
 - JavaSlang

---

### Výběr technologií

Vykreslování 3D náhledu
 - Velice komplikovaný OpenGL kód
 - JMonkeyEngine
   - Každý tab má vlastní canvas
   - Změna velikosti canvasu
   - Deffered shading hack
   - IllegalStateException race
   - Bug v pohybu kamery (interní časovač?)

---

### OpenGL 2.1 limity

Specifikace z roku 2006

---

### Java + OpenGL + Mac

Ovladače se aktualizují až s aktualizací systému
 - Zoufalý výkon u AMD/ATi grafických karet

Běžná konfigurace
 - 4K rozlišení, Intel Iris, 8GB RAM

Java
 - Množství platformně závislých bugů (horší podpora)
 - Veškeré GUI musí běžet ve Swing vlákně

---

### Zajímavé algoritmy

PDF projektová dokumentace - obrys objektů (winged edge mesh, kd strom)

Deffered rendering

Detekce a vyhlazovaní hran

Pakování dat - 1 float obsahuje více proměnných o menším rozsahu