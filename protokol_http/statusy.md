# Grupy statusów HTTP
 - HTTP status codes (kody odpowiedzi HTTP) są grupowane w pięciu głównych kategoriach. Każda z tych grup reprezentuje inny typ odpowiedzi serwera. Oto szczegóły dla każdej grupy:

### 1XX - Informacyjne
#### Statusy w tej grupie wskazują, że żądanie zostało odebrane i proces jest kontynuowany. Serwer informuje klienta, że żądanie jest w toku, ale jeszcze nie zakończone.

- 100 Continue - Serwer otrzymał początkową część żądania i oczekuje na resztę.
- 101 Switching Protocols - Serwer akceptuje żądanie zmiany protokołów, np. z HTTP na WebSocket.
### 2XX - Sukces
#### Statusy w tej grupie oznaczają, że żądanie zostało poprawnie przyjęte, zrozumiane i wykonane.

- 200 OK - Żądanie zostało pomyślnie przetworzone. Jest to najbardziej popularny status.
- 201 Created - Zasób został pomyślnie utworzony w odpowiedzi na żądanie.
- 202 Accepted - Żądanie zostało przyjęte, ale nie zostało jeszcze przetworzone.
- 204 No Content - Żądanie zostało pomyślnie wykonane, ale nie ma żadnej treści do odesłania.
### 3XX - Przekierowania
#### Statusy w tej grupie oznaczają, że klient musi podjąć dodatkowe kroki w celu zakończenia żądania. Zwykle chodzi o przekierowanie na inny adres URL.

- 301 Moved Permanently - Zasób został na stałe przeniesiony pod inny adres URL.
- 302 Found - Zasób został tymczasowo przeniesiony na inny adres URL.
- 304 Not Modified - Zasób nie zmienił się od ostatniego zapytania i nie ma potrzeby ponownego pobierania.
### 4XX - Błędy klienta
#### Statusy w tej grupie wskazują, że żądanie klienta jest niepoprawne lub nie może zostać przetworzone z powodu błędu po stronie klienta.

- 400 Bad Request - Żądanie jest nieprawidłowe, np. zawiera błędną składnię.
- 401 Unauthorized - Żądanie wymaga uwierzytelnienia użytkownika.
- 403 Forbidden - Serwer rozumie żądanie, ale odmawia jego wykonania.
- 404 Not Found - Zasób, o który proszono, nie został znaleziony.
### 5XX - Błędy serwera
#### Statusy w tej grupie wskazują, że żądanie jest poprawne, ale wystąpił błąd po stronie serwera.

- 500 Internal Server Error - Ogólny błąd serwera. Serwer nie jest w stanie przetworzyć żądania z powodu problemu wewnętrznego.
- 502 Bad Gateway - Serwer działa jako brama lub serwer pośredniczący, ale otrzymał nieprawidłową odpowiedź od innego serwera.
- 503 Service Unavailable - Serwer jest niedostępny, zazwyczaj z powodu przeciążenia lub przeprowadzania prac konserwacyjnych.
- 504 Gateway Timeout - Serwer nie otrzymał odpowiedzi na czas od innego serwera.