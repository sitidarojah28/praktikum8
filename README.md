# praktikum8

*latihan1* mmembuat fibonanci dengan ara fungsi iteratif
- Alur Algoritmanya
	-mendefinisikan fungsi fibonanci
	int fibonanci (int suku, int a, int b, int c)
-mengisi int a =0 dan int b=1
-membuat rumus if untuk perbandingan dan rumus fibonanci
```c++
 if (suku== 1) //jika nilai suku 1,nilai=1
        return b;
    if (suku==0)//jika nilai suku 0,nilai=0
        return a;
    else
        {
        for ( int i=2; i<=suku; i++){
            c=a+b; //suku ke-3 = suku kw-1 + suku ke-2
            a=b;//nilai suku a diisi dengan n
            b=c;//nilai suku b disi dengan nilai suku c
        }
        return c;

-Berikut kode lengkapnya

#include <iostream>

using namespace std;
int fibonanci (int suku, int a, int b, int c)
{
    a=0; //int nilai a 0
    b=1;// int nilai b 1
    if (suku== 1) //jika nilai suku 1,nilai=1
        return b;
    if (suku==0)//jika nilai suku 0,nilai=0
        return a;
    else
        {
        for ( int i=2; i<=suku; i++){
            c=a+b; //suku ke-3 = suku kw-1 + suku ke-2
            a=b;//nilai suku a diisi dengan n
            b=c;//nilai suku b disi dengan nilai suku c
        }
        return c;
        }
}
int main()
{
    int suku,a,b,c;

    cout << "Masukan nilai suku Ke-: " ;
    cin>> suku;
    cout<<"\n Bilangan Fibonanci untuk "<< suku << " Adalah ";
    cout<< fibonanci(suku,a,b,c);
    return 0;

- berikut flowchatnya

![img](https://github.com/sitidarojah28/praktikum8/blob/master/latihan1/flowchat1.png)

- berikut hasilnya

![img](https://github.com/sitidarojah28/praktikum8/blob/master/latihan1/hasil1.png)

#Latihan2#Perkalian dengan penjumlahan menggunakan fungsi rekursif

1.Alur Algoritmanya
	-Mendefinisikan fungsi kali
int kali (int a, int b)
	-membuat rumus if dan perkalianya
if (b==0) //jika nilai b=0 maka hasilnya 0
        return 0;
    else
        return a+kali(a,b-1); // nilai a ditambah (nilai a ditambah nilai b dikurangi 1)
2.Berikut kode lengkapnya

#include <iostream>

using namespace std;
int kali (int a, int b)
{
    if (b==0)
        return 0;
    else
        return a+kali(a,b-1);
        cout<< a;
}
int main()
{
    int a,b;
    cout << "Masukan bilangan pertama :";
    cin>> a;
    cout << "Masukan bilangan kedua :";
    cin>> b;
    cout<< " Hasil = " <<kali (a,b);
    return 0;
}

- berikut flowchatnya

![img](https://github.com/sitidarojah28/praktikum8/blob/master/latihan2/flowchat2.png)

-berikut hasilnya 

![img](https://github.com/sitidarojah28/praktikum8/blob/master/latihan2/hasil2.png)

#Latihan3#Pembagian dengan menggunakan fungsi rekursif

1.Alur Algoritmanya
	-Mendefinisikan fungsi bagi
int bagi(int a, int b)
	-membuat rumus if dan pembagianya
if (a<b) 
        return 0;
    else
        return 1+bagi(a-b,b); 
2.Berikut kode lengkapnya

#include <iostream>

using namespace std;
int bagi(int a, int b)
{
    if (a<b)
        return 0;
    else
        return 1+bagi(a-b,b);
     
}
int main()
{
    int a,b;
    cout << "Masukan bilangan pertama :";
    cin>> a;
    cout << "Masukan bilangan kedua :";
    cin>> b;
    cout<< " Hasil = " <<bagi (a,b);
    return 0;
}

-berikut hasilnya 

![img](https://github.com/sitidarojah28/praktikum8/blob/master/latihan3/hasil3.png)

