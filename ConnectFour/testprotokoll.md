Wenn bspw. eine Spalte voll ist und man dann in der gleichen Reihe ein "x" oder "o" setzen möchte, dann stürzt das Programm ab:
Player x: 0
0 1 2 3 4 5 6 
o _ _ _ _ _ _
x _ _ _ _ _ _
o _ _ _ _ _ _
x _ _ _ _ _ _
o _ _ _ _ _ _
x _ _ _ _ _ _
Unhandled exception. System.IndexOutOfRangeException: Index was outside the bounds of the array.


Insgesamt gibt es 7 Spalten (0-6): wenn man also bspw. die Zahl "7" eingibt, stürzt das Programm ab:
0 1 2 3 4 5 6
_ _ _ _ _ _ _
_ _ _ _ _ _ _
_ _ _ _ _ _ _
_ _ _ _ _ _ _
_ _ _ _ _ _ _
_ _ _ _ _ _ _
Player x: 7
Unhandled exception. System.IndexOutOfRangeException: Index was outside the bounds of the array.


Das Programm stürzt ebenfalls ab, wenn man eine negative Zahl eingibt:
0 1 2 3 4 5 6
_ _ _ _ _ _ _
_ _ _ _ _ _ _
_ _ _ _ _ _ _
_ _ _ _ _ _ _
_ _ _ _ _ _ _
_ _ _ _ _ _ _
Player x: -4
Unhandled exception. System.IndexOutOfRangeException: Index was outside the bounds of the array.


Auch stürzt das Programm ab, wenn man eine Kommazahl eingibt:
0 1 2 3 4 5 6 
_ _ _ _ _ _ _
_ _ _ _ _ _ _
_ _ _ _ _ _ _
_ _ _ _ _ _ _
_ _ _ _ _ _ _
_ _ _ _ _ _ _
Player x: 0.3
Unhandled exception. System.FormatException: The input string '0.3' was not in a correct format.


Wenn man ein Buchstaben eingibt, stürzt das Programm ab:
0 1 2 3 4 5 6 
_ _ _ _ _ _ _
_ _ _ _ _ _ _
_ _ _ _ _ _ _
_ _ _ _ _ _ _
_ _ _ _ _ _ _
_ _ _ _ _ _ _
Player x: a
Unhandled exception. System.FormatException: The input string 'a' was not in a correct format.


Nach einer gewissen Angabe legt das Programm einen Sieger fest, obwohl dieser noch gar nicht gewonnen hat:
0 1 2 3 4 5 6 
_ _ _ _ _ _ _
x x o o x o x
o x x x o x o
x o o o x x o
o x x o o o x
x x o o x x o
Player x: A winner is you!