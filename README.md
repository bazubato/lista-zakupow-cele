📋 Moje listy — zakupy i cele życiowe

Progresywna aplikacja webowa (PWA) do zarządzania listą zakupów i celami życiowymi w jednym miejscu. Dane są w pełni edytowalne, kategoryzowane i zapisywane lokalnie na urządzeniu — bez konieczności logowania czy połączenia z internetem.

🔗 Działająca wersja: twojanazwa.github.io/lista-zakupow-cele (podmień na swój link)

Funkcje
Dwa tryby list — przełączanie między listą zakupów a celami życiowymi, każdy z osobnym zestawem danych.
Własne kategorie — dodawanie, usuwanie i zmiana kolejności kategorii (przeciąganie) w każdej z list.
Zmiana kategorii pozycji — jednym dotknięciem, z natywnym pickerem systemowym.
Priorytety — oznaczanie ważnych pozycji, które automatycznie wskakują na górę listy.
Odhaczanie i usuwanie — pojedynczo lub zbiorczo (wszystkie ukończone naraz).
Trwały zapis danych — lista zostaje zapamiętana między sesjami (localStorage), bez backendu i bazy danych.
Instalacja jako aplikacja — działa jako PWA: można dodać do ekranu głównego telefonu i korzystać offline.
Technologie
HTML / CSS / JavaScript — bez frameworków, czysty (vanilla) kod.
localStorage — trwałe przechowywanie danych po stronie klienta.
PWA — manifest.json + service worker (sw.js) dla instalowalności i działania offline.
Responsywny design zaprojektowany mobile-first.
Struktura projektu
├── index.html      # cała logika i interfejs aplikacji
├── manifest.json    # metadane PWA (nazwa, ikony, kolory)
├── sw.js             # service worker — cache i obsługa offline
├── icon-192.png      # ikona aplikacji (mała)
└── icon-512.png      # ikona aplikacji (duża)
Uruchomienie lokalnie

Aplikacja nie wymaga instalacji ani serwera — wystarczy otworzyć index.html w przeglądarce. Do pełnego testowania trybu PWA (instalacja, offline) zalecane jest jednak uruchomienie przez prosty serwer lokalny, np. rozszerzeniem Live Server w VS Code.

Czego się nauczyłem / co przetestowałem
Zarządzanie stanem aplikacji i renderowanie UI bez frameworka (czysty DOM API).
Obsługę zdarzeń dotykowych (pointerdown / pointermove) do implementacji przeciągania elementów (drag & drop) — działającego zarówno na telefonie, jak i na komputerze.
Podstawy Progressive Web App: manifest, service worker, strategię cache-first.
Projektowanie z myślą o urządzeniach mobilnych (mobile-first) i dostępności natywnych komponentów systemowych (np. natywny date/select picker zamiast własnych, które gorzej działają na dotyku).
Możliwe rozszerzenia
Synchronizacja danych między urządzeniami (backend + baza danych).
Terminy i przypomnienia dla celów życiowych.
Udostępnianie listy innym osobom.
