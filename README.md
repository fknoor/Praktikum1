# Praktikum1

Break

#include <iostream>
using namespace std;

struct player_a {
  int id;
  string nama;
  string asalDaerah;
  string kelakuan;
};

int main() 
{
  player_a player[] = {
    {
      1,
      "usep",
      "Bandung",
      "Jahat",
    },
    {
      2,
      "agus",
      "Garut",
      "nakal",
    },
    {
      3,
      "jeje",
      "Bekasi",
      "baik",
    },
    {
      4,
      "susi",
      "Aceh",
      "cengeng",
    },
    {
      5,
      "marsal",
      "Tasik",
      "pemarah",
    }
  };

  int idPlayerYangDiBeriUang = 3;

  player[1].nama = "agus";

  for (int i = 0; i < 5; i++) {

    if (player[i].id == idPlayerYangDiBeriUang) {
      cout << "Ini anak baik " << player[i].nama << "  Beri dia Uang ! \n";

      break;
    }

    cout << "Itu si " << player[i].nama << " adalah anak " << player[i].kelakuan << "\n";
  }

}
