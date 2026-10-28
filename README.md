# Squadrats Live

Aplikacja na Androida pokazująca na żywo zdobywane kafelki Squadrats (squadrats i squadratinhos).
GPS działa też przy zgaszonym ekranie, a nowy kafelek wywołuje powiadomienie.

## Jak zbudować APK (GitHub Actions)

1. Utwórz na GitHubie nowe, puste repozytorium (może być prywatne).
2. Wgraj do niego całą zawartość tego folderu, z ukrytym folderem `.github`.
   Najprościej: Add file → Upload files i przeciągnij wszystko, albo `git push`.
3. Wejdź w zakładkę **Actions**. Workflow „Build APK" ruszy sam po wgraniu
   (albo uruchom go ręcznie przyciskiem „Run workflow").
4. Po kilku minutach otwórz zakończone uruchomienie i pobierz plik
   **squadrats-live-apk** z sekcji Artifacts. W środku jest `app-debug.apk`.
5. Przenieś APK na telefon i zainstaluj. Android poprosi o zgodę na instalację
   z nieznanych źródeł dla aplikacji, z której otwierasz plik.

## Pierwsze uruchomienie

1. Na squadrats.com: Map → Download KML.
2. W aplikacji: „Wgraj KML" i wskaż pobrany plik.
3. „Start", zgoda na lokalizację i powiadomienia.

## Żeby GPS nie był zabijany w tle

Ustawienia Androida → Aplikacje → Squadrats Live → Bateria → **Bez ograniczeń**.
Lokalizacja: najlepiej „Zezwalaj cały czas" (albo „tylko podczas używania aplikacji").

## Zmiany w aplikacji

Cały interfejs jest w `www/index.html`. Po edycji wgraj zmiany na GitHub,
a workflow zbuduje nowy APK.

## Autor

Marcin ([gabrys1](https://github.com/gabrys1)). Aplikacja nieoficjalna, niezwiązana ze Squadrats.com.
