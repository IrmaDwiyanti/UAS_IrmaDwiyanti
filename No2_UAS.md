# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		: Irma Dwiyanti
<br>NIM		:	127050059
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
2. Program dibuat dengan menggunakan array , statement seleksi if  dan rumus operator matematika 

## Source Code
#include <iostream>
#include <iomanip>
using namespace std;
int main(){
    
	int arr[100][100], jumlahBaris, jumlahKolom, i, j, baris, kolom;

	cout << "==================================="<<endl;
	cout << "Nama : Irma Dwiyanti"<<endl;
	cout << "NIM  : 1227050059"<<endl;
	cout << "==================================="<<endl<<endl<<endl;
	
	cout << "2. Program menampilkan bilangan yang habis dibagi 3, 5 dan 7" << endl;
	cout << "---------------------------------------------------------------------"<<endl;
    cout<<"Input jumlah baris: "; cin>>jumlahBaris;
    cout<<"Input jumlah kolom: "; cin>>jumlahKolom;
    cout << endl;

    for(i = 0; i < jumlahBaris; i++){
        for(j = 0; j < jumlahKolom; j++){
            cout << "Baris " <<i+1<<", kolom "<<j+1<< " = ";
            cin >> arr[i][j];
        }
        cout << endl;
    }

    cout << "Hasil input nilai : " << endl;

    for(i = 0; i < jumlahBaris ; i++){
    for(j = 0; j < jumlahKolom; j++){
        cout << setw(3) << arr[i][j] << " ";
    }
    cout << endl;
    }

    cout << "\nHasil bilangan yang tidak bisa dibagi 3,5,7 : " << endl;

    for(i = 0; i < jumlahBaris ; i++){
    for(j = 0; j < jumlahKolom; j++){
        if(arr[i][j] % 3 == 0 || arr[i][j] % 5 == 0 || arr[i][j] % 7 == 0){
        cout << setw(3) << arr[i][j] << " ";
        }
    }
    cout << endl;
    }

    
    cout << endl;
    return 0;
}

## Output

![Screenshot (68)](https://user-images.githubusercontent.com/120999558/208387283-e87d7895-6f38-408e-b829-8902ce231731.png)
