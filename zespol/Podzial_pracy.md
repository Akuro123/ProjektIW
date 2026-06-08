# Podział pracy w zespole
### Projekt FitFlow — Inżynieria wymagań (zespół 4-osobowy)

> Osobny dokument opisujący **zakres odpowiedzialności każdej z 4 osób**. Przypisuje
> członkom zespołu: (1) **rolę interesariusza** w role-playingu, (2) **obszary punktowane**,
> (3) **konkretne części/sekcje** dokumentacji, (4) **szacowany nakład**.

## 1. Skład zespołu i role

| Osoba | Imię i nazwisko        | Rola w projekcie | Rola w role-playingu |
|---|------------------------|---|---|
| **Osoba 1** | _Jakub Wiatr_          | Analityk biznesowy / Lider kontekstu | **Klient / Sponsor** (Właściciel sieci) |
| **Osoba 2** | _Bartłomiej Podlewski_ | Inżynier wymagań / Specyfikacja | **Użytkownik końcowy** (Członek / Trener) |
| **Osoba 3** | _Norbert Szopa_        | Architekt / Modelarz / QA | **Administrator** (IT / Recepcja) |
| **Osoba 4** | _Dawid Osak_           | Menedżer wymagań / Product Owner | **Biznes** (Manager operacyjny) |

---

## 2. Szczegółowe zakresy odpowiedzialności

### 👤 Osoba 1 — Analityk biznesowy (rola: KLIENT / Właściciel)
**Cel roli:** reprezentuje perspektywę biznesową i sponsora — przychód, retencja, ekspansja.

| Obszar punktowany | Wkład |
|---|---|
| **1. Kontekst i interesariusze** (5 pkt) | Identyfikacja użytkowników, mapa interesariuszy, opis kontekstu i problemu biznesowego. |
| **2. Pozyskiwanie wymagań** (współudział) | Prowadzenie/odegranie wywiadu W-1 (Właściciel); współudział w W-2/W-3. |
| **7. Zarządzanie zmianą** (część biznesowa) | Zgłoszenie i uzasadnienie biznesowe CR-01 i CR-02; argumentacja w Change Board. |

**Części dokumentacji:**
- [Część I — SRS](../FitFlow_Dokumentacja.md#część-i--specyfikacja-wymagań-oprogramowania-srs) — §2.3 (użytkownicy), §3 (interesariusze, mapa, kontekst).
- [Część II — Pozyskiwanie](../FitFlow_Dokumentacja.md#część-ii--pozyskiwanie-wymagań) — §2.1 (wywiad W-1), współautor §1.
- [Część V — Zarządzanie zmianą](../FitFlow_Dokumentacja.md#część-v--zarządzanie-zmianą) — opis biznesowy CR-01, CR-02.
- [Część VI — Role-playing](../FitFlow_Dokumentacja.md#część-vi--role-playing) — rola Klient (§1, §2, §3).

**Szacowany nakład:** ~25% (lider sekcji kontekstowej i biznesowej).

---

### 👤 Osoba 2 — Inżynier wymagań (rola: UŻYTKOWNIK końcowy)
**Cel roli:** reprezentuje członka klubu i trenera — wygoda, prostota, codzienne potrzeby.

| Obszar punktowany | Wkład |
|---|---|
| **3. Specyfikacja wymagań** (część FR) | Wymagania funkcjonalne (FR-001…FR-025), user stories, przypadki użycia. |
| **2. Pozyskiwanie wymagań** (ankieta) | Projekt i analiza ankiety (głos użytkowników). |

**Części dokumentacji:**
- [Część I — SRS](../FitFlow_Dokumentacja.md#część-i--specyfikacja-wymagań-oprogramowania-srs) — §4 (wymagania funkcjonalne), §6 (user stories + UC).
- [Część II — Pozyskiwanie](../FitFlow_Dokumentacja.md#część-ii--pozyskiwanie-wymagań) — §3 (ankieta) + współautor W-2 (trener).
- [Część VI — Role-playing](../FitFlow_Dokumentacja.md#część-vi--role-playing) — rola Użytkownik (§1, §2, §3).

**Szacowany nakład:** ~25% (największa część specyfikacji funkcjonalnej).

---

### 👤 Osoba 3 — Architekt / Modelarz / QA (rola: ADMINISTRATOR)
**Cel roli:** reprezentuje IT i recepcję — bezpieczeństwo, niezawodność, utrzymanie, zgodność.

| Obszar punktowany | Wkład |
|---|---|
| **3. Specyfikacja wymagań** (część NFR) | Wymagania niefunkcjonalne (NFR-001…NFR-015) wg ISO 25010 z fit criteria. |
| **4. Modelowanie** (5 pkt) | Wszystkie diagramy: kontekstowy, przypadków użycia, BPMN, klas, sekwencji. |
| **6. Walidacja** (5 pkt) | Checklist jakości, scenariusze testowe, ocena spójności/kompletności, macierz śledzenia. |

**Części dokumentacji:**
- [Część I — SRS](../FitFlow_Dokumentacja.md#część-i--specyfikacja-wymagań-oprogramowania-srs) — §5 (NFR), §7 (modele), §8 (interfejsy).
- [Część IV — Walidacja](../FitFlow_Dokumentacja.md#część-iv--walidacja-wymagań) — całość.
- [Część VI — Role-playing](../FitFlow_Dokumentacja.md#część-vi--role-playing) — rola Administrator (§1, §2, §3).

**Szacowany nakład:** ~28% (modele + walidacja + NFR — duży zakres techniczny).

---

### 👤 Osoba 4 — Menedżer wymagań / Product Owner (rola: BIZNES)
**Cel roli:** spina całość — priorytety, zakres, kontrola zmian, zgodność ze standardem.

| Obszar punktowany | Wkład |
|---|---|
| **5. Priorytetyzacja** (5 pkt) | MoSCoW + uzasadnienia + analiza Kano. |
| **7. Zarządzanie zmianą** (7 pkt) | Proces zmian, impact analysis, wersjonowanie, prowadzenie Change Board. |
| **9. Dokumentacja SRS + Volere** (5 pkt) | Spójność standardu SRS, karty Volere, fit criteria, mapowanie struktury; scalanie dokumentów. |

**Części dokumentacji:**
- [Część III — Priorytetyzacja](../FitFlow_Dokumentacja.md#część-iii--priorytetyzacja-wymagań) — całość.
- [Część V — Zarządzanie zmianą](../FitFlow_Dokumentacja.md#część-v--zarządzanie-zmianą) — proces i impact analysis.
- [Część VII — Volere](../FitFlow_Dokumentacja.md#część-vii--dokumentacja-volere) — całość.
- [Mapa punktacji](../FitFlow_Dokumentacja.md#mapa-punktacji-i-warunki-zaliczenia) — koordynacja spójności całej dokumentacji.
- [Część VI — Role-playing](../FitFlow_Dokumentacja.md#część-vi--role-playing) — rola Biznes/PO (§1, §2, §3).

**Szacowany nakład:** ~22% (koordynacja + 3 obszary).

---

## 3. Obszar wspólny — Role-playing (obszar 8, 3 pkt)
Role-playing jest **realizowany przez wszystkich** — każdy odgrywa swoją rolę podczas
wywiadów, warsztatu negocjacyjnego i Change Board ([Część VI — Role-playing](../FitFlow_Dokumentacja.md#część-vi--role-playing)).
Koordynację sesji i spisanie transkrypcji prowadzi **Osoba 1**, ale wkład wnoszą wszyscy.

---

## 4. Macierz odpowiedzialności RACI

**R** = wykonuje · **A** = odpowiedzialny/zatwierdza · **C** = konsultowany · **I** = informowany

| Obszar punktowany (pkt) | Osoba 1 | Osoba 2 | Osoba 3 | Osoba 4 |
|---|:--:|:--:|:--:|:--:|
| 1. Kontekst i interesariusze (5) | **R/A** | C | C | I |
| 2. Pozyskiwanie wymagań (7) | **R** | **R/A** | C | C |
| 3. Specyfikacja FR (z 8) | C | **R/A** | C | C |
| 3. Specyfikacja NFR (z 8) | I | C | **R/A** | C |
| 4. Modelowanie (5) | I | C | **R/A** | C |
| 5. Priorytetyzacja (5) | C | C | C | **R/A** |
| 6. Walidacja (5) | I | C | **R/A** | C |
| 7. Zarządzanie zmianą (7) | C | I | C | **R/A** |
| 8. Role-playing (3) | **R/A** | R | R | R |
| 9. Dokumentacja SRS+Volere (5) | C | C | C | **R/A** |

---

## 5. Bilans nakładu i warunek prezentacji

| Osoba | Główne obszary | Przybliżony udział |
|---|---|---|
| Osoba 1 | 1, część 2, część 7, role-playing | ~25% |
| Osoba 2 | część 3 (FR), część 2 | ~25% |
| Osoba 3 | część 3 (NFR), 4, 6 | ~28% |
| Osoba 4 | 5, 7, 9 + koordynacja | ~22% |

> **Warunek zaliczenia:** w prezentacji projektu (na zajęciach lub w sesji) **biorą udział
> wszyscy** członkowie zespołu. Sugerowany podział prezentacji pokrywa się z zakresami
> powyżej: każda osoba omawia obszary, za które odpowiada, oraz swoją rolę w role-playingu.
