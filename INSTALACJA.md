# Instrukcja instalacji — The Pandora Directive

[Pobieranie i wymagania](https://marko22.pl/pobieranie#pandora) · [Wydanie GitHub](https://github.com/mariuszm22/The-Pandora-Directive-Spolszczenie-PL/releases/tag/v0.9.0-beta)

## INSTALACJA PRZEZ KREATOR

1. Zamknij grę i DOSBox. Uruchom **marko22-Instalator-Pandora-PL-0.9.0-Beta.exe**.
2. Wybierz **Zainstaluj spolszczenie**. Zatwierdź wykryty folder Steam lub wskaż katalog `Tex Murphy 4` zawierający folder `TEX4`.
3. Sprawdź podsumowanie i zatwierdź instalację. Kreator sprawdza zgodność plików i zapisuje kopie oryginałów.
4. Poczekaj na zakończenie weryfikacji i instalacji.

Wcześniejszą kompilację 0.9.0 Beta z 21 lub 22 plikami możesz zaktualizować z zachowaniem dotychczasowych kopii.

## INSTALACJA RĘCZNA Z ZIP

1. Zamknij grę i DOSBox. Wypakuj **Pandora_PL_0.9.0-Beta.zip** w całości do osobnego folderu.
2. Ustal katalog gry przez **Zarządzaj → Przeglądaj pliki lokalne** w Steam. W folderze z wypakowanymi plikami wpisz `powershell` w pasku adresu i naciśnij Enter.
3. W poniższych poleceniach zastąp przykładową ścieżkę pełną ścieżką do katalogu nadrzędnego gry. Uruchom weryfikację.

   ```powershell
   .\Instalacja_reczna.ps1 -FolderGry "C:\sciezka\Tex Murphy 4" -Operacja Sprawdz
   ```

4. Po pomyślnej weryfikacji uruchom instalację.

   ```powershell
   .\Instalacja_reczna.ps1 -FolderGry "C:\sciezka\Tex Murphy 4" -Operacja Zainstaluj
   ```

Przy aktualizacji wcześniejszego ZIP 0.9.0 Beta zachowaj kopię oryginałów. Przy zmianie metody instalacji przywróć oryginały metodą użytą poprzednio. Szczegóły są w **README_PL.txt** dołączonym do wydania.

## PO INSTALACJI

Uruchom grę przez Steam. Spolszczenie jest aktywne od początku. Wydanie sprawdzono z angielską wersją Steam, AppID 302360, BuildID 470847. Kreator wymaga Windows 10/11 x64 i .NET Framework 4.8. Instalacja ręczna używa Windows PowerShell 5.1.

## PRZYWRACANIE

Przy zamkniętej grze i DOSBoxie wybierz **Odinstaluj spolszczenie i przywróć oryginały** w kreatorze. Zachowaj katalog `.marko22-pandora` do potwierdzenia poprawnego przywrócenia.

Jeśli użyłeś ZIP, uruchom ten sam skrypt z operacją `Przywroc`:

```powershell
.\Instalacja_reczna.ps1 -FolderGry "C:\sciezka\Tex Murphy 4" -Operacja Przywroc
```

Kopie pozostają w `.marko22-pandora-reczny`. Zachowaj pliki skryptu i kopii do potwierdzenia poprawnego przywrócenia.

Projekt — https://marko22.pl/pandora
