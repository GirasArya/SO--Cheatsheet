## pindah ke direktori home
$ cd home/

## Buat Folder 'test'
$ mkdir test

## masuk ke direktori 'test'
$ cd test

## Menampilkan path direktori
$ pwd

## buat file kosong 
$ touch empty.txt

## copy file '/etc/timezone'
$ cp [OPTION] [SOURCE FOLDER/FILE] [copied file name]

## Rename file 
$ mv [OLD FILE/FOLDER] [NEW FILE/FOLDER]

## list direktori 
$ ls

## pindah ke direktori parent
$ cd ../ atau cd ~

## hapus direktori 
$ rm -r [dir]

## tampilkan 5 baris pertama 
$ head -n [File] // n jumlah baris
$ head -5 last

## tampilkan dua baris
$ tail -n [File] // n jumlah baris
$ tail -2 /etc/passwd

## cari file di pada folder yang memuat suatu kata
$ grep [OPTION] 'PATTERN' [FILE]
$ grep 'sem_post' /usr/include

## tampilkan kolom 1 dan 5
$ awk '{print $1, $5}' [FILE]
$ awk '{print $1, $5}' /etc/passwd


## tampilkan isi file dalam huruf kapital
$ awk 'print toupper($0)' [FILE]
$ awk 'print toupper($0)' /etc/motd

## jalankan `cat /dev/random > rand.txt` di background
$ cat /dev/random > rand.txt &

## tampilkan daftar job
$ ps [OPTION]
$ pstree


## kirim sinyal STOP ke job tersebut
// pake ps buat nyari pid bisa sih awkwkwk
$ pstree -p 
atau 
$ pidof [program]

$ kill [option] PID
$ kill -STOP PID

## lanjutkan job tersebut di background
$ jobs //untuk cari proses yang jalan / berhenti
$ bg %[id]

## kirim sinyal TERM ke job tersebut
$ kill [option] PID //default SIGTERM / terminate
