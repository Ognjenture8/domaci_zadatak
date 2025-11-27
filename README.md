# Domaci zadatak iz Tehnicke dokumentacije

## Zadatak 

Program koji na osnovu unete duzine **dijagonale** kvadrata d izracunava **Povrsinu** kvadrata P

$$
\frac{1}{2} d^2
$$

### Algoritamska sema

![Algoritamsko resenje zadatka](zadatak.png)

## Resenje

''' cs


using System;

class Program
{
    static void Main()
    {
        // Unos dijagonale kvadrata
        Console.Write("Unesite dijagonalu kvadrata d: ");
        double d = double.Parse(Console.ReadLine());

        // Racunanje povrsine kvadrata
        double P = 0.5 * d * d;

        // Ispis rezultata
        Console.WriteLine("Površina kvadrata iznosi: " + P);

        Console.ReadLine();
    }
}
'''

### Test primeri

prvi test primeri:

''' text
Unesite dijagonalu kvadrata d: 12
Povrsina kvadrata iznosi: 72


C:\Users\ognje\source\repos\ConsoleApp1\ConsoleApp1\bin\Debug\ConsoleApp1.exe (process 25436) exited with code 0 (0x0).
To automatically close the console when debugging stops, enable Tools->Options->Debugging->Automatically close the console when debugging stops.
Press any key to close this window . . .
'''

Drugi test primeri:

''' text

Unesite dijagonalu kvadrata d: 4.28
Povrsina kvadrata iznosi: 9.1592


C:\Users\ognje\source\repos\ConsoleApp1\ConsoleApp1\bin\Debug\ConsoleApp1.exe (process 13568) exited with code 0 (0x0).
To automatically close the console when debugging stops, enable Tools->Options->Debugging->Automatically close the console when debugging stops.
Press any key to close this window . . .

### Objekti

| Redni broj | Naziv promenljive | Tip promeljive |
| _ _ _ _ _ _| _ _ _ _ _ _ _ _ _ | _ _ _ _ _ _ _ _|
| 1.         | 'd'               | 'double'       |
| 2.         | 'P'               | 'double'       |
