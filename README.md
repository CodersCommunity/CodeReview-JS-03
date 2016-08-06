# CodeReview-JS-03
CodeReview materiału z trzeciego odcinka kursu javascript.

Film: [Klik](https://www.youtube.com/watch?v=9FVtiJHFCSU)

Temat na forum: [Klik](http://forum.pasja-informatyki.pl/165988/cr-javascript-%233-gra-w-wisielca-przetwarzanie-lancuchow)

---

Ten branch zawiera poprawki dotyczące zarówno kodu HTML, arkusza stylów, jak i logiki skryptu JS.

---

## Lista poprawek

_Tak naprawdę największe zmiany zaszły w skrypcie, który nadaje grze logikę. Został on mocno przebudowany, obecnie jest bardziej czytelny i spełnia wiele dobrych praktyk w JS._

### Ogólne

* Polskie klasy/identyfikatory elementów dostały angielskie zamienniki.
* Stylowanie elementów po id zostało zastąpione przez stylowanie po klasach.
* Zlikwidowano atrybuty [style] z elementów, zamiast tego, są stylowane po klasach w arkuszu.
* Definicja skryptu została przeniesiona przed tag </body>.

### Skrypt

* Całość została owinięta w IIFE, aby zmienne zadeklarowane wewnątrz niego nie przechodziły do scope'u globalnego.
* Kod podzielony został na funkcje, które odpowiadają konkretnym czynnościom w grze.
* Pozbyto się mieszania kodu HTML z kodem JS poprzez dynamiczne tworzenie elementów DOM.
