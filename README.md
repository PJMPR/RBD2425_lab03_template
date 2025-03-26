
# 🧪 Zadanie – Implementacja bazy danych na podstawie ERD

## 🔍 Kontekst
Na poprzednich zajęciach zaprojektowaliście diagram ERD dla jednej z dwóch tematycznych baz danych:
- System zarządzania szpitalem 🏥
- System zarządzania zakładem samochodowym 🚗

Na podstawie tego diagramu przygotujcie komplet skryptów SQL służących do implementacji fizycznego modelu bazy danych.

---

## 🎯 Cel zadania

Twoim zadaniem jest przygotowanie **trzech oddzielnych skryptów SQL**, które wykonają następujące kroki:

---

### 🧱 1. Skrypt: Tworzenie tabel (bez relacji)

Przygotuj plik `01_create_tables.sql`, który:

- Tworzy wszystkie tabele wynikające z Twojego diagramu ERD.
- Zawiera poprawnie zdefiniowane:
  - typy danych (`INT`, `VARCHAR`, `DATE`, itp.),
  - klucze główne (`PRIMARY KEY`),
  - ograniczenia:
    - `NULL` / `NOT NULL`
    - `DEFAULT`
    - `CHECK` (np. sprawdzanie poprawności zakresu danych)
- Nie zawiera jeszcze kluczy obcych (`FOREIGN KEY`).

---

### 🔗 2. Skrypt: Tworzenie relacji

Przygotuj plik `02_add_foreign_keys.sql`, który:

- Dodaje relacje pomiędzy tabelami za pomocą:
  
```sql
ALTER TABLE ... ADD CONSTRAINT ... FOREIGN KEY (...) REFERENCES ...(...);
```

- Pamiętaj o:
  - nadawaniu **czytelnych nazw** ograniczeń (`fk_nazwa_tabeli_nazwa_kolumny`),
  - poprawnym wskazaniu kolumn i tabel docelowych,
  - opcjonalnie użyj `ON DELETE` / `ON UPDATE`.

---

### 🧾 3. Skrypt: Przykładowe dane

Przygotuj plik `03_sample_data.sql`, który:

- Dodaje po **co najmniej 10 rekordów do każdej tabeli**,
- Przestrzega spójności danych (relacje muszą być zachowane),
- Dane mogą być fikcyjne, ale realistyczne (np. imiona pacjentów, marki aut, daty wizyt itp.).

---

## ✅ Wskazówki

- Wszystkie skrypty powinny działać niezależnie od siebie i być możliwe do uruchomienia w MariaDB.
- Przed każdym skryptem możesz dodać komentarze `--` objaśniające, co się dzieje.
- Zadbaj o przejrzystość i konsekwencję nazewnictwa tabel i kolumn.
- Użyj `IF NOT EXISTS` lub `DROP TABLE` (opcjonalnie) w celach testowych.

---

## 📦 Co oddajecie?

- `01_create_tables.sql` – definicje tabel
- `02_add_foreign_keys.sql` – relacje
- `03_sample_data.sql` – dane testowe

---

## 🧠 Cel edukacyjny

To zadanie pozwala przećwiczyć:
- tworzenie fizycznego modelu bazy danych,
- użycie ograniczeń (`CHECK`, `DEFAULT`, `NOT NULL`, `UNIQUE`),
- tworzenie i zarządzanie relacjami (`FOREIGN KEY`),
- wypełnianie tabel sensownymi danymi.

---

**Powodzenia!** 💡
