# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		: Irma Dwiyanti
<br>NIM		:	1227050059
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## 1. Transpose matriks adalah matriks baru yang diperoleh dengan cara menukar elemen-elemen baris menjadi elemen kolom atau sebaliknya. Sementara pengertian matriks itu sendiri adalah susunan bilangan yang terdiri atas baris dan kolom dan ditulis dalam kurung ().

```
## Source Code
#include <iostream>
using namespace std;

int main() {
   int a[10][10], transpose[10][10], row, column, i, j;

   
   cout<<"Input jumlah baris: "; cin>>row;
    cout<<"Input jumlah kolom: "; cin>>column;
    cout << endl;
   

   cout << "\nMasukkan angka: " << endl;

   
   for (int i = 0; i < row; ++i) {
      for (int j = 0; j < column; ++j) {
         cout << "Masukkan element " << i + 1 <<","<< j + 1 << ": ";
         cin >> a[i][j];
      }
   }

   
   cout << "\nHasil Transpose: " << endl;
   for (int i = 0; i < row; ++i) {
      for (int j = 0; j < column; ++j) {
         cout << " " << a[i][j];
         if (j == column - 1)
            cout << endl << endl;
      }
   }

  
   for (int i = 0; i < row; ++i)
      for (int j = 0; j < column; ++j) {
         transpose[j][i] = a[i][j];
      }

   
   cout << "\nAwal Tranpose: " << endl;
   for (int i = 0; i < column; ++i)
      for (int j = 0; j < row; ++j) {
         cout << " " << transpose[i][j];
         if (j == row - 1)
            cout << endl << endl;
      }

   return 0;
}
```

## Output![Screenshot (67)](https://user-images.githubusercontent.com/120999558/208386329-d7e8251d-c9df-480a-9793-545cb62d59f1.png)


