# Husa blocare ecran

Aplicație Android pentru blocarea și aprinderea ecranului printr-o husă cu magnet, folosind magnetometrul necalibrat.

[Descarcă Husa 1.1 și ghidurile PDF](https://github.com/caiuspoputa-debug/husa-blocare-ecran/releases/tag/v1.1)

Versiunea 1.1 include configurarea timpilor, sensibilității și energiei, solicitarea permisiunilor, o pictogramă nouă și un jurnal local de diagnostic.

Acest repository distribuie APK-ul semnat și documentația de instalare și configurare.

## Configurare

Reglajele aplicației se salvează automat. Android cere confirmarea utilizatorului pentru accesibilitate, notificări și excepția de baterie. Opțiunile Samsung „Menține deschisă” din Recente și regulile modului Somn sunt pași manuali explicați în aplicație.

## Verificare și compatibilitate

Identificator Android: `com.example.husablocareecran`. Versiune: `1.1`, build `2`.

Pe Android 13+ pachetul folosește certificatul personal Caius Poputa, SHA-256 `95c79cbc9e68e31611c477f8cc27050a682b4ee616a5c25d6cbc40005f1d2bf6`. Include lanțul de rotație de la cheia Husa 1.0 pentru actualizare cu păstrarea datelor. Compatibilitatea instalării peste aplicația de pe telefon necesită proba pe dispozitiv.

Compilarea release, cele 8 teste ale logicii husei, verificarea semnăturii și alinierea APK au trecut. Android Lint a raportat zero erori. Telefonul țintă este Samsung S25 Ultra. Testarea fizică și testarea în emulator nu au fost efectuate. Problema în modul Somn și la apel rămâne de confirmat cu jurnalul noii versiuni.
