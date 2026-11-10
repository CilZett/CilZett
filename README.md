<p align="center">
  <img src="https://raw.githubusercontent.com/CilZett/CilZett/refs/heads/main/assets/profile.svg" alt="animated ascii profile card" width="100%" />
</p>

<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?font=Fira+Code&weight=600&size=22&duration=3500&pause=1000&color=00FF66&center=true&vCenter=true&width=500&height=50&lines=root%40peter-terminal%3A~%23+whoami;System+Compromised...;Informatics+Engineering+Student;Welcome+to+my+domain" alt="Typing SVG" />
</p>

<p align="center">
  <pre align="center" style="background: transparent; border: none; padding: 0;">
██████╗ ███████╗████████╗███████╗██████╗ 
██╔══██╗██╔════╝╚══██╔══╝██╔════╝██╔══██╗
██████╔╝█████╗     ██║   █████╗  ██████╔╝
██╔═══╝ ██╔══╝     ██║   ██╔══╝  ██╔══██╗
██║     ███████╗   ██║   ███████╗██║  ██║
╚═╝     ╚══════╝   ╚═╝   ╚══════╝╚═╝  ╚═╝
  </pre>
<p align="center">
  <span style="color: #FFD700; font-size: 24px;">★★★★★★</span><br><br>
  <img src="https://img.shields.io/badge/RANK--GOD-000000?style=for-the-badge&logoColor=FFD700&color=000000" alt="RANK GOD">
</p>

<picture data-importer="pacman">
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/CilZett/CilZett/pacman-output/pacman-contribution-graph-dark.svg?game=pacman">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/CilZett/CilZett/pacman-output/pacman-contribution-graph.svg?game=pacman">
  <img alt="pacman contribution graph" src="https://raw.githubusercontent.com/CilZett/CilZett/pacman-output/pacman-contribution-graph.svg?game=pacman">
</picture>

###

#include <iostream>
#include <thread>   // Diperlukan untuk fungsi jeda (sleep)
#include <chrono>   // Diperlukan untuk satuan waktu (milliseconds/seconds)

using namespace std;

// Fungsi untuk animasi loading titik-titik (.)
void animasiLoading() {
    cout << "Sedang meracik kopi pesananmu";
    
    // Perulangan untuk memunculkan titik sebanyak 4 kali
    for (int i = 0; i < 4; i++) {
        cout << "." << flush; // flush memaksa teks langsung muncul di layar tanpa menunggu buffer penuh
        
        // Jeda waktu selama 500 milidetik (0.5 detik)
        this_thread::sleep_for(chrono::milliseconds(500));
    }
    cout << "\nKopi siap disajikan!\n";
}

// Fungsi untuk efek teks seperti mesin ketik (typewriter)
void efekKetik(string teks, int kecepatanMS) {
    for (char c : teks) {
        cout << c << flush;
        this_thread::sleep_for(chrono::milliseconds(kecepatanMS));
    }
    cout << endl;
}

int main() {
    cout << "=== DEMO ANIMASI TEKS C++ ===\n\n";
    
    // Menjalankan efek ketik
    efekKetik("Halo! Selamat datang di Coffee Shop kami.", 40); // kecepatan 40ms per huruf
    
    cout << endl;
    
    // Menjalankan animasi loading
    animasiLoading();

    return 0;
}
