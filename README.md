# Husa blocare ecran

[APK și cele două ghiduri PDF](https://caiuspoputa-debug.github.io/aplicatii/#husa) · [Descărcare directă Husa 1.1.5](https://caiuspoputa-debug.github.io/aplicatii/downloads/husa/1.1.5/Husa-Blocare-Ecran-1.1.5.apk)

Aplicație Android pentru blocarea și aprinderea ecranului cu o husă magnetică, folosind magnetometrul necalibrat. Acest repository distribuie APK-ul semnat și documentația.

## 1.1.5: instalatorul intern eliminat

După reapariția avertizării Play Protect pe 1.1.4, instalatorul și descărcarea APK din Husa au fost eliminate. REQUEST_INSTALL_PACKAGES și FileProvider-ul pentru actualizări nu mai sunt prezente. Verificarea versiunii și descărcarea prin browser funcționează ca în 1.1.3, versiune acceptată pe telefon conform utilizatorului. Cauza exactă a clasificării Google și acceptarea APK-ului 1.1.5 nu sunt confirmate.

În meniul cu trei puncte: Verifică actualizările. Automat, verificarea se face cel mult o dată la 24 de ore când Husa este deschisă. Pentru o versiune nouă apare un popup. Deschide descărcarea deschide URL-ul APK-ului în browser. Deschide fișierul descărcat și confirmă actualizarea în Android. Husa nu mai solicită instalarea de aplicații.

Instalează 1.1.5 peste versiunea existentă, fără dezinstalare. Setările și semnătura sunt păstrate. Identificator: com.example.husablocareecran. Versiune 1.1.5, build 7. Certificatul personal Caius Poputa pe Android 13+: SHA-256 95c79cbc9e68e31611c477f8cc27050a682b4ee616a5c25d6cbc40005f1d2bf6, cu rotația corectată de la certificatul Husa 1.0.

## Monitorizare și diagnostic

Senzorul necalibrat, pragul, timpii și mecanismul alternativ de aprindere sunt neschimbate față de 1.1.4. Dacă impulsul inițial lasă afișajul stins, Reîncearcă aprinderea folosește Activity.setTurnScreenOn prin serviciul de accesibilitate activat de utilizator. Cererea se anulează la închiderea husei și expiră dacă este întârziată. Securitatea ecranului blocat rămâne activă. Comportamentul în Somn și în timpul apelurilor trebuie confirmat pe S25 Ultra.

Diagnostic oferă Copiază diagnosticul, Distribuie, Salvează fișier .txt și selectarea textului. Raportul păstrează 40 de evenimente și arată starea afișajului și confirmarea pornirii activității alternative. Doze Android și modul Somn Samsung sunt distincte.

Reglajele se salvează automat. Accesibilitatea, notificările și excepția de baterie folosesc confirmările Android. Menține deschisă în Recente și regulile Somn rămân pași manuali explicați în aplicație.

Compilarea release, 19 teste unitare, Lint fără erori, 29 verificări ale semnăturii și continuității actualizării, precum și alinierea APK au trecut. Nu s-a efectuat test fizic sau pe emulator. Aceste verificări nu constituie un verdict Play Protect.
