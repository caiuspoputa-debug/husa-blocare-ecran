# Husa blocare ecran

[APK și cele două ghiduri PDF](https://caiuspoputa-debug.github.io/aplicatii/#husa) · [Descărcare directă Husa 1.1.4](https://caiuspoputa-debug.github.io/aplicatii/downloads/husa/1.1.4/Husa-Blocare-Ecran-1.1.4.apk)

Aplicație Android pentru blocarea și aprinderea ecranului cu o husă magnetică, folosind magnetometrul necalibrat. Acest repository distribuie APK-ul semnat și documentația.

## Ce aduce 1.1.4

Jurnalul S25 Ultra cu Android 17 a arătat deschideri detectate și cereri de aprindere, dar afișajul rămânea stins. Dacă impulsul inițial nu reușește, Reîncearcă aprinderea folosește acum Activity.setTurnScreenOn, prin serviciul de accesibilitate deja activat. Fereastra temporară nu are elemente interactive, este exclusă din Recente și se închide la aprindere, expirare sau închiderea husei. Cererile întârziate ori anulate sunt respinse înaintea activării aprinderii. PIN-ul și securitatea ecranului blocat nu sunt eliminate.

Magnetometrul necalibrat, pragul, logica tranzițiilor, reglajele și blocarea sunt păstrate. Diagnosticul arată starea efectivă a afișajului și dacă Android a creat și reluat activitatea alternativă. Doze Android și modul Somn Samsung sunt distincte. Efectul pe telefon trebuie confirmat în Somn și în timpul unui apel.

## Diagnostic și actualizări

Diagnostic oferă Copiază diagnosticul, Distribuie, Salvează fișier .txt și selectarea textului. Raportul include ultimele 40 de evenimente și starea telefonului la export.

În meniul cu trei puncte: Verifică actualizările. Automat, verificarea se face cel mult o dată la 24 de ore când Husa este deschisă. Pentru versiuni noi apare un popup. Descarcă actualizarea preia APK-ul prin HTTPS de pe domeniul de distribuție acceptat, apoi verifică dimensiunea, SHA-256, identificatorul, versiunea și certificatul. Instalează deschide instalatorul Android. Prima dată permiți instalarea din Husa, revii în aplicație și apeși din nou Instalează. Confirmarea Android rămâne obligatorie; nu există instalare silențioasă sau descărcare automată în fundal.

La cererea utilizatorului, în 1.1.4 au fost reintegrate instalatorul direct, permisiunea REQUEST_INSTALL_PACKAGES și un FileProvider neexportat, limitat la directorul cache al actualizărilor. Google Play Protect nu a fost încă verificat pe acest APK. Versiunea 1.1.3 fără instalator intern a fost acceptată pe telefon, conform utilizatorului; cauza avertizării precedente nu este stabilită.

## Configurare și compatibilitate

Reglajele se salvează automat. Android cere confirmarea utilizatorului pentru accesibilitate, notificări, excepția de baterie și instalarea din Husa. Menține deschisă în Recente și regulile Samsung Somn rămân pași manuali explicați în aplicație.

Pachet: com.example.husablocareecran. Versiune 1.1.4, build 6. Se instalează peste versiunea existentă. Pe Android 13+ folosește certificatul personal Caius Poputa, SHA-256 95c79cbc9e68e31611c477f8cc27050a682b4ee616a5c25d6cbc40005f1d2bf6, cu rotația corectată de la certificatul Husa 1.0.

Compilarea release, 19 teste unitare (8 ale husei, 5 ale actualizărilor, 5 ale cererilor de aprindere și testul existent), Lint fără erori, 29 verificări ale semnăturii și alinierea APK au trecut. Nu s-a efectuat test pe telefon sau emulator. Verdictul Play Protect și comportamentul One UI trebuie confirmate pe dispozitiv.

[Android: aprinderea ecranului](https://developer.android.com/reference/android/app/Activity#setTurnScreenOn(boolean)) · [Google: verificarea aplicațiilor](https://support.google.com/android/answer/2992033?hl=en)
