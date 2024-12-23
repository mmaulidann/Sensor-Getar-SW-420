//Sensor getar
const int pinGetar = 3;     //inisialisasi pin sensor
const int ledBlue = 8;       //inisialisasi pin LED
const int ledOrange = 7;     //inisialisasi pin LED

void setup() {
Serial.begin (9600);        //program menyalakan serial monitor
pinMode (ledBlue, OUTPUT);   //menetapkan pin 8 sebagai output
pinMode (ledOrange, OUTPUT); //menetapkan pin 7 sebagai output
}

void loop() {
//Membaca data dari pin yang dihubungkan ke sensor kemudian di tampilkan di serial monitor
int datadigital = digitalRead (pinGetar);
Serial.print ("Sensor : ");
Serial.print (datadigital);

//Program ketika sensor mendeteksi guncangan
if (datadigital == 1) {
  Serial.println (" mendeteksi getaran");
  digitalWrite (ledBlue, HIGH);
  digitalWrite (ledOrange, LOW);
}

//Program ketika sensor tidak mendeteksi guncangan
else if (datadigital == 0) {
  Serial.println (" Tidak mendeteksi getaran");
  digitalWrite (ledBlue, LOW);
  digitalWrite (ledOrange, HIGH);
}
}
