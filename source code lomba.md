
#include <windows.h>
#include <iostream>
#include <iomanip>
#include <string>
using namespace std;

/*
Program Konversi Suhu
Oleh :
Ahsin Aqsath
Oktavianus S.M.
SMA Negeri 1 Sampit
*/

void cf (double y) {
    double i=9;
    double j=5;
    double hasil=(y*(i/j))+32;
    int cek = hasil;
    if (hasil==cek){
        cout<<cek;
    } else {
    cout<<hasil;
    }
}

void ck (double y) {
    cout <<y+273.15;
}

void cre(double y) {
    double i=4;
    double j=5;
    double hasil=y*(i/j);
    int cek = hasil;
    if (hasil==cek){
        cout<<cek;
    } else {
    cout<<hasil;
    }
}

void cra (double y) {
    double i=9;
    double j=5;
    double hasil=y*(i/j)+491.67;
    int cek = hasil;
    if (hasil==cek){
        cout<<cek;
    } else {
    cout<<hasil;
    }

}

void fc (double y) {
    double i=9;
    double j=5;
    double hasil=(y-32)*(j/i);
    int cek = hasil;
    if (hasil==cek){
        cout<<cek;
    } else {
    cout<<hasil;
    }

}

void fk (double y) {
    double i=9;
    double j=5;
    double hasil=(y-32)*(j/i)+273.15;
    int cek = hasil;
    if (hasil==cek){
        cout<<cek;
    } else {
    cout<<hasil;
    }
}

void fra (double y) {
    double hasil=y+459.67;
    int cek = hasil;
    if (hasil==cek){
        cout<<cek;
    } else {
    cout<<hasil;
    }
}

void fre (double y) {
    double i=9;
    double j=4;
    double hasil=(y-32)*(j/i);
    int cek = hasil;
    if (hasil==cek){
        cout<<cek;
    } else {
    cout<<hasil;
    }
}

void kf (double y) {
    double i=5;
    double j=9;
    double hasil=(y-273.15)*(j/i)+32;
    int cek = hasil;
    if (hasil==cek){
        cout<<cek;
    } else {
    cout<<hasil;
    }
}
void kc (double y) {

    double hasil=y-273.15;
    int cek = hasil;
    if (hasil==cek){
        cout<<cek;
    } else {
    cout<<hasil;
    }
}

void kra (double y) {

    double hasil=y*1.8;
    int cek = hasil;
    if (hasil==cek){
        cout<<cek;
    } else {
    cout<<hasil;
    }
}

void kre (double y) {
    double i=5;
    double j=4;
    double hasil=(y-273.15)*(j/i);
    int cek = hasil;
    if (hasil==cek){
        cout<<cek;
    } else {
    cout<<hasil;
    }
}

void rare (double y) {
    double j=4;
    double hasil=(y-491.67)*(j/9);
    int cek = hasil;
    if (hasil==cek){
        cout<<cek;
    } else {
    cout<<hasil;
    }
}

void raf (double y) {

    double hasil=y-459.67;
    int cek = hasil;
    if (hasil==cek){
        cout<<cek;
    } else {
    cout<<hasil;
    }
}

void rac (double y) {
    double i=9;
    double j=5;
    double hasil=(y-491.67)*(j/i);
    int cek = hasil;
    if (hasil==cek){
        cout<<cek;
    } else {
    cout<<hasil;
    }
}

void rak (double y) {
    double i=9;
    double j=5;
    double hasil=y*(j/i);
    int cek = hasil;
    if (hasil==cek){
        cout<<cek;
    } else {
    cout<<hasil;
    }
}

void rec(double y) {
    double i=4;
    double j=5;
    double hasil=y*(j/i);
    int cek = hasil;
    if (hasil==cek){
        cout<<cek;
    } else {
    cout<<hasil;
    }
}

void ref (double y) {
    double i=9;
    double j=4;
    double hasil=y*(i/j)+32;
    int cek = hasil;
    if (hasil==cek){
        cout<<cek;
    } else {
    cout<<hasil;
    }
}

void rek(double y) {
    double i=4;
    double j=5;
    double hasil=y*(j/i)+273.15;
    int cek = hasil;
    if (hasil==cek){
        cout<<cek;
    } else {
    cout<<hasil;
    }
}

void rera(double y) {
    double i=9;
    double j=4;
    double hasil=y*(i/j)+491.67;
    int cek = hasil;
    if (hasil==cek){
        cout<<cek;
    } else {
    cout<<hasil;
    }
}
//referensi --> stackoverflow
VOID WINAPI SetConsoleColors(WORD attribs);

int main(){
       SetConsoleColors(BACKGROUND_BLUE | FOREGROUND_RED | FOREGROUND_INTENSITY);
    double x;
    string in,out;

    cout<<"TEMPERATURE CONVERTER\n\n\n";
    cout<<"Petunjuk Input\n\nInput dimasukan sesuai dengan format yang diminta, misal (suhu (spasi) satuan)\n\nSatuan yang digunakan antara lain : \nCelcius : C\nFahrenheit : F\nReamur : Re\nRankine : R\nKelvin : K\n\nContoh Input : 273 K\n";
    cout<<"\n(Tekan Enter Untuk Lanjut)";
cin.get();
    bool lanjut=true;



    while (true) {
            system("cls");
        cout<<"MENU TEMPERATUR CONVERTER\n\n\n1. Konversi ke satu satuan\n2. Konversi ke semua satuan\n3. Berhenti\nAyo dipilih ^v^ : ";
        cin>>in;

    if (in=="1") {
    while (true){
        system("cls");
        //input ouput konversi
        while (lanjut) {
        cout <<"Suhu Awal (suhu (spasi) satuan) : ";
        cin>>x>>in;

        cout <<"Konversi Ke : ";
        cin>>out;
        if (in==out){
            cout<<"\nKAMU GABUT YA??? KAMU MAU KONVERSI "<<in<<" KE "<<out<<"?? ITU KAN SAMA NGAPAIN DI KONVERSI? :(\n";
            break;
        }



        cout <<x<<" "<<in<<" = ";

        if (in=="C" && out=="F") {
            cf(x);
        } else if (in=="C" && out=="K") {
            ck(x);
        } else if (in=="C" && out=="Re") {
            cre(x);
        }else if (in=="C" && out=="R") {
            cra(x);
        } else if (in=="F" && out=="C") {
            fc(x);
        } else if (in=="F" && out=="Re") {
            fre(x);
        } else if (in=="F" && out=="R") {
            fra(x);
        }else if (in=="F" && out=="K") {
            fk(x);
        } else if (in=="K" && out=="C") {
            kc(x);
        } else if (in=="K" && out=="F") {
            kf(x);
        } else if (in=="K" && out=="Re") {
            kre(x);
        } else if (in=="K" && out=="Ra") {
            kra(x);
        }else if (in=="R" && out=="C") {
            rac(x);
        } else if (in=="R" && out=="F") {
            raf(x);
        } else if (in=="R" && out=="K") {
            rak(x);
        } else if (in=="R" && out=="Re") {
            rare(x);
        } else if (in=="Re" && out=="C") {
            rec(x);
        } else if (in=="Re" && out=="F") {
            ref(x);
        } else if (in=="Re" && out== "K") {
            rek(x);
        } else if (in=="Re" && out=="R") {
            rera(x);
        } else {
            system("cls");
        cout<<"INPUT KAMU ADA YANG SALAH YA??? BENERIN LAGI YA!!\n\n\n";
    Sleep(1400);
            break;
        }

        cout<<" "<<out;

     break;


    }
    //s

    //Lanjut/Ga
    cout<<endl<<endl<<"Konversi lagi?(Y/N) : ";
        char input;
        cin>>input;
        if(input=='Y'){
            lanjut=true;
            continue;
        } else if (input=='N'){
            break;
        } else {
            cout << "Input Salah!! Masukan input 'Y' untuk konversi lagi atau 'N' untuk berhenti!!";
            lanjut=false;
        }
        //s

    }

    }
    else if (in=="2"){

        while(true) {
            system("cls");
            cout<<"Halo!!Mau konversi dari mana?\n1. Celcius\n2. Fahrenheit\n3. Kelvin\n4. Rankine\n5. Reamur\nAyo dipilih ^v^ (Angka saja) : ";
            cin>>in;

while (lanjut) {
            if(in=="1") {
                system("cls");
            cout << "Suhu awal (Angka saja) : ";
            cin>>x;
            system("cls");
            cout <<x<<" Celcius Setara dengan : ";
            cf(x);
            cout<<" F, ";
            ck(x);
            cout<<" K, ";
            cra(x);
            cout<<" R, dan ";
            cre(x);
            cout<< " Re"<<endl<<endl<<endl;
            break;
            } else if(in=="2") {
                system("cls");
            cout << "Suhu awal (Angka saja) : ";
            cin>>x;
            system("cls");
            cout <<x<<" Fahrenheit Setara dengan : ";
            fc(x);
            cout<<" C, ";
            fk(x);
            cout<<" K, ";
            fra(x);
            cout<<" R, dan ";
            fre(x);
            cout<< " Re"<<endl<<endl<<endl;
            break;
            } else if(in=="3") {
                system("cls");
            cout << "Suhu awal (Angka saja) : ";
            cin>>x;
            system("cls");
            cout <<x<<" Kelvin Setara dengan : ";
            kc(x);
            cout<<" C, ";
            kf(x);
            cout<<" F, ";
            kra(x);
            cout<<" R, dan ";
            kre(x);
            cout<< " Re"<<endl<<endl<<endl;
            break;
            } else if(in=="4") {
                system("cls");
            cout << "Suhu awal (Angka saja) : ";
            cin>>x;
            system("cls");
            cout <<x<<" Rankine Setara dengan : ";
            rac(x);
            cout<<" C, ";
            raf(x);
            cout<<" F, ";
            rak(x);
            cout<<" K, dan ";
            rare(x);
            cout<< " Re"<<endl<<endl<<endl;
            break;
            }else if(in=="5") {
                system("cls");
            cout << "Suhu awal (Angka saja) : ";
            cin>>x;
            system("cls");
            cout <<x<<" Reamur Setara dengan : ";
            rec(x);
            cout<<" C, ";
            ref(x);
            cout<<" F, ";
            rek(x);
            cout<<" K, dan ";
            rera(x);
            cout<< " R"<<endl<<endl<<endl;
            break;
            }
            else {
            system("cls");
        cout<<"MAAF KAMI CUMAN PUNYA PILIHAN 1 HINGGA 5 :( SILAHKAN PILIH ULANG\n";


    Sleep(1400);
   break;
    }

}


        cout<<endl<<endl<<"Konversi lagi?(Y/N) : ";
        char input;
        cin>>input;
        if(input=='Y'){
            lanjut=true;
            continue;
        } else if (input=='N'){
            break;
        } else {
            cout << "Input Salah!! Masukan input 'Y' untuk konversi lagi atau 'N' untuk berhenti!!";
            lanjut=false;
        }

    }
    }
    else if (in=="3" ){
        break;
    }

    else {
            system("cls");
        cout<<"MAAF KAMI CUMAN PUNYA PILIHAN 1 DAN 2 :( SILAHKAN PILIH ULANG\n";


    Sleep(1400);
    }

    }
    system("cls");
    cout<<"Terimakasih ya udah pakek program kami :)\n\nTertanda : \nAhsin Aqsath\nOktavianus Samuel\nSMAN 1 Sampit\n\n";
     Sleep(3000);
    system("cls");

    cout<<"Disclaimer!!!\n\nProgram ini ditulis secara manual(dari nol) dengan berbagai referensi tanpa niat menjiplak,meniru, maupun memanfaatkan program orang lain\n\nTerimakasih:)";

}


VOID WINAPI SetConsoleColors(WORD attribs) {
    HANDLE hOutput = GetStdHandle(STD_OUTPUT_HANDLE);

    CONSOLE_SCREEN_BUFFER_INFOEX cbi;
    cbi.cbSize = sizeof(CONSOLE_SCREEN_BUFFER_INFOEX);
    GetConsoleScreenBufferInfoEx(hOutput, &cbi);
    cbi.wAttributes = attribs;
    SetConsoleScreenBufferInfoEx(hOutput, &cbi);
}




