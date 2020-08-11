oke disini kita akan membahas flex model.
https://media.prod.mdn.mozit.cloud/attachments/2012/07/09/3739/97750afee8f091f8b82864be884a3695/flex_terms.png

kalian liat gambar ini.
flex container adalah induk dari element yang ingin kita gunakan flex. contoh disini div class container dan section adalah flex container.
flex item adalah element yang ingin kita gunakan flex. contoh disini kita ada 3 tag div di dalam div class container dan 3 tag article di dalam section.
main axis adalah urutan baris / row dari kanan ke kiri.
main start adalah awal dari urutan row.
main end adalah akhir dari urutan row.

cross axis adalah urutan kolom / column dari atas ke bawah.
cross start adaalah urutan awal dari urutan kolom.
cross end adalah urutan akhir dari uruan kolom.

bisa di bilang kalo main itu sumbu x dan cross sumbu y.

default dari flex adalah urutan tampilan nya row / baris dari kanan ke kiri, coba ganti dengan memasukan flex-direction ke induk element.

disini kita menambahkan properti justify content.
justify content mengatur tampilan main axis.
di properti ini ada flex-start, flex-end, space-around, space-evenly dan masih banyak lagi yang bisa kalian coba.

walaupun menggunakan flex, kita masih bisa mengatur lagi posisi dari flex-item itu sendiri. contoh disini kita membuat flex-item nempel ke flex end di kanan, dan kita akan membuat class home menempel ke kiri, lihat di 
.container .home

flex sizing di flex items.
kita akan memberi nilai proporsi tanpa unit yang menentukan berapa banyak ruang yang tersedia di sumbu utama dan setiap flex-item akan disesuaikan dan dibandingkan dengan flex-item yang ada di sumbu tersebut.
contoh kita memberi proporsi ke tag article yang ada di dalam section. dengan properti flex: 1; memberitahu bahwa setiap elemet flex-item akan mendapatkan proporsi satu dari elemet flex-item lain di sumbu tersebut.
dan kita tambahkan flex: 2; ke article urutan 2 dan lihat bahwa proporsi element ini 2 kali lipat dari article yang lain.