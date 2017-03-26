# DELL XPS 15 zacina się

## Problem
Po świeżej instalacji Windowsa 10, DELL XPS 15 9560 (z monitorem: 4K) przycina się co jakiś czas.

## Rozwiązanie
Należy zainstalować ręcznie sterownik **Intel(R) HD Graphics 630** ze strony Intela.

## Jak to zrobić?
1. Najpierw należy pobrać plik ZIP ze sterownikiem [ze strony Intela](https://downloadcenter.intel.com/download/26669/Graphics-Intel-Graphics-Driver-for-Windows-15-45-?v=t). Na stronie **może pojawić** się żółta ramka mówiącą, że dostępna jest nowsza wersja tego sterownika.
   > A newer version of this software is available. Click here to get the latest version of this software.
   - my testowaliśmy wersję 21.20.16.4627, ale lepiej najpierw spróbować wersji najnowszej

2. Należy rozpakować plik, który dla naszej wersji nawzywał się **win64_154516.4627.zip** - jest to sterownik karty graficznej **Intel(R) HD Graphics 630**.
3. Następnie otwieramy Menedżer urządzeń -> Karty graficzne
4. Prawy klik na **Intel(R) HD Graphics 630** i klik na Aktualizuj Oprogramowanie Sterownika
5. Przeglądaj mój komputer w poszukiwaniu oprogramowania sterownika
6. Wskazać na podfolder `\Graphics` w folderze z rozpakowanym sterownikiem
   > Ważne jest żeby wskazać podfolder Graphics w rozpakowanym folderze ze sterownikiem! Wybór całego folderu może sprawić, że sterownik się nie zainstaluje.
   - należy zaznaczyć opcję `[x] Uwzględnij podfoldery`
7. Kliknąc `Dalej` i pozwolić na zainstalowanie sterownika.

Po instalacji najlepiej jest zrestartować system Windows. Problem powinien zniknąć.

[< Powrót](index.md)
