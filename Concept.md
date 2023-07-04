## Tujuan
Gamifikasi hidup untuk mometivasi kita berbuat hal yang produktif menggunakan Chat GPT 4

## Alur user
1. User menginisialisasi chat (/start)
2. tahap pembentukan karakter
    - user mengisi biodata
    - user mengisi keahlian yang dia miliki
        - sistem akan membuat satu kategory mastery untuk setiap keahlian yang user submit
        - sistem akan mengkalkulasi level berapa user tersebut berdasarkan konteks yang dia berikan
3. Sistem akan memberi tahu user stats dia setelah mendapatkan konteks mengenai user
    - tampilkan statistik  menggunakan diagrams
    - jika statistik dirasa kurang akurat, user bisa mengubahnya 
    - jika statistik user dirasa
4. game dimulai dan sistem siap menerima input dari user

## Elemen didalam game

### Leveling system
setiap level membutuhkan exp yang sama untuk leveling up yaitu 250exp, tidak ada batas pada level umum, hal yang bisa meningkatkan level adalah semua kegiatan produktif yang dilakukan pemain, dan setiap aktivitas buruk atau tidak produktif akan mengurangi experience dari pemain 

### Professions
Profesions adalah pekerjaan yang sedang dimiliki oleh user misal (bakery, fullstack software developer, HRD, siswa SMA)

### Skill
skill adalah keahlian yang dimiliki user dan terikat pada profesi yang dimiliki oleh user 
misal Typescript, express, nuxt, ai prompting untuk fullstack developer. Deep focus, pomodoro technique, focus read untuk siswa SMA

penamaan skill mungkin bisa disajikan dalam style MMORPG

### Physical and Mental Attributes
Atribut fisik seperti kekuatan, otot, kecepatan, lompat (tapi elemen ini harus merepresentasikan data aktual yang terjadi di real life, misal ai tidak bisa menebak secara pasti berapa kalori yang dibakar user ketika bersepeda sehingga dapat mengkalkuklasi berat badan yang sekarang)

### Habits
habits adalah kebiasaan, diperlukan 21 hari untuk membuat sebuah habits, habits bisa terikat ke mastery yang relevan dengan habits tersebut.

### Quest
Quest adalah task tidak wajib yang harus diselesaikan oleh user jika ingin mendapaktan exp.

Quest tergantung dengan banyaknya waktu luang yang dimiliki oleh user perharinya, user bisa mengatur waktu luang default yang dia miliki untuk satu hari. tapi user tersebut dapat menentukan waktu luangnya untuk hari spesifik

### Achievements
Achievments adalah pencapaian yang didapatkan oleh user

achievement akan ada tergantung dari profesi yang dimiliki oleh user

jika user mencapai achievment tertentu dia bisa mendapatkan badges

concern: bagaimana ai menentukan apa saja achievements yang bakalan bisa diraih oleh user?
sepertinya achievments ini harus dibuat manual

## Jenis-jenis user input
game ini tergantung dari input user untuk kemajuannya berikut adalha beberapa input yang bisa dilakukan oleh user

### Activity Input
user melakukan input terharap aktivitas yang telah dia lakukan.

"saya telah melakukan pushup sebanyak 40 kali"

- sistem harus mengkalkulasikan apa saja profesi, skills, achievements, yang akan dipengaruhi oleh input baru ini
- sistem harus mengkalkulasikan exp yang didapatkan oleh user untuk setiap profesi, skills, achievements.
- jika belum ada profesi atau skill  yang relevan terhadap aktivitas user. dan user sudah melakukan hal ini berulang kali (revisit this concept) maka sistem harus membuat profesi atau skill baru untuk user tersebut
- sistem juga harus melihat peningkatan stats yang bisa terjadi

## Mekanik game
- skill decay, dimana user jarang melakukan skill, profesi sehingga skill atau profesi tersebut menjadi tidak terlatih lagi