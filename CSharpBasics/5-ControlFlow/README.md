# Control Flow | Conditionals - If, Else, Switch og Ternary

I C# er conditionals en vigtig del af programmering, der giver dig mulighed for at udføre forskellige handlinger baseret på en bestemt betingelse. Du kan bruge forskellige typer conditionals i C#, herunder if, else, switch og ternary operator. Vi reffere også til det som kontrol flow, for vi kontrollere flowet af vores kode ud fra nogle betingelser (conditionals)

### If Statement

If statement (hvis-udtalelse) er den mest grundlæggende form for conditional i C#. Det giver dig mulighed for at udføre en bestemt kodeblok, hvis en betingelse er sand. Hvis betingelsen er falsk, springes kodeblokken over.

Her er syntaksen for en if statement:

```csharp
if (betingelse)
{
    // Kode, der skal udføres, hvis betingelsen er sand
}

```

For eksempel kan du bruge en if statement til at kontrollere, om et tal er større end 10:

```csharp
int num = 15;

if (num > 10)
{
    Console.WriteLine("Tallet er større end 10.");
}

```

I dette eksempel vil konsollen udskrive "Tallet er større end 10", fordi betingelsen `num > 10` er sand.

### Else Statement

Else statement (ellers-udtalelse) bruges sammen med if statement til at definere en alternativ kodeblok, der skal udføres, hvis betingelsen i if statement er falsk.

Her er syntaksen for en else statement:

```csharp
if (betingelse)
{
    // Kode, der skal udføres, hvis betingelsen er sand
}
else
{
    // Kode, der skal udføres, hvis betingelsen er falsk
}

```

For eksempel kan du bruge en else statement til at kontrollere, om et tal er større end 10 eller ej:

```csharp
int num = 5;

if (num > 10)
{
    Console.WriteLine("Tallet er større end 10.");
}
else
{
    Console.WriteLine("Tallet er ikke større end 10.");
}

```

I dette eksempel vil konsollen udskrive "Tallet er ikke større end 10", fordi betingelsen `num > 10` er falsk.

### Else If Statement

Else if statement (ellers hvis-udtalelse) bruges til at teste flere betingelser i træk, hvis den foregående betingelse er falsk. Det giver dig mulighed for at definere alternativer til en if statement uden at oprette flere nestede if statements.

Her er syntaksen for et else if statement:

```csharp
if (betingelse1)
{
    // Kode, der skal udføres, hvis betingelse1 er sand
}
else if (betingelse2)
{
    // Kode, der skal udføres, hvis betingelse2 er sand
}
else if (betingelse3)
{
    // Kode, der skal udføres, hvis betingelse3 er sand
}
else
{
    // Kode, der skal udføres, hvis ingen af betingelserne er sande
}

```

For eksempel kan du bruge et else if statement til at kontrollere, om et tal er positivt, negativt eller nul:

```csharp
int num = -5;

if (num > 0)
{
    Console.WriteLine("Tallet er positivt.");
}
else if (num < 0)
{
    Console.WriteLine("Tallet er negativt.");
}
else
{
    Console.WriteLine("Tallet er nul.");
}

```

I dette eksempel vil konsollen udskrive "Tallet er negativt", fordi betingelsen `num < 0` er sand.

### Switch Statement

Switch statement (switch-udtalelse) giver dig mulighed for at vælge mellem forskellige handlinger baseret på værdien af en variabel eller et udtryk. Det er nyttigt, når du har flere mulige tilfælde at håndtere.

Her er syntaksen for en switch statement:

```csharp
switch (variabel/udtryk)
{
    case værdi1:
        // Kode, der skal udføres, når variabel/udtryk er lig med værdi1
        break;
    case værdi2:
        // Kode, der skal udføres, når variabel/udtryk er lig med værdi2
        break;
    default:
        // Kode, der skal udføres, når ingen af de ovenstående tilfælde matcher
        break;
}

```

For eksempel kan du bruge en switch statement til at håndtere forskellige handlinger baseret på en variabels værdi:

```csharp
int day = 3;
string dayName;

switch (day)
{
    case 1:
        dayName = "Mandag";
        break;
    case 2:
        dayName = "Tirsdag";
        break;
    case
}
```

### Ternary Operator

Ternary operator (ternær operator) er en kompakt syntaks til at udføre en betinget handling baseret på en betingelse. Det er en forkortet måde at skrive en if-else statement på.

Her er syntaksen for en ternary operator:

```csharp
resultat = (betingelse) ? værdiHvisSand : værdiHvisFalsk;

```

For eksempel kan du bruge en ternary operator til at kontrollere, om et tal er positivt eller negativt:

```csharp
int num = -5;
string result = (num >= 0) ? "Positivt" : "Negativt";

Console.WriteLine(result);

```

I dette eksempel vil konsollen udskrive "Negativt", fordi betingelsen `num >= 0` er falsk.

Ternary operator kan være nyttig, når du har en enkel betingelse og ønsker at skrive koden mere kompakt. Det kan gøre koden mere læselig og reducere antallet af linjer. Men vær forsigtig med at overbruge ternary operator, da det kan gøre koden mere kompleks og sværere at forstå, hvis betingelsen bliver for kompleks.

Ternary operator kan være fortrukket i visse situationer, især når betingelsen og værdierne er korte og enkle. Det kan forbedre kodens læsbarhed og gøre den mere elegant. Men hvis betingelsen og værdierne er komplekse, kan det være bedre at bruge en if-else statement for at gøre koden mere forståelig og vedligeholdelig.

Husk altid at vælge den mest passende syntaks og struktur for din kode baseret på dens kompleksitet og læsbarhed.
