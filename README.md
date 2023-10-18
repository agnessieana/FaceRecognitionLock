# Face Recognition Lock

Project yang saya ambil adalah FaceDoor yang dibuat oleh HunterJhonson
https://github.com/HunterJohnson/FaceDoor
FaceDoor adalah project yang dibuat untuk membuka dan mengunci pintu menggunakan pengenalan wajah

## Face Recognition

![result882](https://github.com/agnessieana/FaceRecognitionLock/assets/148158189/789599a0-8ee6-4e9f-b160-59f30a27ef12)

Face recognition atau “pengenalan wajah” adalah teknologi yang digunakan untuk mengidentifikasi dan mengautentikasi individu berdasarkan karakteristik wajah mereka. Teknologi ini menggunakan analisis pola dan pengenalan pada fitur wajah seseorang, seperti bentuk mata, hidung, mulut, dan struktur wajah lainnya. Proses pengenalan wajah ini biasanya dilakukan dengan menggunakan software atau algoritma khusus yang dapat mengolah gambar wajah dan membandingkannya dengan data referensi yang  ada.

## Raspberry Pi

![Bagian-bagian Raspberry Pi](https://github.com/agnessieana/FaceRecognitionLock/assets/148158189/43821272-f556-438f-80e2-bb69bf465a62)

Raspberry Pi merupakan komputer mini yang dibuat oleh Raspberry Pi Foundation dan dapat digunakan untuk berbagai macam aplikasi. Ini mendukung banyak sistem operasi yang berbeda, termasuk Raspberry Pi OS, dan dapat digunakan untuk berbagai proyek, seperti belajar dan mengajar. Raspberry Pi memiliki beragam port dan koneksi, termasuk jaringan, USB, HDMI, dan GPIO, memungkinkannya terhubung ke banyak perangkat eksternal dan periferal. Cocok untuk hiburan rumah dan pusat media  karena kemampuan multimedianya yang sangat baik. Berbagai versi dan model Raspberry Pi meningkatkan kinerja dan kompatibilitas.

## Perangkat Keras

Berikut adalah perangkat keras yang digunakan dalam project:
* Raspberry Pi 3 
* Camera of choice (I used a NoIR that cost about $25 on Amazon)
* 12V lock style solenoid
* Hammer/nails or Drill/screws to secure the lock to your door of choice (or even just strong tape if you want to test it out)
* 5V relay
* 12V power supply + DC adapter

## Perangkat Lunak 

Berikut adalah perangkat lunak yang dibutuhkan project:
* picamera 
* OpenCV
* Keras / Tensorflow
* various Python libraries

## Struktur Project
 

    while(door_is_active):
    
         if motion_detected():
       
             if face_detected():
     
                 if valid_entrant(img):
          
                     unlock_door()
                 
                 else:
          
                     "Access Denied"
      
