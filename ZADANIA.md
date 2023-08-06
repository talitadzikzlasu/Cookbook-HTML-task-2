# Interaktywna Książka Przepisów

**Cel:** 
Stworzenie strony zawierającej listę przepisów kulinarnych w formie "karty" dla każdego przepisu. Strona ma być responsywna i dostosowana do różnych rozmiarów ekranu.

## Instrukcje:

1. **Struktura HTML dla listy przepisów:** 
   - Każdy przepis powinien mieć tytuł, krótki opis oraz miniaturkę.

2. **Stylizacja karty przepisu za pomocą Flexbox:** 
   - Ustal style dla karty przepisu, aby elementy wewnątrz były odpowiednio rozmieszczone.
   
3. **Pełne szczegóły przepisu:** 
   - Utwórz sekcję, która będzie zawierała pełne szczegóły wybranego przepisu, ale domyślnie będzie ukryta.
   - (bez javascript jest to troche trudniejsze, ale do zrobienia, na przyklad uzywajac elementu checkbox
    ```<div class="recipe">
    <input type="checkbox" id="recipe1-toggle" class="toggle">
    <label for="recipe1-toggle" class="recipe-summary">Tytuł i krótki opis przepisu</label>
    <div class="recipe-details">
        Pełne szczegóły przepisu...
    </div>
    </div>
    ```
    css:
    ```
    .toggle {
        display: none;
    }

    .recipe-details {
        display: none;
    }

    .toggle:checked + .recipe-summary + .recipe-details {
        display: block;
    }
    ```
   )

4. **Stylizacja pełnych szczegółów przepisu z Flexbox:** 
   - Nadaj odpowiednie style dla szczegółów przepisu, korzystając z właściwości Flexbox.

5. **Interakcja z kartą przepisu:** 
   - po kliknieciu przepisu, wyswietl jego pelne szczegoly

6. **Dodaj animację:** 
   - Ustal animację dla pojawiania się szczegółów przepisu przy użyciu klucza `@keyframes`.

7. **Ustal nawigację:** 
   - Dodaj 2 dodatkowe sekcje strony 
   - Dodaj górny pasek nawigacji, który pozwala na nawigację między różnymi sekcjami strony. 

8. **Responsywność z Flexbox i Media Queries:** 
   - Ustal różne układy dla różnych rozmiarów ekranu.

9. **Dodaj formularz dodawania przepisów:** 
   - Utwórz formularz, który pozwala użytkownikom na dodawanie własnych przepisów. (bez funkcjonalnosci, jedynie elementy input, textarea, form i button)

10. **Stylizacja formularza:** 
   - Ustal style dla formularza, aby był atrakcyjny wizualnie i zgodny z ogólnym wyglądem strony.
