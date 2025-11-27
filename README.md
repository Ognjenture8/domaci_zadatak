# Domaci zadatak iz Tehnicke dokumentacije

## Zadatak 

Program koji na osnovu unete duzine **dijagonale** kvadrata d izracunava **Povrsinu** kvadrata P

## formula
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
        Console.WriteLine("Program za izračunavanje površine kvadrata.");
        Console.WriteLine("Formula: P = 1/2 * d^2");
        
        // Unos dijagonale
        Console.Write("Unesite dijagonalu kvadrata d: ");
        double d;
        
        // Provera da li je unos validan
        if (double.TryParse(Console.ReadLine(), out d) && d > 0)
        {
            // Računanje površine
            double P = 0.5 * d * d;
            Console.WriteLine($"Površina kvadrata sa dijagonalom {d} je: {P}");
        }
        else
        {
            Console.WriteLine("Unos nije validan! Dijagonala mora biti pozitivan broj.");
        }

        Console.WriteLine("Pritisnite bilo koji taster za izlaz.");
        Console.ReadKey();
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
| _ _ _ _ _  | _ _ _ _ _ _ _ _ _ | _ _ _ _ _ _ _  |
| 1.         | 'd'               | 'double'       |
| 2.         | 'P'               | 'double'       |
