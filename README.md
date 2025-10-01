# VocabEase - Duolingo-like Quiz Application

VocabEase adalah aplikasi quiz bahasa Inggris yang terinspirasi dari Duolingo, dibangun dengan HTML, CSS, dan JavaScript murni. Aplikasi ini menyediakan pengalaman belajar yang interaktif dengan berbagai jenis soal, sistem leveling, leaderboard, dan achievement.

## 🌟 Fitur Utama

### 📚 Sistem Quiz Interaktif
- **Multiple Choice Questions**: Soal pilihan ganda dengan 4 opsi jawaban
- **Audio Listening Test**: Soal mendengarkan seperti TOEFL dengan Speech Synthesis API
- **Timer System**: Batas waktu untuk setiap soal (30 detik untuk listening, 20 detik untuk multiple choice)
- **Real-time Feedback**: Feedback langsung dengan warna hijau/merah untuk jawaban benar/salah

### 🏆 Sistem Gamifikasi
- **XP System**: Dapatkan 10 XP untuk jawaban benar, 5 XP untuk jawaban salah
- **10 Level System**: Mulai dari Beginner hingga Master dengan visual progress path
- **Leaderboard**: Ranking berdasarkan total XP dengan avatar unik
- **Achievement System**: 6 kategori achievement dengan progress tracking:
  - First Steps (Quiz pertama)
  - Speed Demon (Jawab cepat)
  - Perfect Score (Skor sempurna)
  - Streak Master (Streak panjang)
  - Level Up (Naik level)
  - Quiz Master (Banyak quiz)

### 🎨 Desain Modern
- **Glassmorphism UI**: Efek kaca transparan yang modern
- **Gradient Backgrounds**: Background gradien yang menarik
- **Smooth Animations**: Animasi halus untuk transisi
- **Responsive Design**: Tampilan optimal di berbagai ukuran layar
- **Icon Integration**: Icon yang relevan untuk setiap elemen

## 🚀 Cara Menjalankan

### Metode 1: Server Lokal (Recommended)
```bash
# Navigasi ke folder project
cd vocabease

# Jalankan server HTTP sederhana
python -m http.server 8000

# Buka browser dan akses
http://localhost:8000/vocabease.html
```

### Metode 2: Buka Langsung
Buka file `vocabease.html` langsung di browser (beberapa fitur mungkin terbatas)

## 🎮 Cara Bermain

1. **Mulai Quiz**: Klik tombol "Start Quiz" di halaman utama
2. **Jawab Soal**: 
   - Untuk soal listening: Dengarkan audio dan ketik apa yang Anda dengar
   - Untuk multiple choice: Pilih jawaban yang benar
3. **Perhatikan Timer**: Setiap soal memiliki batas waktu
4. **Lihat Progress**: Progress bar menunjukkan kemajuan quiz
5. **Dapatkan XP**: Kumpulkan XP untuk naik level dan unlock achievement
6. **Cek Leaderboard**: Lihat ranking Anda dibandingkan pemain lain

## 📊 Sistem Penilaian

- **Jawaban Benar**: +10 XP
- **Jawaban Salah**: +5 XP (tetap dapat reward untuk usaha)
- **Bonus Speed**: XP tambahan untuk jawaban cepat
- **Perfect Score**: Bonus achievement untuk skor 100%

## 🏅 Level System

| Level | Nama | XP Required |
|-------|------|-------------|
| 1 | Beginner | 0 |
| 2 | Novice | 50 |
| 3 | Learner | 150 |
| 4 | Student | 300 |
| 5 | Scholar | 500 |
| 6 | Expert | 750 |
| 7 | Advanced | 1050 |
| 8 | Professional | 1400 |
| 9 | Specialist | 1800 |
| 10 | Master | 2250 |

## 💾 Penyimpanan Data

Aplikasi menggunakan **Local Storage** untuk menyimpan:
- Progress level dan XP
- Achievement yang sudah didapat
- Statistik quiz
- Data leaderboard

## 🛠️ Teknologi yang Digunakan

- **HTML5**: Struktur aplikasi
- **CSS3**: Styling dengan Flexbox, Grid, dan animasi
- **JavaScript ES6+**: Logika aplikasi dan interaktivitas
- **Web Speech API**: Text-to-Speech untuk soal listening
- **Local Storage API**: Penyimpanan data lokal

## 📱 Kompatibilitas

- ✅ Chrome 60+
- ✅ Firefox 55+
- ✅ Safari 11+
- ✅ Edge 79+
- ✅ Mobile browsers (responsive design)

## 🔧 Kustomisasi

### Menambah Soal Baru
Edit array `questions` di dalam file `vocabease.html`:

```javascript
const questions = [
    {
        type: 'listening',
        text: 'The weather is beautiful today',
        options: null
    },
    {
        type: 'multiple',
        question: 'What is the capital of France?',
        options: ['London', 'Berlin', 'Paris', 'Madrid'],
        correct: 2
    }
    // Tambah soal baru di sini
];
```

### Mengubah Tema Warna
Modifikasi CSS variables di bagian `:root`:

```css
:root {
    --primary-color: #4f46e5;
    --secondary-color: #06b6d4;
    --success-color: #10b981;
    --warning-color: #f59e0b;
    --error-color: #ef4444;
}
```

## 🤝 Kontribusi

Aplikasi ini adalah project open source. Kontribusi dalam bentuk:
- Bug reports
- Feature requests
- Code improvements
- UI/UX enhancements

## 📄 Lisensi

Project ini menggunakan lisensi MIT. Bebas digunakan untuk tujuan pembelajaran dan komersial.

## 🎯 Roadmap

- [ ] Tambah kategori soal (Grammar, Vocabulary, Reading)
- [ ] Sistem multiplayer
- [ ] Integrasi dengan API kamus
- [ ] Mode offline dengan Service Worker
- [ ] Export/import progress data
- [ ] Dark mode toggle

---

**Selamat belajar dengan VocabEase! 🚀📚**
