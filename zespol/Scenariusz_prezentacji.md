# Scenariusz prezentacji na obronę
### Projekt FitFlow — System zarządzania klubem fitness (Inżynieria wymagań)

> Gotowy scenariusz wystąpienia na **~15–18 min** + pytania. Dla każdego segmentu: **kto mówi**,
> **co powiedzieć** (gotowe kwestie — można parafrazować), **ile czasu** i **co pokazać w dokumentacji**.
> Dokumentacja: [`../FitFlow_Dokumentacja.md`](../FitFlow_Dokumentacja.md).

## Obsada (role-playing)
| Osoba | Mówca | Rola interesariusza | Główne segmenty |
|---|---|---|---|
| **O1** | **Jakub Wiatr** | Klient / Właściciel | otwarcie, kontekst, wywiady, podsumowanie |
| **O2** | **Bartłomiej Podlewski** | Użytkownik końcowy | ankieta, wymagania funkcjonalne, user stories |
| **O3** | **Norbert Szopa** | Administrator (IT) | wymagania niefunkcjonalne, modelowanie, walidacja |
| **O4** | **Dawid Osak** | Biznes / Product Owner | priorytetyzacja, zarządzanie zmianą, SRS+Volere |

## Oś czasu wystąpienia
| # | Segment | Mówca(y) | Czas | Dokumentacja |
|---|---|---|--:|---|
| 0 | Otwarcie i przedstawienie | O1 | 1:00 | strona tytułowa |
| 1 | Problem i interesariusze | O1 | 1:30 | [Cz. I §3](../FitFlow_Dokumentacja.md#część-i--specyfikacja-wymagań-oprogramowania-srs) |
| 2 | Pozyskiwanie wymagań | O2 + O1 | 2:00 | [Cz. II](../FitFlow_Dokumentacja.md#część-ii--pozyskiwanie-wymagań) |
| 3 | Specyfikacja (FR/NFR, US/UC) | O2 + O3 | 2:30 | [Cz. I §4–§6](../FitFlow_Dokumentacja.md#część-i--specyfikacja-wymagań-oprogramowania-srs) |
| 4 | Modelowanie (diagramy) | O3 | 2:00 | [Cz. I §7](../FitFlow_Dokumentacja.md#część-i--specyfikacja-wymagań-oprogramowania-srs) |
| 5 | Priorytetyzacja | O4 | 1:30 | [Cz. III](../FitFlow_Dokumentacja.md#część-iii--priorytetyzacja-wymagań) |
| 6 | Walidacja | O3 | 1:30 | [Cz. IV](../FitFlow_Dokumentacja.md#część-iv--walidacja-wymagań) |
| 7 | Zarządzanie zmianą + scenka role-play | wszyscy | 3:30 | [Cz. V](../FitFlow_Dokumentacja.md#część-v--zarządzanie-zmianą), [Cz. VI](../FitFlow_Dokumentacja.md#część-vi--role-playing) |
| 8 | Dokumentacja SRS + Volere | O4 | 1:30 | [Cz. VII](../FitFlow_Dokumentacja.md#część-vii--dokumentacja-volere) |
| 9 | Podsumowanie | O1 | 1:00 | [Mapa punktacji](Podzial_pracy.md#mapa-punktacji-i-warunki-zaliczenia), [Spis treści](../FitFlow_Dokumentacja.md#spis-treści) |
| — | Pytania komisji | wszyscy | — | zob. [sekcja Q&A](#pytania-komisji--przygotowane-odpowiedzi) |

> **Obsługa ekranu:** dokument/diagramy przewija **O3** (ma najwięcej rysunków). Pokazujcie
> diagramy renderowane (Markdown na GitHub / PDF), nie surowy kod.

---

## Segment 0 — Otwarcie (O1, 1:00)

**Jakub (O1):**
> „Dzień dobry. Nazywam się Jakub Wiatr, a to mój zespół: Bartłomiej Podlewski, Norbert Szopa
> i Dawid Osak. Przedstawimy projekt z inżynierii wymagań — **FitFlow**, system zarządzania
> siecią klubów fitness. Przeprowadziliśmy **pełny proces inżynierii wymagań**: od identyfikacji
> problemu, przez pozyskiwanie i specyfikację wymagań, modelowanie, priorytetyzację i walidację,
> aż po zarządzanie zmianą. Pracowaliśmy metodą **role-playing** — każdy z nas wcielił się
> w innego interesariusza. Ja reprezentowałem **klienta — właściciela sieci klubów**."

---

## Segment 1 — Problem i interesariusze (O1, 1:30) · *obszar 1*

**Jakub (O1):** *(pokaż mapę interesariuszy — [Cz. I §3](../FitFlow_Dokumentacja.md#część-i--specyfikacja-wymagań-oprogramowania-srs))*
> „Naszym klientem jest fikcyjna, ale realistyczna sieć **Vitality Fitness** — trzy kluby,
> z planem rozrostu do sześciu. Problem: wszystko działa **ręcznie** — grafik w arkuszu,
> papierowe karnety, rezerwacje telefoniczne, rozliczenia w zeszycie. Skutki to kolejki na
> recepcji, błędy w rozliczeniach, tzw. **martwe karnety** i — co najważniejsze dla mnie jako
> właściciela — **brak danych do decyzji** i trudność skalowania na kolejne kluby.
>
> Zidentyfikowaliśmy **dziesięciu interesariuszy** i ułożyliśmy ich na **mapie wpływu i
> zainteresowania**. Kluczowi gracze to właściciel i manager — nimi trzeba zarządzać ściśle.
> Użytkownicy końcowi — członkowie, trenerzy, recepcja — to grupa o wysokim zainteresowaniu,
> którą trzeba na bieżąco informować i włączać. To właśnie te perspektywy odegraliśmy w zespole."

---

## Segment 2 — Pozyskiwanie wymagań (O2 + O1, 2:00) · *obszar 2*

**Bartłomiej (O2):** *(pokaż [Cz. II](../FitFlow_Dokumentacja.md#część-ii--pozyskiwanie-wymagań))*
> „Bartłomiej Podlewski — w zespole odpowiadałem za specyfikację i ankietę, a w role-playingu
> grałem **użytkownika końcowego**. Wymagania pozyskaliśmy **trzema technikami**, choć wymagane
> były dwie — świadomie zastosowaliśmy **triangulację**, żeby ograniczyć błąd pojedynczej metody:
> **wywiady** z decydentami, **ankietę** wśród członków i **analizę konkurencji**.
>
> Ankietę wypełniło **62 członków**. Najważniejsze wyniki: **89%** chce rezerwować zajęcia
> online, **81%** chce płacić online, a check-in kodem QR oceniono na **4,1 na 5**. To dało nam
> twarde dane do priorytetów."

**Jakub (O1):**
> „Ja, jako właściciel, byłem rozmówcą w **wywiadzie W-1**. Z wywiadów wyszły cele biznesowe —
> przychód, odnowienia, raporty — oraz **konflikt**, który rozstrzygnęliśmy później: sprawa
> kart partnerskich typu Multisport. Tam, gdzie wszystkie trzy źródła były zgodne, wymaganie
> dostawało wysoki priorytet i niskie ryzyko."

---

## Segment 3 — Specyfikacja wymagań (O2 + O3, 2:30) · *obszar 3*

**Bartłomiej (O2):** *(pokaż [Cz. I §4](../FitFlow_Dokumentacja.md#część-i--specyfikacja-wymagań-oprogramowania-srs))*
> „Specyfikacja zawiera **25 wymagań funkcjonalnych** w 11 modułach — przy wymaganym minimum
> 15–20. Przykłady serca systemu: **FR-008** — rezerwacja zajęć, **FR-009** — lista rezerwowa
> z automatycznym awansem, **FR-013** — check-in kodem QR z weryfikacją karnetu. Każde wymaganie
> ma identyfikator, priorytet i źródło. Do tego napisaliśmy **10 historyjek użytkownika** oraz
> **6 pełnych przypadków użycia** — ze scenariuszem głównym i alternatywnymi, np. UC-02 rezerwacja
> zajęć z obsługą braku miejsc."

**Norbert (O3):** *(pokaż [Cz. I §5](../FitFlow_Dokumentacja.md#część-i--specyfikacja-wymagań-oprogramowania-srs))*
> „Norbert Szopa — odpowiadałem za wymagania niefunkcjonalne, modelowanie i walidację; rola:
> **administrator**. Mamy **15 wymagań niefunkcjonalnych** według normy **ISO 25010** — wydajność,
> bezpieczeństwo, niezawodność, użyteczność, zgodność. Kluczowe: każde z nich ma **mierzalne
> kryterium akceptacji** — np. NFR-001: *95% żądań poniżej 2 sekund*, czy NFR-006: zgodność
> z **RODO** i realizacja prawa do bycia zapomnianym w 30 dni. Dzięki temu wymagania są
> **testowalne**, a nie ogólnikowe."

---

## Segment 4 — Modelowanie (O3, 2:00) · *obszar 4*

**Norbert (O3):** *(pokazuj kolejno diagramy — [Cz. I §7](../FitFlow_Dokumentacja.md#część-i--specyfikacja-wymagań-oprogramowania-srs))*
> „Przygotowaliśmy **sześć diagramów**. **Diagram kontekstowy** pokazuje granicę systemu i
> integracje — bramkę płatniczą, powiadomienia, operatora kart. **Diagram przypadków użycia**
> wiąże aktorów z funkcjami. Proces sprzedaży karnetu opisaliśmy w **notacji BPMN** z torami
> — od wyboru karnetu, przez płatność, po aktywację i wysłanie kodu QR. Domenę pokazuje
> **diagram klas**, a przebieg rezerwacji — **diagram sekwencji**. Wszystkie diagramy są
> w dokumentacji jako Mermaid i renderują się bezpośrednio w pliku."

*(Jeśli mało czasu: omów na żywo tylko diagram przypadków użycia i BPMN, resztę wymień.)*

---

## Segment 5 — Priorytetyzacja (O4, 1:30) · *obszar 5*

**Dawid (O4):** *(pokaż [Cz. III](../FitFlow_Dokumentacja.md#część-iii--priorytetyzacja-wymagań))*
> „Dawid Osak — byłem menedżerem wymagań i **Product Ownerem**; rola: **biznes**. Wymagania
> spriorytetyzowaliśmy metodą **MoSCoW**: 14 funkcji **Must**, 8 **Should**, 3 **Could**.
> Priorytety nie są uznaniowe — oceniliśmy każde wymaganie w **czterech kryteriach**: wartość
> biznesowa, popyt użytkowników, ryzyko braku i zależności. Dodatkowo zrobiliśmy analizę
> **Kano** — rozróżniającą funkcje podstawowe, jak check-in, od **'zachwycaczy'**, jak lista
> rezerwowa, która jest tanią przewagą nad konkurencją. Z priorytetów wynika **zakres MVP**."

---

## Segment 6 — Walidacja (O3, 1:30) · *obszar 6*

**Norbert (O3):** *(pokaż [Cz. IV](../FitFlow_Dokumentacja.md#część-iv--walidacja-wymagań))*
> „Wymagania zwalidowaliśmy na trzy sposoby. Po pierwsze, **checklist jakości** — sprawdziliśmy
> jednoznaczność, kompletność, weryfikowalność i atomowość. Wykrył on realne defekty — na
> przykład konflikt: czy z **zamrożonym** karnetem można zrobić check-in? Dopisaliśmy regułę.
> Po drugie, **12 scenariuszy testowych** w formacie *Given–When–Then*, w tym przypadki
> negatywne. Po trzecie, **macierz śledzenia** wiążąca źródło → wymaganie → przypadek użycia →
> test → interesariusza. Sprawdziliśmy, że żadne wymaganie Must nie jest **'sierotą'** — każde
> ma test."

---

## Segment 7 — Zarządzanie zmianą + scenka role-play (wszyscy, 3:30) · *obszary 7 i 8*

**Dawid (O4) — wprowadzenie (40 s):** *(pokaż [Cz. V](../FitFlow_Dokumentacja.md#część-v--zarządzanie-zmianą))*
> „To był **twist projektowy**. Zaproponowaliśmy **trzy zmiany wymagań**: CR-01 — sprzedaż online
> i subskrypcje; CR-02 — wejście **nowego interesariusza**, operatora kart partnerskich;
> i CR-03 — moduł zajęć online. Dla każdej przeprowadziliśmy **analizę wpływu** — co dotyka,
> jaki wysiłek, ryzyko i koszt. Pokażemy to na przykładzie CR-02, bo wywołał **konflikt**.
> Odegramy krótko nasze stanowiska."

**🎭 Scenka — Change Board (CR-02: karty partnerskie), ~1:40:**

**Jakub (Właściciel):**
> „Jako właściciel chcę kart Multisport **już teraz** — konkurencja je ma, a to gotowy strumień
> nowych członków."

**Norbert (Administrator):**
> „Jako administrator się nie zgadzam bez zabezpieczeń. To **nowy interesariusz**, przekazujemy
> mu dane wejść — potrzebna **umowa powierzenia** zgodnie z RODO. I rozliczenia: bez **audytu
> wejść** narażamy się na spór finansowy z operatorem."

**Bartłomiej (Użytkownik/Trener):**
> „Z perspektywy klubu — 'kartowicze' potrafią zająć popularne zajęcia i odwołać w ostatniej
> chwili. Stali członkowie się zniechęcą. Potrzebny **limit miejsc** kartowych na zajęcia."

**Dawid (Product Owner):**
> „Godzę te stanowiska: przyjmujemy CR-02, ale jako **Should**, po MVP, z trzema warunkami
> wpisanymi do wymagań — audyt wejść, konfigurowalny limit i umowa powierzenia danych. Konflikt
> rozwiązany **negocjacją**, nie głosowaniem — każda obawa stała się konkretnym wymaganiem."

**Dawid (O4) — domknięcie (40 s):**
> „I odpowiadamy na kluczowe pytanie projektu: **co się dzieje z systemem, gdy zmienia się
> wymaganie?** Zmiana **nigdy nie jest lokalna** — propaguje się po śladzie: wymaganie → przypadki
> użycia → modele → testy → priorytety. Dlatego utrzymujemy **macierz śledzenia** i **wersjonujemy**
> dokument: baseline 1.0, a po zmianach wersja **1.1** z wpisem w historii. Tak zmiana pozostaje
> **kontrolowana i spójna**."

---

## Segment 8 — Dokumentacja SRS + Volere (O4, 1:30) · *obszar 9*

**Dawid (O4):** *(pokaż [Cz. VII](../FitFlow_Dokumentacja.md#część-vii--dokumentacja-volere))*
> „Cała dokumentacja spełnia **dwa standardy** wymagane do zaliczenia. Struktura to **SRS**
> według IEEE 830 i ISO 29148 — wprowadzenie, opis ogólny, wymagania, modele, interfejsy.
> Dodatkowo zastosowaliśmy podejście **Volere**: każde wymaganie ma **kryterium akceptacji
> (fit criterion)**, a kluczowe wymagania zapisaliśmy w pełnym szablonie **Volere Requirements
> Shell** — z polami rationale, źródło, priorytet, konflikty i historia. Pokazaliśmy też
> **mapowanie** sekcji szablonu Volere na nasze części. Oba warunki — SRS i Volere — są spełnione."

---

## Segment 9 — Podsumowanie (O1, 1:00)

**Jakub (O1):** *(pokaż [Mapę punktacji](Podzial_pracy.md#mapa-punktacji-i-warunki-zaliczenia) lub [Spis treści](../FitFlow_Dokumentacja.md#spis-treści))*
> „Podsumowując: przeszliśmy **pełny cykl inżynierii wymagań** dla systemu FitFlow.
> Efekt to **25 wymagań funkcjonalnych**, **15 niefunkcjonalnych** z mierzalnymi kryteriami,
> **6 diagramów**, priorytetyzacja MoSCoW i Kano, walidacja z macierzą śledzenia oraz
> **trzy zmiany** przeanalizowane pod kątem wpływu — w pełnym role-playingu czterech
> interesariuszy. Dokumentacja jest zgodna ze standardem **SRS** i podejściem **Volere**.
> Dziękujemy za uwagę — chętnie odpowiemy na pytania."

---

## Pytania komisji — przygotowane odpowiedzi

> **Zasada:** na pytanie odpowiada osoba 'właściciel' danego obszaru; inni mogą uzupełnić.

| Prawdopodobne pytanie | Odpowiada | Szkic odpowiedzi |
|---|---|---|
| Skąd dane w ankiecie i wywiadach? | O2/O1 | **Uczciwie:** to scenariusz **role-playing** — dane są syntetyczne, ale realistyczne (oparte na researchu rynku). Wcieliliśmy się w interesariuszy, by przeanalizować wymagania z wielu perspektyw. |
| Dlaczego MoSCoW, a nie ocena liczbowa? | O4 | MoSCoW jest czytelne dla biznesu i wprost wyznacza **zakres MVP** (Must = release 1). Uzupełniliśmy je o Kano dla rozróżnienia funkcji 'podstawowych' i 'zachwycających'. |
| Jak zapewniliście **testowalność** wymagań? | O3 | Każde NFR ma **fit criterion** (np. 95% < 2 s), a Must-FR mają scenariusze testowe Given–When–Then i wpis w **macierzy śledzenia**. |
| Czym jest **Volere** i fit criterion? | O4 | Volere to metoda i szablon wymagań; **fit criterion** to mierzalne kryterium, po którym poznamy, że wymaganie jest spełnione — czyni je testowalnym. |
| Dlaczego akurat te techniki pozyskiwania? | O1/O2 | **Triangulacja**: wywiady dają 'dlaczego' od decydentów, ankieta — ilościowy głos masy użytkowników, analiza konkurencji — bazowy zakres rynkowy. |
| Jak rozwiązaliście **konflikt** wymagań? | O1/O4 | Na przykładzie kart partnerskich: warsztat negocjacyjny, w którym każda obawa (RODO, rozliczenia, obłożenie) stała się konkretnym warunkiem/wymaganiem. |
| Co z **bezpieczeństwem i RODO**? | O3 | NFR-003–007: TLS, RBAC, audyt, RODO i PCI-DSS (tokenizacja — brak przechowywania danych kart). |
| Co się dzieje, gdy **zmienia się wymaganie**? | O4/O3 | Propagacja po śladzie (wymaganie→UC→model→test→priorytet), analiza wpływu, aktualizacja i **wersjonowanie** dokumentu. |
| Co byście zrobili inaczej / największe ryzyko? | O4 | Zajęcia online (CR-03) — wysoki koszt, niepewny popyt; dlatego **odroczone** do pilotażu, a nie wpychane do MVP. |
| Dlaczego wybraliście ten temat / system? | O1 | Bogaci, wyraźni interesariusze i realne konflikty (właściciel vs. administrator vs. użytkownik) — idealny do pełnego procesu i role-playingu. |

---

## Wskazówki dla zespołu (delivery)
- **Czas:** ćwiczcie z zegarem; jak goni czas, skróćcie segment 4 (modelowanie) do 2 diagramów.
- **Płynne przejścia:** kończąc swój fragment, zapowiedz następnego: *„…a o wymaganiach
  niefunkcjonalnych powie Norbert"*.
- **Patrzcie na komisję**, nie na ekran; diagram komentujcie, nie czytajcie z niego.
- **Scenka role-play** (segment 7) to mocny punkt — odegrajcie ją z przekonaniem, to bezpośrednio
  punktowany obszar 8.
- **Każdy musi się odezwać** — to warunek zaliczenia. Podział mówienia jest mniej więcej równy
  (~4–5 min na osobę z pytaniami).
- **Na trudne pytanie** spokojnie: *„Dobre pytanie — w dokumentacji rozwiązaliśmy to w…"* i pokażcie
  odpowiednią część (linki w tabeli powyżej).
- **Plan B na diagramy:** miejcie pod ręką wersję **PDF/HTML** dokumentacji (z wypalonymi
  diagramami), gdyby czytnik na sali nie renderował Mermaid.
