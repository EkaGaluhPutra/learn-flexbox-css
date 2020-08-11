disini kita akan belajar tata letak align items yang berpusat pada sumbu cross axis.

lihat di code flexbox3.css, kita punya height / besar 100px. kita tambahkan property align-items: flex-start; dan perhatikan perbedaannya.
flex item ada di atas nempel ke kiri karena flex-start adalah awal dari tata letak. coba ganti flex-start dengan flex-end. dan flex item akan berada di bawah. dan kalau di ubah valuenya ke center, flex item akan berada di tengah.

coba kita gabungkan dengan justify-content yang mengatur tata letak main axis. tambahkan properti justify-content: space-around; dan lihat perbedaannya.
dan pengaturan tata letak menjadi sempurna.

kita juga bisa mengatur satu satu flex item yang berpusat pada sumbu cross axis. tambahkan property align-self:flex-start; ke .container > div:nth-child(1n).
dan align-self: center; ke .container > div:nth-child(2n)dan align-self: flex-end; ke .container > div:nth-child(3n).

dan kita akan bahas flex-wrap.
flex-wrap di gunakan untuk responsive, ketika flex item terdiri dari 6 di tampilan dekstop, dan jika di tampilan tablet kita tidak ingin enam tapi 3 dan 3 dibawah, ini sangat berguna. lihat di flexbox3.css di baris ke 49. dan lihat di baris 56. code itu menjelaskan jika flex item memiliki lebar 200px jika sudah tidak muat untuk di tampilkan maka akan di tampilkan ke bawahnya.