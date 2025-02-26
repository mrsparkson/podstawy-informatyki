# Topologie Sieci

## Sieci Fizyczne
Sieci fizyczne odnoszą się do fizycznego ułożenia kabli, urządzeń i połączeń. Przykłady:
- **Topologia magistrali** (Bus) :
  - Wady: Awaria jednej części sieci (np. przerwanie kabla) może zakłócić całą sieć.
  Zmniejsza się wydajność w miarę dodawania urządzeń.
  Trudności w rozbudowie sieci.
  - Zalety: Prosta i tania w implementacji.
   Wymaga mniejszej ilości kabli.
  - Gdzie stosowane: Używana w małych sieciach, np. w starszych systemach lokalnych (LAN).
- **Topologia pierścienia** (Ring):
  - Wady: Awaria jednej części sieci powoduje przerwanie całej komunikacji.
  Trudności w rozbudowie.
  - Zalety: Prosta w budowie i łatwa do implementacji.
   Brak kolizji w sieci, ponieważ dane podróżują w jednym kierunku.
  - Gdzie stosowane: Stosowana w starszych sieciach, np. w sieci Token Ring.
- **Topologia gwiazdy** (Star):
  - Wady:
   Wymaga centralnego urządzenia (hub/switch), które może stać się punktem awarii.
  Większe zużycie okablowania.
  - Zalety:
   Łatwość w rozbudowie i konfiguracji.
   Awaria jednego urządzenia nie wpływa na działanie całej sieci.
  - Gdzie stosowane:
  Współczesne sieci LAN, np. Ethernet.

## Sieci Logiczne
Sieci logiczne opisują sposób przesyłania danych między urządzeniami, niezależnie od fizycznej struktury. Przykłady:

- **Punkt-punkt** (Point-to-Point):
  - Wady:
   Ograniczona skalowalność, ponieważ sieć może łączyć tylko dwa urządzenia.
  - Zalety:
   Prosta i niezawodna komunikacja.
  - Zastosowanie:
   Łącza między dwoma routerami, połączenia VPN.

- **Przekazywanie żetonu** (Token Passing):
  - Wady:
  Potrzebny jest specjalny mechanizm synchronizacji.
  Może dochodzić do opóźnień w przypadku utraty tokenu.
  - Zalety:
  Brak kolizji w sieci, ponieważ tylko urządzenie posiadające token może wysyłać dane.
  - Zastosowanie:
  Sieci Token Ring, Ethernet z wykorzystaniem Token Passing.

- **Wielodostępowa** (Multiple Access):
  - Wady:
  Możliwość kolizji, co wymaga dodatkowego zarządzania dostępem.
  - Zalety:
   Umożliwia współdzielenie medium przez wiele urządzeń.
  - Zastosowanie:
   Sieci Ethernet, Wi-Fi.