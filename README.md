
```try{
    Console.WriteLine("Bir sayı giriniz:");
    int sayi = Convert.ToInt32(Console.ReadLine());
    Console.WriteLine("Girmiş olduğunuz sayı :" + sayi);

}
catch(Exception ex) {

    Console.WriteLine("Hata: " + ex.Message.ToString());

}

//finally {
//    Console.Write("İşlem tamamlandı.");
//}
```
```
try{
   //int a = int.Parse(null);
   //int a = int.Parse("test");
   int a = int.Parse("-20000000000");
}
catch(ArgumentNullException ex) {

    Console.WriteLine("Boş değer girdiniz");
    Console.WriteLine(ex);
}
catch(FormatException ex) {

    Console.WriteLine("Veri tipi uygun değil.");
    Console.WriteLine(ex);
}

catch(OverflowException ex) {
    Console.WriteLine("Girilen değer çok küçük ya da çok büyük.");
    Console.WriteLine(ex);

}

finally {
    Console.WriteLine("İşlem başarıyla tamamlandı");
}
```