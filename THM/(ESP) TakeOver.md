# TakeOver

> Plataforma: THM

> Dificultad: Easy

---

## Task 1 - Help us

<img width="1289" height="390" alt="Captura de pantalla 2026-03-01 223814" src="https://github.com/user-attachments/assets/d3b70812-7fff-4c38-832c-dbba56a52bc0" />

---

## Solución
Primero, nos conectamos al VPN que nos da Try Hack Me con el comando openvpn:

<img width="428" height="36" alt="TakeOver01" src="https://github.com/user-attachments/assets/c1b7d56a-ae57-4137-80fa-f6fc6ec081a8" /><br>

<img width="438" height="14" alt="TakeOver02" src="https://github.com/user-attachments/assets/23b16ffb-484a-48d1-92b3-7816ee70e986" /><br>

Luego, añadimos el enlace futurevera.thm al /etc/hosts con la IP que nos asigna:

<img width="252" height="37" alt="TakeOver03" src="https://github.com/user-attachments/assets/1818b652-579e-4fd7-b15d-e59ee4ecd5dd" /><br>

<img width="235" height="18" alt="TakeOver04" src="https://github.com/user-attachments/assets/a39fb024-6a89-4397-8439-24f65b95bec6" /><br>

Siguiendo lo que nos indica el task 1, nos indican "we are rebuilding our support", así que añadimos un subdominio support al /etc/hosts:

<img width="424" height="20" alt="TakeOver06" src="https://github.com/user-attachments/assets/8858f0c9-2792-48b5-acc9-fa5d7a3a09c4" /><br>

Ingresamos a la página y nos aparece lo siguiente:

<img width="890" height="251" alt="TakeOver07" src="https://github.com/user-attachments/assets/fafd3961-7780-4204-b7c8-524498c40986" /><br>

Hacemos click en "Advanced..." y analizando en "View Certificate" encontramos nueva información:

<img width="772" height="261" alt="TakeOver08" src="https://github.com/user-attachments/assets/994cf557-9c33-4c4c-bac0-e6acb8ba496d" /><br>

<img width="495" height="71" alt="TakeOver09" src="https://github.com/user-attachments/assets/3776da8b-9d55-4974-8f96-957e4208872b" /><br>

Añadimos este subdominio al /etc/hosts y lo analizamos:

<img width="782" height="21" alt="TakeOver10" src="https://github.com/user-attachments/assets/5b550fb7-96ce-406c-9f03-706a2969c4d4" /><br>

<img width="371" height="28" alt="TakeOver11" src="https://github.com/user-attachments/assets/4c50a6af-6287-45b2-b4e1-7bc83bd39f6c" /><br>

Al cargar nos entrega este enlace con la flag:

<img width="581" height="26" alt="TakeOver12" src="https://github.com/user-attachments/assets/4bdffda0-cf6f-407c-b417-ce9a50329bae" />

