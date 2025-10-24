# lisamine-teise-while-n-idise-koos-case-kasutasega

```csharp
Console.WriteLine("Tere tulemust mobifix parandusautomaati! Kuidas saan aidata");
Console.WriteLine("0 - headaega\n1 - tahan telefoni parandada");
Console.WriteLine("palun tee valik, kirjutades vastav arv:");
int valik = int.Parse(Console.ReadLine());
while (valik < 0 && valik > 1)
{
    Console.WriteLine("Palun tee oma valik, kirjatades vastav arv");
    valik = int.Parse(Console.ReadLine());
}
if (valik == 0)
{
    Console.WriteLine("Headaega, tulge teinekord jälle!");
}
else
{
    Console.WriteLine("palun sisesta oma telefoni mudel, mida parandada soovid:");
    Console.WriteLine("1-iFöön\n2-xiaomjäu\n3-nihuawei\n4-Scamsung");
    Console.WriteLine("palun tee valik, kirjutades vastav arv:");
    int telefonimudel = 0;
    telefonimudel = int.Parse(Console.ReadLine());
    while (telefonimudel < 1 && telefonimudel > 4)
    {
        telefonimudel = int.Parse(Console.ReadLine());
        Console.WriteLine("palun tee valik, kirjutades vastav arv:");
    }
    switch (telefonimudel)
    {
        case 1:
            Console.WriteLine("Aitah, oma iFööni saaad tagasi 1 nädala pärast");
            break;
        case 2:
            Console.WriteLine("Aitah, sinu xiomjäu on valmis tagasi 2 kuu pärast");
            break;
        case 3:
            Console.WriteLine("Kahjuks me nihuaweid ei teneninda");
            break;
        case 4:
            Console.WriteLine("SinuScamsung on valmis 2 päeva pärast");
            break;
        default:
            Console.WriteLine("Ei tunne sellist telefonitootjat");
            break;
    }
    
}
