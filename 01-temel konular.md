**Casting**   ifadesi ne anlama gelir ?

Dönüştürme işlemidir



````c#
long deger1=100;
İnt deger2=(int)deger1;
````



**Is** *ve* **As**  operatörleri ne işe yarar ?

**as** referans tiplerde veriyi dönüştürürse veriyi dönüştüremesse null değerini verir;
**is**  dönüştürme işlemi yapılabilirse true, yapılamazsa false değeri döndürür.



```c#
object obj=null;
string result= obj as string;
Console.WriteLine(result);
```



```c#
object[] values={"hasan",5,5.5,true,false,"veli"};

foreach(var item in values){
       
       if(item is string)
       {
       		string value=item as string;
             Console.WriteLine("string-> " +value);
       }
       
}
```



**Switch Case Referans ve veri Tipi Karşılaştırması**



```c#
object[] values={"hasan",5,5.5,true,false,"veli"};
       
foreach(var item in values)
       {
       switch(item )
       {
       case string aa:
       Console.WriteLine("string-> " +aa);
       break;
       case bool aa:
       Console.WriteLine("bool-> " +aa);
       break;
       case int aa:
       Console.WriteLine("int-> " +aa);
       break;
       case double aa:
       Console.WriteLine("double-> " +aa);
       break;
             case decimal aa:
       Console.WriteLine("double-> " +aa);
       break;
       }
       
       
       }
       
}
```



