# Ujian Akhir Semester 
<br>Mata Kuliah		: Dasar Pemrograman
<br> Nama		: ILham Marwan Sidik
<br>NIM			: 1227050055
<br>Jurusan		: [Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum


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
