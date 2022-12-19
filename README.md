# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		: Muhammad Fakhruddin Al Farrosy
<br>NIM		:	1227050088
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
  Untuk menghitung matriks pada C++ dengan bilangan yang dapat habis dibagi 3, 5, atau 7, kita dapat menggunakan perulangan for untuk mengakses setiap elemen dari matriks satu per satu dan mengecek apakah elemen tersebut habis dibagi oleh 3, 5, atau 7

## Source Code
#include <iostream>
using namespace std;

int main(){
  int x, y; 
  int baris, kolom; 
  int matriks[100][100], matrikst[100][100];
  
  cout << "Bilangan matriks yang bisa dibagi 3,5,7 \n";
  cout << "================================================\n";
  
  cout<<endl;
  cout << "================================================\n";
  cout<<endl;
  
  cout << "Masukkan baris matriks: ";
  cin >> baris;
  
  cout<<endl;
  cout << "================================================\n";
  cout<<endl;
  
  cout << "Masukkan kolom matriks: ";
  cin >> kolom;
  cout<<endl;

  cout << "\nMasukkan elemen matriks : \n";
  for (x = 1; x <= baris; x++){
    for (y = 1; y <= kolom; y++){
      cout << "Baris ke-" << x << ", kolom ke-" << y << " : ";
      cin  >> matriks[x][y];
    }
  }
  
  cout << "\nMatriks yang bilangannya habis 3,5,7 adalah : \n";
  for (x = 1; x <= baris; x++){
  	for (y = 1; y <= kolom; y++){
  		if (matriks [x][y] % 3 == 0 or matriks [x][y] % 5 == 0 or matriks [x][y] % 7 == 0){
  			matriks [x][y] = matriks [x][y];
		  }
		else {
			matriks [x][y] = 0;
			
		}
	  }
  }
  for (x = 1; x <= baris; x++){
    for (y = 1; y <= kolom; y++){
      cout << matriks [x][y] << "\t";
    }
    cout << endl;
  }  
}
  
## Output
  ![image](https://user-images.githubusercontent.com/105347617/208530441-ef2734ed-f94b-4a11-9ec5-062ce17915d8.png)
Pada program di atas, kita menginputkan nilai ke dalam matriks, dan menggunakan perulangan for untuk mengakses setiap elemen dari matriks satu per satu. Kemudian, kita mengecek apakah elemen tersebut habis dibagi oleh 3, 5, atau 7 dengan menggunakan operator modulus (%). Jika elemen tersebut habis dibagi oleh salah satu dari bilangan tersebut, maka elemen tersebut akan dicetak ke layar.
