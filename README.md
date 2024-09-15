# FlugSimulator
Bewegung entlang geodätischer Linien auf der Erdkugel

![image](https://github.com/user-attachments/assets/2c1fe583-0ed8-4c33-be48-165be1588b34)

## Vorgehensweise
Es wurden mathematische Formeln im 3D-Raum benutzt.

### Punkte auf der Kugel
Die Punkte auf der Kugel wurden mit Hilfe von geografischen Kugelkoordinaten und dem radius berechnet.

![image](https://github.com/user-attachments/assets/dfc024c8-4d80-4d52-8f88-fc487fa295fc)

### Winkelberechnung zwischen 2 Vektoren
Der Winkel wurde aus dem Skalarprodukt aus den Einheitsvektoren zu den jeweiligen Punkten berechnet

![image](https://github.com/user-attachments/assets/d0e28545-b59f-43c1-986d-72472dc96e9a)

### Großkreis
Für die Bestimmung des Großkreises wurde folgende Vorgehensweise benutzt:

![image](https://github.com/user-attachments/assets/a971b778-6d15-4a1d-89d4-bc84c8579855)

#### Bestimmung der Drehmatrix
1. Drehen des Einheitsvektors in X-Richtung auf den Einheitsvektor, der in Richtung des ersten Punktes zeigt
2. z auf Einheitsvektor n (n sthet orthogonal auf beide Vektoren)
3. y auf Einheitsvektor u orthogonal zu n und p
4. Drehung des Vektor => Drehmatrix * Vektor
5. Drehmatrix [p u n]

#### Parameterformel Großkreis
Die Parameterformel des Großkreises lautet nun:

![image](https://github.com/user-attachments/assets/5395ae44-3724-455f-b251-598689c57a69)

Wenn für t-Werte zwischen 0 und Theta eingesetzt werden, bekommz man die jeweilige Vektoren zu Punkten, welche auf der Kurve auf dem Großkreis zwischen Start und Endpunkt liegen, heraus.
Diese beschreiben die Flugroute.

### Projektion von 3D auf 2D (Bildschirm)

![image](https://github.com/user-attachments/assets/1853045b-03b0-46c8-817f-52ecd3380e8c)
![image](https://github.com/user-attachments/assets/6b8dd2e4-e6a0-4200-bac9-daabf1bb2886)

#### Formel:
![image](https://github.com/user-attachments/assets/bb825c97-2b31-4324-be11-54af434cf699)

### Drahtgittermodell mit Umrisselipse
Das Drahtgittermodell wurde gemacht indem Vektoren z uden Punktern, welche die Großkreise des Drahtgittermodells Beschreiben, erzeugt und die jeweiligen Punkte zeichnet.

![image](https://github.com/user-attachments/assets/2a5da67f-d753-4611-9d2f-0a9403ab538b)

#### Umrisselipse
![image](https://github.com/user-attachments/assets/9b422fcc-204a-4e65-9dde-59c59a58c4f6)





