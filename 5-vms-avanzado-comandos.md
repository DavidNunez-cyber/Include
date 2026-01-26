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

> Comandos requeridos: `ls, cd, pwd, mv, cp, rm, mkdir, rmdir, touch, cat, echo, nano, grep, chmod, ifconfig, ping, netstat, nmap, curl, wget, apt-get, dpkg, tar, unzip, locate, find, history, clear, exit`.[file:2]

> Nota: si `ifconfig` o `netstat` no están, instala `net-tools` (`sudo apt-get update && sudo apt-get install net-tools`) y documenta también ese paso.

| Comando | Ejemplo ejecutado (seguro) | Salida (resumen para rellenar) | Para qué sirve |
|--------|-----------------------------|---------------------------------|----------------|
| ls | `ls -la` | (captura) | Listar archivos y permisos. |
| cd | `cd /tmp` | (captura) | Cambiar de directorio. |
| pwd | `pwd` | (captura) | Mostrar ruta actual. |
| mv | `mv /tmp/a.txt /tmp/b.txt` | (captura) | Mover o renombrar archivos. |
| cp | `cp /tmp/b.txt /tmp/c.txt` | (captura) | Copiar archivos. |
| rm | `rm /tmp/c.txt` | (captura) | Borrar archivos (evita `rm -rf` en este ejercicio). |
| mkdir | `mkdir -p /tmp/lab` | (captura) | Crear directorios. |
| rmdir | `rmdir /tmp/lab` | (captura) | Borrar directorios vacíos. |
| touch | `touch /tmp/a.txt` | (captura) | Crear archivo vacío / actualizar timestamp. |
| cat | `cat /tmp/b.txt` | (captura) | Mostrar contenido de archivo. |
| echo | `echo "hola kali" > /tmp/b.txt` | (captura) | Imprimir texto o escribir a archivo. |
| nano | `nano /tmp/nano.txt` | (captura) | Editar archivos en terminal (guardar con Ctrl+O, salir Ctrl+X). |
| grep | `grep -n "hola" /tmp/b.txt` | (captura) | Buscar patrones en texto/archivos. |
| chmod | `chmod 644 /tmp/b.txt` | (captura) | Cambiar permisos (lectura/escritura/ejecución). |
| ifconfig | `ifconfig` | (captura) | Ver interfaces de red (alternativa moderna: `ip a`). |
| ping | `ping -c 4 8.8.8.8` | (captura) | Probar conectividad con número limitado de paquetes. |
| netstat | `netstat -tulpn` | (captura) | Ver puertos en escucha y procesos asociados. |
| nmap | `nmap -sV 127.0.0.1` | (captura) | Escanear puertos/servicios (usa localhost para no escanear terceros). |
| curl | `curl -I https://example.com` | (captura) | Hacer peticiones HTTP (headers, APIs, etc.). |
| wget | `wget -O /tmp/example.html https://example.com` | (captura) | Descargar archivos vía HTTP/HTTPS. |
| apt-get | `sudo apt-get update` | (captura) | Actualizar índice de paquetes e instalar/actualizar software. |
| dpkg | `dpkg -l | head` | (captura) | Listar paquetes instalados (gestión .deb). |
| tar | `tar -czf /tmp/lab.tar.gz -C /tmp b.txt` | (captura) | Comprimir/descomprimir tar (con gzip). |
| unzip | `unzip -v | head` | (captura) | Gestionar ZIP; para evidencia puedes mostrar versión/ayuda si no tienes zip real. |
| locate | `sudo updatedb` y luego `locate bash | head` | (captura) | Buscar por base de datos (requiere actualizarla). |
| find | `find /tmp -maxdepth 1 -type f -name "*.txt"` | (captura) | Buscar archivos por criterios (nombre, tipo, etc.). |
| history | `history | tail` | (captura) | Ver historial de comandos. |
| clear | `clear` | (captura) | Limpiar pantalla. |
| exit | `exit` | (captura) | Salir de la shell / cerrar terminal.
---


