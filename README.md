##e-book reader

![image](https://github.com/user-attachments/assets/f0dca005-5e76-41f9-93e5-f9a191230d6c)


##Bill of Materials (BOM)

![image](https://github.com/user-attachments/assets/0e01b04d-baaf-4a38-97ce-78c1fccab934)


##Conexiuni și module hardware utilizate:
•	USB-C Connector + ESD Protection
-	Intrare principală de alimentare și programare.
•	LDO Voltage Regulator
-	Reglează tensiunea de intrare la 3.3V stabil pentru alimentarea ESP32 și altor componente.
•	Li-Po Battery Charging Controller
-	Încarcă un acumulator Li-Po de la 5V (USB)
•	ESP32-C6
-	Microcontroller principal - responsabil de control, procesare si comunicare
•	E-Paper Drive Circuit
-	Oferă semnalul de putere necesar pentru activarea e-paper-ului
•	Display Type Selector
-	Permite comutarea
•	Voltage Supervisor + Reset
-	Asigură resetul corect la pornire
Poziționarea componentelor a fost gândită pentru:
•	acces facil la butoane,
•	vizibilitatea e-paper-ului,
•	montarea sigură a bateriei cu suport mecanic.
(pe baza schemei si recomandarilor primite)

##Functionalitate Hardware:
**Componente, Module și Senzori**
**Alimentare și Management Energie**
 Conector USB-C + Protecție ESD
 Funcție: Asigură alimentarea principală a sistemului și protejează împotriva descărcărilor electrostatice.
 
 Controler Încărcare Baterie – MCP73831
 Funcție: Gestionează încărcarea bateriei Li-Po, controlează curentul de încărcare.
 
 Baterie Li-Po
 Funcție: Sursă de alimentare secundară pentru funcționare autonomă (fără USB).
 
 Regulator de Tensiune LDO (3.3V)
 Funcție: Stabilizează tensiunea de alimentare pentru microcontroler și restul componentelor.
 
 Supervizor Tensiune + Buton Reset/Boot
 Funcție: Monitorizează nivelul tensiunii de alimentare și permite resetarea sau intrarea în modul boot al ESP32-C6.

**Control și Procesare:**
 ESP32-C6-WROOM-1-N8
 Funcție: Microcontroler principal. Gestionează comunicațiile (SPI, I2C, UART), interacțiunea cu senzorii și controlul perifericelor. Oferă conectivitate Wi-Fi și Bluetooth Low Energy.
 
 Memorie Externă NOR Flash – 64MB
 Funcție: Stocare extinsă pentru firmware și date.
 Interfață: SPI.

**Timp Real:**
 Modul RTC – DS3231SN
 Funcție: Ceas de timp real de înaltă precizie, cu suport pentru alarmă și funcționare pe baterie de backup.
 Interfață: I2C.

**Senzori de Mediu:**
 BME688 – Senzor ambiental
 Funcție: Măsoară temperatura, umiditatea, presiunea atmosferică și compușii organici volatili (VOC).
 Interfață: I2C (Qwiic / Stemma QT pentru conectare rapidă).
 Consum: Standby ultra-low power, activ ~3.1 mA.

**Afișaj:**
 Circuit de control pentru ecran E-Paper + Header de conectare
 Funcție: Generează semnalele necesare pentru funcționarea ecranelor E-Paper.
 Interfață: SPI cu linii de control dedicate (Busy, Reset, DC, CS).

**Stocare locală:**
 Slot Card microSD
 Funcție: Permite salvarea datelor local (loguri, configurări, fișiere).
 Interfață: SPI, cu semnal Chip Select dedicat.

**Interfețe de Comunicație:**
 I2C: Utilizat pentru BME688 și DS3231SN.
 SPI: Utilizat pentru NOR Flash, E-Paper Display și Card SD.
 UART: Disponibil pentru debug sau extensii opționale.
 Wi-Fi & Bluetooth LE: Oferite de modulul ESP32-C6.

![image](https://github.com/user-attachments/assets/82fb4581-66f3-4a63-aa71-735fee8700ba)

##PCB_2D:
 

![Screenshot 2025-04-14 160136](https://github.com/user-attachments/assets/6044687e-4dcb-4780-9697-1aaa23781730)



##PCB_3D:
 
![Screenshot 2025-04-14 125641](https://github.com/user-attachments/assets/18c22c55-3fa6-4fb3-b62a-33a25a4e5761)


