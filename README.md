# Ujian Akhir Semester 
<br>Mata Kuliah		: Dasar Pemrograman
<br> Nama		: Ilham Marwan Sidik
<br>NIM			: 1227050055
<br>Jurusan		: [Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
Array dua dimensi adalah sebutan untuk array yang penomoran index-nya menggunakan 2 buah angka. Analogi lain adalah matriks. Matrixs Merupakan kumpulan-kumpulan bilangan yang disusun secara baris (vertikal) dan kolom (horizontal) bisa disebut juga array dua dimensi (multi-dimensional). Transpose Matriks adalah memperoleh sebuah matriks dengan cara menukar baris menjadi kolom dan kolom menjadi baris dari sebuah matriks. Dalam matematika, matriks terdiri dari kolom dan baris. Kembali, untuk menentukan nilai dari sebuah matriks, kita harus sebut secara berpasangan seperti baris 1 kolom 1, atau baris 2 kolom 3, dst. Konsep seperti inilah yang menjadi dasar dari array 2 dimensi. Untuk membuat array 2 dimensi di dalam bahasa C++, caranya tulis 2 kali tanda kurung siku setelah nama variabel, seperti contoh berikut:
int arr[2][2];

Pada UAS semester 1 ini saya diminta untuk membuat 2 buah program yaitu program pertama adalah membuat array 2 dimensi dengan baris , kolom dan nilai nya di input lalu ditukarkan antara kolom dan baris (transpose) lalu untuk program ke dua yaitu digunakan untuk mencari nilai yang dapat di bagi 3, 7, dan 5.

## Source Code
#include <iostream>
using namespace std;

int main()
{
    double a[10][10];
    int i, j, k, baris, colom;

    cout << " Masukan jumlah baris = ";
    cin >> baris;
    cout << " Masukan jumlah kolom = ";
    cin >> colom;
    cout << endl;

    cout << endl
         << " Elemen matriks : " << endl;
    for (i = 0; i < baris; i++)
    {
        for (j = 0; j < colom; j++)
        {
            cout << " Elemen matrik baris ke-" << i << " kolom ke-" << j << ": ";
            cin >> a[i][j];
        }
    }

    cout << endl;

    cout << " Element matriks adalah : " << endl;
    for (i = 0; i < baris; i++)
    {
        for (j = 0; j < colom; j++)
        {
            cout << "    " << a[i][j];
        }
        cout << endl;
    }
    cout << endl;
    cout << endl;
    cout << " Matriks Transpose :" << endl;
    for (i = 0; i < colom; i++)
    {
        // if ()
        for (j = 0; j < baris; j++)
        {
            cout << "    " << a[j][i];
        }
        cout << endl;
    }
	return 0;
}


## Output
![image](https://user-images.githubusercontent.com/121008252/208376431-8728dd9c-9c0b-470c-894c-4b737c12db5d.png)

## Source Code
#include <iostream>
#include <iomanip>
using namespace std;
int main(){
    
	int arr[100][100], jumlahBaris, jumlahKolom, i, j, baris, kolom;

    cout<<" Input jumlah baris: "; 
	cin>>jumlahBaris;
    cout<<" Input jumlah kolom: "; 
	cin>>jumlahKolom;
    cout << endl;

    for(i = 0; i < jumlahBaris; i++){
        for(j = 0; j < jumlahKolom; j++){
            cout << " Baris " <<i+1<<", Kolom "<<j+1<< " = ";
            cin >> arr[i][j];
        }
        cout << endl;
    }

    cout << " Hasil input nilai : " << endl;

    for(i = 0; i < jumlahBaris ; i++){
    for(j = 0; j < jumlahKolom; j++){
        cout << setw(3) << arr[i][j] << " ";
    }
    cout << endl;
    }

    cout << " Hasil bilangan yang habis dibagi 3,5,7 : " << endl;

    for(i = 0; i < jumlahBaris ; i++){
    for(j = 0; j < jumlahKolom; j++){
        if(arr[i][j] % 3 == 0 || arr[i][j] % 5 == 0 || arr[i][j] % 7 == 0){
        cout << setw(3) << arr[i][j] << " ";
        }
    }
    cout << endl;
    }
	cout << endl;
}

## Output
![image](https://user-images.githubusercontent.com/121008252/208377766-5be6b7da-d6c5-4a30-99bb-608306ca6ca8.png)
