# Husa blocare ecran

Aplicație Android pentru blocarea și aprinderea ecranului printr-o husă cu magnet, folosind magnetometrul necalibrat.

[Descarcă Husa 1.1.1 și ghidurile PDF](https://caiuspoputa-debug.github.io/aplicatii/#husa)

[Descarcă direct APK-ul Husa 1.1.1](https://caiuspoputa-debug.github.io/aplicatii/downloads/husa/1.1.1/Husa-Blocare-Ecran-1.1.1.apk). Fișierul este servit direct de GitHub Pages și are aceeași semnătură și sumă SHA-256 ca APK-ul din release.

Versiunea 1.1.1 corectează continuitatea permisiunilor semnate la schimbarea certificatului. Această incompatibilitate din 1.1 putea împiedica actualizarea peste Husa 1.0, afișând „Aplicația nu este instalată”.

Versiunea 1.1 include configurarea timpilor, sensibilității și energiei, solicitarea permisiunilor, o pictogramă nouă și un jurnal local de diagnostic.

Acest repository distribuie APK-ul semnat și documentația de instalare și configurare.

## Configurare

Reglajele aplicației se salvează automat. Android cere confirmarea utilizatorului pentru accesibilitate, notificări și excepția de baterie. Opțiunile Samsung „Menține deschisă” din Recente și regulile modului Somn sunt pași manuali explicați în aplicație.

## Verificare și compatibilitate

Identificator Android: `com.example.husablocareecran`. Versiune: `1.1.1`, build `3`.

Pe Android 13+ pachetul folosește certificatul personal Caius Poputa, SHA-256 `95c79cbc9e68e31611c477f8cc27050a682b4ee616a5c25d6cbc40005f1d2bf6`. Include lanțul de rotație de la cheia Husa 1.0 pentru actualizare cu păstrarea datelor. Compatibilitatea instalării peste aplicația de pe telefon necesită proba pe dispozitiv.

Compilarea release, Lint vital, verificarea semnăturii și alinierea APK au trecut. Testul de regresie al semnăturii a trecut toate cele 27 de verificări: detectează lipsa continuității permisiunilor în 1.1 și confirmă corecția în 1.1.1. Logica husei este neschimbată față de 1.1, unde cele 8 teste au trecut și analiza Lint completă a raportat zero erori. Telefonul țintă este Samsung S25 Ultra. Testarea fizică și testarea în emulator nu au fost efectuate. Problema în modul Somn și la apel rămâne de confirmat cu jurnalul noii versiuni.
