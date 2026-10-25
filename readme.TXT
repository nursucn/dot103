int[] a = new int[10];
for (int i = 0; i < a.Length; i++)
{
    a[i] = new Random().Next(1, 100);
    Console.WriteLine("Sayılar:"+a[i].ToString());
}
    int enb = a[0];
    int enk = a[0];
    foreach (int sayi in a)
    {
        if (sayi > enb)
        {
            enb = sayi;
        }
        if (sayi < enk)
        {
            enk = sayi;
        }
    }      

    
Console.WriteLine("En büyük sayı:"+enb.ToString());
Console.WriteLine("En küçük sayı:"+enk.ToString());
Console.WriteLine("Çift sayılar:");
    foreach (int sayi in a)
{
    if (sayi % 2 == 0)
    {
        Console.WriteLine(sayi.ToString());
    }
}
    Console.WriteLine("Tek sayılar:");
foreach (int sayi in a)
{
    if (sayi % 2 == 1)
    {
        Console.WriteLine(sayi.ToString());
    }
}

/*Sıraları gösterme ve kullanıcıdan sayı isteyip ondan büyük sayıları gösterme kısmını yapamadım*/