# Sprawdź, czy plik był zmodyfikowany od ostatniego pobrania
if git diff --quiet ppcw2; 

then
    # Plik nie był zmodyfikowany, więc nie robimy nic
    echo "Plik ppcw2 nie został zmodyfikowany od ostatniego pobrania."

else    
    # Plik był zmodyfikowany, dodaj go do przechowalni i zatwierdź zmiany
    git add ppcw2
    git commit -m "Zaktualizuj plik ppcw2: dodaj funkcję XYZ"

fi
# Wyświetl historię zatwierdzeń
git log
