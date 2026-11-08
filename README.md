# Husa blocare ecran

[Descarcă Husa 1.1.3 și cele două ghiduri PDF](https://caiuspoputa-debug.github.io/aplicatii/#husa)

[Descărcare directă APK 1.1.3](https://caiuspoputa-debug.github.io/aplicatii/downloads/husa/1.1.3/Husa-Blocare-Ecran-1.1.3.apk)

Aplicație Android pentru blocarea și aprinderea ecranului printr-o husă cu magnet, folosind magnetometrul necalibrat. Acest repository distribuie APK-ul semnat și documentația.

## Diagnostic și actualizări

În Diagnostic: Copiază diagnosticul, Distribuie, Salvează fișier .txt și selectarea textului prin apăsare lungă. Raportul include jurnalul și starea telefonului, energiei, permisiunilor și reglajelor la export.

În meniul cu trei puncte: Verifică actualizările. Verificarea automată se face cel mult o dată la 24 de ore, când aplicația este deschisă. O versiune nouă apare într-un popup. Butonul Deschide descărcarea trimite la APK în browser. Husa nu descarcă APK-uri și nu solicită instalarea lor. Permisiunea REQUEST_INSTALL_PACKAGES și furnizorul de fișiere pentru instalare au fost eliminate.

## Configurare și compatibilitate

Reglajele se salvează automat. Android cere confirmarea utilizatorului pentru accesibilitate, notificări, excepția de baterie. Opțiunile Samsung Menține deschisă și regulile modului Somn rămân pași manuali explicați în aplicație.

Identificator: `com.example.husablocareecran`. Versiune `1.1.3`, build `5`. Se instalează peste versiunea existentă. Pe Android 13+ folosește certificatul personal Caius Poputa, SHA-256 `95c79cbc9e68e31611c477f8cc27050a682b4ee616a5c25d6cbc40005f1d2bf6`, cu rotația corectată de la certificatul Husa 1.0.

După semnalarea avertizării „această aplicație poate fi dăunătoare”, instalatorul intern a fost eliminat pentru reducerea permisiunilor. Nu este confirmată cauza clasificării și nu a fost verificată acceptarea de către Play Protect. Nu ocoli avertizările de securitate.

Logica husei este neschimbată față de 1.1.2. Problema din modul Somn rămâne în investigație; exportul permite colectarea diagnosticului.

Compilarea release, analiza Lint fără erori, cele 8 teste ale husei, cele 5 teste ale regulilor de actualizare și verificările semnăturii și alinierii APK au trecut. Noile fluxuri nu au fost testate fizic pe telefon sau emulator.
