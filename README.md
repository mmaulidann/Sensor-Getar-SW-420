Sensor getar SW-420 dapat bereaksi terhadap getaran dari berbagai sudut. Pada 
kondisi statis / tanpa getaran, komponen elektronika berfungsi seperti saklar yang 
berada pada kondisi menutup (normally closed) dan bersifat kondiktif, sebaliknya 
pada terguncang (terpapar getaran). saklar akan membuka / menutup dengan 
kecepatan pengalihan (switching frequency) proporsional dengan kekerapan 
guncangan. Pengalihan bergantian secara cepat ini mirip seperti cara kerja PWM 
(pulse width modulation) yang merupakan sinyal pseduo-analog berupa tingkat 
tegangan yang kemudian dibandingkan oleh sirkuit terpadu LM393 (Voltage 
Comparator IC) dengan besar nilai ambang batas (treshold) tegangan pembanding 
diatur oleh sebuah resistor eksternal.
 Adapun cara kerja sensor getar SW-420 dari experiment ini yaitu sensor akan 
mendeteksi segala bentuk guncangan/getaran yang ditimbulkan kemudian akan 
ditandakan dengan indikator 2 buah LED yang disiapkan. Ketika sensor getar SW420 menerima getaran maka indikator LED Biru akan menyala dan nilai yang 
ditampilkan pada serial monitor bernilai 1. Sedangkan ketika sensor tidak menerima 
getaran maka akan ditandai dengan indikator lampu LED Orange yang menyala dan 
nilai yang ditampilkan pada serial monitor sebesar 0
