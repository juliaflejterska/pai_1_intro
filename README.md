1. Co to są circuit breakers i do czego służą? Dlaczego to jest ważny element aplikacji Netfixa?

Circuit breakers to mechanizm, który zapobiega awariom przez kontrolowanie przeciążenia i ograniczanie nacisku na usługi. W przypadku Netflixa, który działa w oparciu o architekturę mikrousługową, circuit breakers działają na poziomie mikrousług, gdzie wykrywają przeciążenia lub problemy z komunikacją z daną usługą. Gdy pojawia się problem, circuit breaker przechodzi w tryb otwarty i blokuje żądania, co czasowo odciąża system i pozwala na przywrócenie go do stabilnego stanu. Dzięki temu inne usługi mogą dalej działać, a użytkownicy mogą kontynuować korzystanie z platformy bez przerw.

2. Wykorzystaj jq, aby wypisać nazwy super bohaterów z https://mdn.github.io/learning-area/javascript/oojs/json/superheroes.json. Wrzuć pełną instrukcję z curl i jq do pliku README.md w Twoim repozytorium.

curl -s https://mdn.github.io/learning-area/javascript/oojs/json/superheroes.json | jq '.members[].name'
