# Simple-queries
Exercise 2 - Homework PCLP 1

Problema 2 - Simple query pe litere

        Modularizam problema cu ajutorul headerului intitulat "function2.h"

        Citim litere introduse de la tastatura pana in momentul in care
    una dintre valori nu mai respecta conditia din do{ }while();
    (daca 'n', nu este litera mica a alfabetului sau 'Q','T','E','X')

        Prin intermediul structurii de decizie "switch" avem posibilitatea
    sa tratam fiecare caz special in parte:
        a) In cazul aparitiei literi 'Q' programul interogheaza numarul de aparitii
    a unui caracter 'L' citit de la tastatura;
        b) In cazul aparititei literei 'T' programul interogheaza Topul literelor,
    in functie de numarul de aparitii al fiecaruia. Parcurgem vectorul de frecventa,
    observam cel mai mare numar de aparitii si il memoram in variabila "max".
    Dupa ce am aflat maximul, mai parcurgem inca odata vectorul de frecventa si afisam
    literele cu numarul de aparitii == max. Totodata stergem numarul de aparitii al literei,
    deoarece urmeaza sa aflam urmatorul maxim. Vectorul "vf2" reprezinta o copie a vectorului
    initial "vf". Nu vrem sa l modificam pe "vf", deoarece vom avea nevoie de el ulterior.
        c) In cazul aparitiei literei 'E' se elimina numarul de aparitie 
    a unei litere 'L' citite de la tastatura;
        d) In cazul in care se introduc litere mici ale alfabetului, programul
    intra in 'default' si numara aparitiile literei respective. Totodata functia
    "alerta(f,u_a,vf)" afiseaza alerte in cazul in care este nevoie. Aceasta verifica fiecare
    conditie pusa in problema, iar daca una dintre acestea nu este respectata se va afisa 
    o alerta.

        Fiecare caz al problemei este modularizat prin functiile:
            numarul_de_aparitii
            topul_literelor
            eliminare_litera
