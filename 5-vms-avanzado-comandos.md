# 5 - VMs Avanzado: Comandos Windows y Kali

**Objetivo**  
Completar el nivel Avanzado del apartado “Creación y Gestión de máquinas virtuales” ejecutando y documentando comandos básicos en Windows y Kali Linux.

---

## 1. Comandos en Windows (CMD dentro de la VM)

> “Usar los siguientes comandos y documentar para qué sirve cada uno:  
> `cd, dir, copy, move, del, mkdir, rmdir, ipconfig, ping, netstat, shutdown, echo, cls, type, chkdsk, format, attrib, exit`.

| Comando | Ejemplo ejecutado (seguro) | Salida (resumen para rellenar) | Para qué sirve |
|--------|-----------------------------|---------------------------------|----------------|
| cd | `cd \` | <img width="1026" height="854" alt="Screenshot 2026-01-26 120843" src="https://github.com/user-attachments/assets/886a7054-e071-4720-b745-0fc843b59864" /> | Cambiar de directorio actual. |
| dir | `dir` | <img width="1026" height="854" alt="Screenshot 2026-01-26 120939" src="https://github.com/user-attachments/assets/b9d93b67-3765-469e-8f3a-3df2ff91c2b3" /> | Listar archivos y carpetas. |
| copy | `copy C:\temp\origen.txt C:\temp\copia.txt` | <img width="1026" height="864" alt="Screenshot 2026-01-26 121718" src="https://github.com/user-attachments/assets/2c6ba30d-731b-4e01-95a0-545e2d6c6cba" /> | Copiar archivos. |
| move | `move C:\temp\copia.txt C:\temp\movido.txt` | <img width="1026" height="864" alt="Screenshot 2026-01-26 121758" src="https://github.com/user-attachments/assets/9833b657-4194-4f94-a3c0-d369661c5dd4" /> | Mover o renombrar archivos. |
| del | `del C:\temp\movido.txt` | <img width="1026" height="864" alt="Screenshot 2026-01-26 121909" src="https://github.com/user-attachments/assets/ba13f40a-824f-4a16-a691-33cc4ad3c4f5" /> | Borrar archivos. |
| mkdir | `mkdir C:\temp\lab` |<img width="1026" height="864" alt="Screenshot 2026-01-26 121957" src="https://github.com/user-attachments/assets/df12efc9-fc46-404e-aa20-64deb30e6573" /> | Crear directorios. |
| rmdir | `rmdir C:\temp\lab` | <img width="1026" height="864" alt="Screenshot 2026-01-26 122028" src="https://github.com/user-attachments/assets/8047093c-fbdb-40c5-8a9a-ba1754e48af0" /> | Borrar directorios (normalmente vacíos). |
| ipconfig | `ipconfig /all` | <img width="1026" height="864" alt="Screenshot 2026-01-26 122051" src="https://github.com/user-attachments/assets/54ea99ce-3433-458d-b037-cd4d58ecd2e8" /> | Ver configuración de red (IP, gateway, DNS, MAC). |
| ping | `ping 8.8.8.8` | <img width="1026" height="864" alt="Screenshot 2026-01-26 122113" src="https://github.com/user-attachments/assets/b07cdd60-d698-48bd-92b0-793a53ed04bc" /> | Probar conectividad hacia un host/IP. |
| netstat | `netstat -ano` | <img width="1026" height="864" alt="Screenshot 2026-01-26 122151" src="https://github.com/user-attachments/assets/8fc17b61-b7ad-4ede-9485-d1803af7b253" /> <img width="1026" height="864" alt="Screenshot 2026-01-26 122159" src="https://github.com/user-attachments/assets/3a5e9418-ca85-454d-84d7-d8fb8c77985b" /> | Ver conexiones y puertos en uso (y PID). |
| shutdown | `shutdown /s /t 60` y luego `shutdown /a` | <img width="1026" height="864" alt="Screenshot 2026-01-26 122236" src="https://github.com/user-attachments/assets/39f1e953-9a48-4740-bde4-c5353a0f0334" /> <img width="1026" height="864" alt="Screenshot 2026-01-26 122252" src="https://github.com/user-attachments/assets/731b0659-f08c-4fdd-a5c2-a04452defd32" /> | Programar apagado/reinicio y cancelarlo. |
| echo | `echo Hola Include > C:\temp\hola.txt` | <img width="1026" height="864" alt="Screenshot 2026-01-26 122412" src="https://github.com/user-attachments/assets/1907d0a7-cb04-4521-a93a-4bf6ab332efb" /> | Imprimir texto o redirigirlo a un archivo. |
| cls | `cls` | <img width="1026" height="864" alt="Screenshot 2026-01-26 122449" src="https://github.com/user-attachments/assets/3dfbf9e8-eb03-481e-9925-1a64ffbf90b5" /> <img width="1026" height="864" alt="Screenshot 2026-01-26 122454" src="https://github.com/user-attachments/assets/fc1160ed-2d43-4fe4-9585-50b3a83e0b70" /> | Limpiar pantalla de la consola. |
| type | `type C:\temp\hola.txt` | <img width="1026" height="864" alt="Screenshot 2026-01-26 122544" src="https://github.com/user-attachments/assets/fc24ee7c-b019-4c16-ba4d-0d3cf47ab376" /> | Mostrar contenido de un archivo de texto. |
| chkdsk | `chkdsk C:` | <img width="1026" height="854" alt="Screenshot 2026-01-26 123913" src="https://github.com/user-attachments/assets/36835359-7f9c-4bd0-9fc8-66cb4de0c292" /> <img width="1026" height="854" alt="Screenshot 2026-01-26 123920" src="https://github.com/user-attachments/assets/cf31c794-0108-41f6-99bf-8e5c236c483f" /> | Comprobar el estado lógico del disco. |
| format | `format /?` | <img width="1026" height="854" alt="Screenshot 2026-01-26 123953" src="https://github.com/user-attachments/assets/28e4040e-cb93-424a-b710-c1f964104d80" /> <img width="1026" height="854" alt="Screenshot 2026-01-26 124000" src="https://github.com/user-attachments/assets/5e5990b0-497c-41f1-9eae-1327a707f799" /> | Formatear unidades (en evidencia: mostrar ayuda, no ejecutar formateo real). |
| attrib | `attrib C:\temp\hola.txt` | <img width="1026" height="854" alt="Screenshot 2026-01-26 124103" src="https://github.com/user-attachments/assets/6d68fe54-46ae-41c8-ba83-74b260ce5200" /> | Ver/cambiar atributos (R, H, S, A) de archivos. |
| exit | `exit` | <img width="1026" height="854" alt="Screenshot 2026-01-26 124113" src="https://github.com/user-attachments/assets/bf3bade5-eb8e-4e0f-99e4-c4cd2fd93771" /> | Cerrar la ventana de CMD. |

---

## 2) Kali Linux (Terminal en la VM)

> Comandos requeridos: `ls, cd, pwd, mv, cp, rm, mkdir, rmdir, touch, cat, echo, nano, grep, chmod, ifconfig, ping, netstat, nmap, curl, wget, apt-get, dpkg, tar, unzip, locate, find, history, clear, exit`.

| Comando | Ejemplo ejecutado (seguro) | Salida (resumen para rellenar) | Para qué sirve |
|--------|-----------------------------|---------------------------------|----------------|
| ls | `ls -la` | <img width="725" height="885" alt="Screenshot 2026-01-26 130526" src="https://github.com/user-attachments/assets/304fec7c-9cc1-4788-835a-92b87dd100c6" /> | Listar archivos y permisos. |
| cd | `cd /tmp` | <img width="725" height="885" alt="Screenshot 2026-01-26 130557" src="https://github.com/user-attachments/assets/02294efb-c400-428b-9aca-bc26169d0da1" /> | Cambiar de directorio. |
| pwd | `pwd` | <img width="725" height="885" alt="Screenshot 2026-01-26 130612" src="https://github.com/user-attachments/assets/77f338ed-e6ad-4afc-a49b-449a178e979b" /> | Mostrar ruta actual. |
| mv | `mv /tmp/a.txt /tmp/b.txt` | <img width="725" height="885" alt="Screenshot 2026-01-26 130745" src="https://github.com/user-attachments/assets/94161a72-2183-4409-b29c-4795f287efa3" /> | Mover o renombrar archivos. |
| cp | `cp /tmp/b.txt /tmp/c.txt` | <img width="725" height="885" alt="Screenshot 2026-01-26 130810" src="https://github.com/user-attachments/assets/5785665b-6825-4929-b69f-5bf12cc8e11c" /> | Copiar archivos. |
| rm | `rm /tmp/c.txt` | <img width="725" height="885" alt="Screenshot 2026-01-26 140213" src="https://github.com/user-attachments/assets/76ada0ac-9bb1-45db-acca-bc80ac69c936" /> | Borrar archivos. |
| mkdir | `mkdir -p /tmp/lab` | <img width="725" height="885" alt="Screenshot 2026-01-26 130853" src="https://github.com/user-attachments/assets/41fc98ab-92cd-4cb8-98b9-3b7a498ac193" /> | Crear directorios. |
| rmdir | `rmdir /tmp/lab` | <img width="725" height="885" alt="Screenshot 2026-01-26 130906" src="https://github.com/user-attachments/assets/9436fab4-8760-4257-910c-27684a6cc4c3" /> | Borrar directorios vacíos. |
| touch | `touch /tmp/a.txt` | <img width="725" height="885" alt="Screenshot 2026-01-26 130928" src="https://github.com/user-attachments/assets/0ed08d33-fe24-4c0c-9ffd-6b7661d187af" /> | Crear archivo vacío / actualizar timestamp. |
| cat | `cat /tmp/b.txt` | <img width="725" height="885" alt="Screenshot 2026-01-26 130949" src="https://github.com/user-attachments/assets/eaa78e0f-eb30-44ef-af95-8a9edbecb1ab" /> | Mostrar contenido de archivo. |
| echo | `echo "hola kali" > /tmp/b.txt` | <img width="725" height="885" alt="Screenshot 2026-01-26 131006" src="https://github.com/user-attachments/assets/cace5576-74ea-4abc-b393-f168929c9f18" /> | Imprimir texto o escribir a archivo. |
| nano | `nano /tmp/nano.txt` | <img width="725" height="885" alt="Screenshot 2026-01-26 131231" src="https://github.com/user-attachments/assets/5d4fde48-a57a-4325-980e-3473c3425cf3" /> <img width="725" height="885" alt="Screenshot 2026-01-26 131255" src="https://github.com/user-attachments/assets/c19b1aed-0696-4889-8022-d81a3eb7059e" /> | Editar archivos en terminal (guardar con Ctrl+O, salir Ctrl+X). |
| grep | `grep -n "hola" /tmp/b.txt` | <img width="725" height="885" alt="Screenshot 2026-01-26 131318" src="https://github.com/user-attachments/assets/6e93172e-dbd6-4044-ae4e-2f92dae9d83a" /> | Buscar patrones en texto/archivos. |
| chmod | `chmod 644 /tmp/b.txt` | <img width="725" height="885" alt="Screenshot 2026-01-26 131414" src="https://github.com/user-attachments/assets/448a5a48-cd12-4fe9-b4e3-5aecf3c86410" /> | Cambiar permisos (lectura/escritura/ejecución). |
| ifconfig | `ifconfig` | <img width="725" height="885" alt="Screenshot 2026-01-26 131759" src="https://github.com/user-attachments/assets/f2c27928-011e-458c-bf1d-959ce4d3c716" /> | Ver interfaces de red (alternativa moderna: `ip a`). |
| ping | `ping -c 4 8.8.8.8` | <img width="725" height="885" alt="Screenshot 2026-01-26 131835" src="https://github.com/user-attachments/assets/f8a16d0d-09d1-4e3f-80ab-77a57e11378c" /> | Probar conectividad con número limitado de paquetes. |
| netstat | `netstat -tulpn` | <img width="725" height="885" alt="Screenshot 2026-01-26 131926" src="https://github.com/user-attachments/assets/cf714262-7c4c-4d05-9549-3ba8fe686427" /> | Ver puertos en escucha y procesos asociados. |
| nmap | `nmap -sV 127.0.0.1` | <img width="725" height="885" alt="Screenshot 2026-01-26 131950" src="https://github.com/user-attachments/assets/e875584c-4032-45b3-b8ad-e78214d52130" /> | Escanear puertos/servicios (usa localhost para no escanear terceros). |
| curl | `curl -I https://example.com` | <img width="725" height="885" alt="Screenshot 2026-01-26 132024" src="https://github.com/user-attachments/assets/35449420-3fc0-4dc0-88a4-b3660090a622" /> | Hacer peticiones HTTP (headers, APIs, etc.). |
| wget | `wget -O /tmp/example.html https://example.com` | <img width="725" height="885" alt="Screenshot 2026-01-26 132048" src="https://github.com/user-attachments/assets/a8f9d8ee-622b-46bf-bbb7-265b6f860023" /> | Descargar archivos vía HTTP/HTTPS. |
| apt-get | `sudo apt-get update` | <img width="725" height="885" alt="Screenshot 2026-01-26 132115" src="https://github.com/user-attachments/assets/4ba7e914-7e9a-4749-8b89-d527522b791a" /> | Actualizar índice de paquetes e instalar/actualizar software. |
| dpkg | `dpkg -l \| head` | <img width="725" height="885" alt="Screenshot 2026-01-26 132140" src="https://github.com/user-attachments/assets/081604f6-216d-41ce-82c6-6f562614d552" /> | Listar paquetes instalados (gestión .deb). |
| tar | `tar -czf /tmp/lab.tar.gz -C /tmp b.txt` | <img width="725" height="885" alt="Screenshot 2026-01-26 132212" src="https://github.com/user-attachments/assets/18f57a36-bc5e-4ba0-b891-da770eccce76" /> | Comprimir/descomprimir tar (con gzip). |
| unzip | `unzip -v \| head` | <img width="725" height="885" alt="Screenshot 2026-01-26 132259" src="https://github.com/user-attachments/assets/a8039cf5-604e-4778-966c-ea47d8049a0d" /> | Gestionar ZIP; para evidencia puedes mostrar versión/ayuda si no tienes zip real. |
| locate | `sudo updatedb` y luego `locate bash \| head` | <img width="725" height="885" alt="Screenshot 2026-01-26 132342" src="https://github.com/user-attachments/assets/ddf7f8f0-cfae-4d73-850b-69d0bee40385" /> | Buscar por base de datos (requiere actualizarla). |
| find | `find /tmp -maxdepth 1 -type f -name "*.txt"` | <img width="725" height="885" alt="Screenshot 2026-01-26 132411" src="https://github.com/user-attachments/assets/58c01013-a11d-4988-9291-6c86cb01605f" /> | Buscar archivos por criterios (nombre, tipo, etc.). |
| history | `history \| tail` | <img width="725" height="885" alt="Screenshot 2026-01-26 132439" src="https://github.com/user-attachments/assets/d15f1c21-bd71-4515-a016-e44f9103677c" /> | Ver historial de comandos. |
| clear | `clear` | <img width="725" height="885" alt="Screenshot 2026-01-26 132451" src="https://github.com/user-attachments/assets/28a34536-6f36-4c60-bfb0-da57dd42e14d" /> <img width="725" height="885" alt="Screenshot 2026-01-26 132457" src="https://github.com/user-attachments/assets/ef830c52-74ef-45b7-81e6-27ba1940d7cd" /> | Limpiar pantalla. |
| exit | `exit` | <img width="725" height="885" alt="Screenshot 2026-01-26 132504" src="https://github.com/user-attachments/assets/e9be7c50-a7d1-4f05-94da-e48a4c046c2a" /> <img width="725" height="885" alt="Screenshot 2026-01-26 132510" src="https://github.com/user-attachments/assets/9c60440a-1614-4542-b1bc-b50f4b2f4f12" /> | Salir de la shell / cerrar terminal.

---

## Tiempo invertido
- Total: 3 horas.
- Bloqueos: Ninguno 

---

*Documentado por David Nuñez - Preparación curso IT/Ciberseguridad marzo 2026. Fundación GoodJob.*
