# rectangle.calculator
to calculate area, circumference, and diagonal

//p l lu k d

#include <iostream>
#include <iomanip>
#include <cmath>
using namespace std;

int main() {
    long double p, l, lu, k, d;
    int choice;

    // memasukan panjang persegi
    cout << "masukan panjang persegi: ";
    // membaca suhu masukan
    cin >> p;
    
    // memasukan lebar persegi
    cout << "masukan lebar persegi: ";
    // membaca suhu masukan
    cin >> l;
    
    lu = p*l;
    k = (p*2)+(l*2);
    d = sqrt(pow(p, 2) + pow(l, 2));
    
    cout << "ingin menghitung apa" << "\n" << 
            "1. luas persegi" << "\n" <<
            "2. keliling persegi"<< "\n"<<
            "3. panjang diagonal persegi" << "\n"
            "4. keluar" << "\n";
    std::cin >> choice;

//pilihan/menu
        switch (choice) {
            case 1:
                std::cout << lu;
                break;
            case 2:
                std::cout << k;
                break;
            case 3:
                std::cout << d;
                break;
            case 4:
                std::cout << "program selesai";
                break;
            default:
                std::cout << "Invalid choice. Please enter a number between 1 and 3.\n";
                break;
        }

    return 0;
}
