
# Instrukcja dla studentów: Praca z GitHub Classroom

## 1. Akceptacja Assignmentu

Po otrzymaniu linku do assignmentu z GitHub Classroom:

1. Kliknij link otrzymany od prowadzącego (np. na Teamsie, mailu lub Moodle).
2. Zaloguj się na swoje konto GitHub (lub załóż konto, jeśli jeszcze go nie masz).
3. Kliknij **"Accept the assignment"**.
4. GitHub Classroom automatycznie utworzy dla Ciebie prywatne repozytorium z szablonem projektu.
5. Po chwili pojawi się link do Twojego repozytorium — zapisz go lub kliknij, by przejść dalej.

## 2. Klonowanie repozytorium na komputer

1. Wejdź na stronę swojego repozytorium.
2. Kliknij zielony przycisk **"Code"**, a następnie skopiuj link (HTTPS lub SSH).
3. W terminalu/IDE wykonaj polecenie:

```bash
git clone <skopiowany_link>
```

Przykład:

```bash
git clone https://github.com/pjwstk-2024-programowanie/lab1-jan-kowalski.git
```

4. Przejdź do katalogu projektu:

```bash
cd lab1-jan-kowalski
```

## 3. Rozwiązanie zadania

1. Otwórz projekt w swoim edytorze (np. VS Code, IntelliJ, PyCharm, itp.).
2. Wprowadź wymagane zmiany w kodzie.
3. Zapisz pliki i upewnij się, że wszystko działa lokalnie.

## 4. Commitowanie zmian i wysyłanie na GitHub

Po zakończeniu prac:

```bash
git add .
git commit -m "Rozwiązanie zadania"
git push
```

Po `git push` Twoje zmiany zostaną wysłane do repozytorium na GitHubie.

## 5. (Opcjonalnie) Sprawdzanie wyników z GitHub Actions

Jeśli prowadzący przygotował workflow (CI/CD) w repozytorium:

1. Wejdź w zakładkę **Actions** na GitHubie.
2. Sprawdź status testów i automatycznych sprawdzeń.
3. Jeśli testy nie przeszły — kliknij na nie i przeanalizuj logi błędów.

## 6. Oddanie zadania

Zadanie jest uznawane za oddane, jeśli:

- Repozytorium zawiera Twoje rozwiązanie,
- (jeśli dotyczy) testy przeszły pomyślnie,
- Prowadzący ma dostęp do Twojego repozytorium (nie musisz nic więcej wysyłać, chyba że poprosił o link).

---

📌 **Pamiętaj:** Nie usuwaj repozytorium ani nie zmieniaj jego ustawień prywatności — prowadzący musi mieć do niego dostęp przez cały semestr.

Powodzenia! 💡🧑‍💻
