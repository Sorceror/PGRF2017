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

---?image=assets/design_tool_1.png

---?image=assets/design_tool_2.jpg

---?image=assets/design_tool_3.png

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

---

# Virtual Beam Lines

---

### ELI Beamlines

Součástí evropského projektu Extreme Light Infrastructure

Několik pracovišť na území České republiky, Maďarska a Rumunska

Zkoumáním interakce světla s hmotou při nejvyšších intenzitách a nejkratších časových rozpětích

---

### Cíle Virtual Beam Line projektu

- Designér experimentů
- Nástroj pro vzdělávání (studentů, bezpečnosti práce)
- Součást PR pro veřejnost

---

### Fukční požadavky

- Model celé budovy včetně vybavení
- Běh na průměrném PC
- Možnost zobrazení na mobilních zařízeních
- Historie experimentů s možností nahrát i několik let starou verzi
- Propojení s reálnou konfigurací
- Zobrazení výsledků experimentů (simulace, reálné)

---

### Dvě paralelní verze

Unity - kompletní model, pohyb uvnitř scény, základy časticových systémů, vizualizace simulací

WebGL - částečný model

---

### Asset pipeline

- Ruční extrakce dat z Siemens Team Center
- Kompletace do jednoho celku a optimalizace modelů v 3D Max
- Export hierarchie (plochý csv soubor)
- Vytvoření BVH stromu z hierarchie
- Generování LOD
- Balení do binárního formátu (vertex a index buffer)

---

### Zajímavé algoritmy

Bounding volume hierarchy, LOD

Casticove systemy, raytracing pro vypočet cesty paprsku, volume rendering pro vysledky PIC (Particle in cell) simulací, řešení průhlednosti, ...

---

# VR / AR

---

### Vzestup

Technologie jsou dostupné už dlouhou dobu (90. léta - Nintendo Virtual Boy, Sega)

Výkon CPU/GPU dosáhl bodu kdy lze zobrazovat "věrné" scény v reálném čase

Nutné dosáhnout alespoň 60Hz při 2160x1200 pro každé oko

---?image=assets/virtual_boy.jpg

---

### Využití nejen na hry

Hry - stále se čeká na kvalitní AAA hru

Prohlídky - Virtual Beam Line, koncerty, muzea, sportovní události

Komunikace - video konference (facebook)

Zdravotnictví - psychologie, výuka (virtuální operace)

---

### Problémy

- výkon PC
- GUI ve VR
- konstrukce HMD (head mounted display)
- zpětná vazba (vibrační vesty)
- počítačové vidění (AR)
- umělá inteligence (komunikace s virtuálním světem)
- psychologie (závislost na VR)
- sociologie (oční kontakt během virtuální komunikace)

---

### Jak začít

Unity / Unreal enginy

Frameworky - VRTK (VR), A-Frame / Three.js (WebGL), Vuforia (AR), AR.js (mobile AR)

Udacity’s VR Developer Nanodegree

---

### Dostupný hardware

Cardboard / Samsung Gear VR, Daydream

Oculus rift, HTC Vive, Playstation VR

Hololens

Oznámeno mnoho dalších

---

# Let's play