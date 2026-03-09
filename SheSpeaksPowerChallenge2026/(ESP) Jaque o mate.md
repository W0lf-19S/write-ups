# Jaque o mate

> Plataforma: hackrocks

> Dificultad: Medio

> Categoría: FORENSICS - Digital forensics

---

## Descripción

<img width="1204" height="683" alt="JoM 1" src="https://github.com/user-attachments/assets/9681242c-0a1e-4aca-bace-56c7c3046ae2" /><br>

---

## Solución
Como no hay más información, empezamos analizando el archivo que nos adjunta el reto `capture-output.pcap` haciendo uso de Wireshark:

<img width="1140" height="342" alt="JoM 2" src="https://github.com/user-attachments/assets/955f1943-ada7-4794-9e8d-b69eb5d8b69c" /><br>

Hacemos seguimiento por HTTP Stream y encontramos lo siguiente:

<img width="653" height="683" alt="JoM 3" src="https://github.com/user-attachments/assets/ee808b4d-8240-40e7-894c-276903d22dda" /><br>

<img width="1247" height="452" alt="JoM 4 - cen" src="https://github.com/user-attachments/assets/d4c7b7e6-ad91-4208-acf7-404f8a30ab14" /><br>

Hacemos seguimiento por TCP Stream y encontramos lo siguiente:

<img width="708" height="257" alt="JoM 5 - cen" src="https://github.com/user-attachments/assets/77f3d67a-3160-4f5c-85fd-03bccd8948da" /><br>

Desencriptamos lo encontrado en el HTTP Stream:

<img width="1057" height="265" alt="JoM 6 - cen" src="https://github.com/user-attachments/assets/caf4d457-ee2f-46ab-a71c-048a176961f8" /><br>

Y lo usamos como contraseña para el archivo ZIP encontrado en TCP Stream:

<img width="1186" height="432" alt="JoM 7 - cen" src="https://github.com/user-attachments/assets/340be828-6052-42e3-9b1a-7f0612b87a95" /><br>

Y obtenemos la flag:

<img width="657" height="542" alt="finish SSPC2026 CTF" src="https://github.com/user-attachments/assets/fa3f9377-9bbd-4912-a66b-d1666b1c6429" />
