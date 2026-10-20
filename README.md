# Moonbase Control: Lazy Loading

Zadanie z modułu Angular. Repozytorium zawiera kod startowy aplikacji Moonbase Control dla tej lekcji.

## Zadanie

Skonfiguruj Lazy Loading dla widoku Missions.

#### 1. Skonfiguruj Lazy Loading
- Zmień eksport komponentu `Missions` na domyślny: `export default class Missions`.
- Usuń statyczny import komponentu.
- Wykorzystaj `loadComponent` oraz dynamiczny `import()`.

💡 Dzięki domyślnemu eksportowi `loadComponent: () => import('./features/missions/missions')` nie wymaga wskazywania nazwy klasy komponentu.

💡 Komponent powinien zostać pobrany dopiero podczas pierwszego przejścia na stronę.

#### 2. Zweryfikuj działanie
- Otwórz zakładkę Network.
- Odśwież aplikację.
- Przejdź do widoku Missions.
- Sprawdź, że przeglądarka pobiera nowy plik JavaScript dopiero po wejściu na tę ścieżkę.

## Jak zacząć

1. Zrób fork tego repozytorium na swoje konto GitHub.
2. Sklonuj swój fork na komputer.
3. Zainstaluj zależności: `npm install`.
4. Uruchom aplikację: `npm start`.
5. Jeśli zadanie korzysta z danych z API, uruchom w drugim terminalu mock API: `npm run api`.

## Jak oddać zadanie

1. Zapisz zmiany w commicie i wypchnij je do swojego forka.
2. Otwórz Pull Request z forka do repozytorium `mate-academy/angular_lazy-loading`, do brancha `main`.
3. Platforma uruchomi review Twojego Pull Requesta.
