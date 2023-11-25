# pindah ke direktori home anda
$ cd home/

# buat satu folder kosong 'test'
$ mkdir test

# masuk ke direktori 'test'
$ cd test

# tampilkan path direktori saat ini
$ pwd

# buat file kosong bernama 'empty.txt'
$ touch empty.txt

# copy file '/etc/timezone' ke direktori ini
$ cp [OPTION] [SOURCE FOLDER/FILE] [copied file name]

# ubah nama file 'timezone' menjadi 'tz.txt'
$ mv [OLD FILE/FOLDER] [NEW FILE/FOLDER]

# list isi direktori ini
$ ls

# pindah ke direktori parent
$ cd ../ atau cd ~

# hapus direktori 'test' seisinya
$ rm -r [dir]

# tampilkan 5 baris pertama keluaran perintah `last`
$ head -n [File] # n jumlah baris
$ head -5 last

# tampilkan dua baris terakhir file '/etc/passwd'
$ tail -n [File] # n jumlah baris
$ tail -2 /etc/passwd

# cari file di '/usr/include' yang memuat kata 'sem_post'
$ grep [OPTION] 'PATTERN' [FILE]
$ grep 'sem_post' /usr/include

# tampilkan kolom 1 dan 5 dari file '/etc/passwd'
$ awk '{print $1, $5}' [FILE]
$ awk '{print $1, $5}' /etc/passwd


# tampilkan isi file '/etc/motd' dalam huruf kapital
$ awk 'print toupper($0)' [FILE]
$ awk 'print toupper($0)' /etc/motd

# jalankan `cat /dev/random > rand.txt` di background
...
# tampilkan daftar job
...
# kirim sinyal STOP ke job tersebut
...
# lanjutkan job tersebut di background
...
# kirim sinyal TERM ke job tersebut
...
