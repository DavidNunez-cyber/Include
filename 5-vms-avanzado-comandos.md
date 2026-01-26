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
| mkdir | `mkdir C:\temp\lab` | (captura) | Crear directorios. |
| rmdir | `rmdir C:\temp\lab` | (captura) | Borrar directorios (normalmente vacíos). |
| ipconfig | `ipconfig /all` | (captura) | Ver configuración de red (IP, gateway, DNS, MAC). |
| ping | `ping 8.8.8.8` | (captura) | Probar conectividad hacia un host/IP. |
| netstat | `netstat -ano` | (captura) | Ver conexiones y puertos en uso (y PID). |
| shutdown | `shutdown /s /t 60` y luego `shutdown /a` | (captura) | Programar apagado/reinicio y cancelarlo. |
| echo | `echo Hola Include > C:\temp\hola.txt` | (captura) | Imprimir texto o redirigirlo a un archivo. |
| cls | `cls` | (captura) | Limpiar pantalla de la consola. |
| type | `type C:\temp\hola.txt` | (captura) | Mostrar contenido de un archivo de texto. |
| chkdsk | `chkdsk C:` | (captura) | Comprobar el estado lógico del disco. |
| format | `format /?` | (captura) | Formatear unidades (en evidencia: mostrar ayuda, no ejecutar formateo real). |
| attrib | `attrib C:\temp\hola.txt` | (captura) | Ver/cambiar atributos (R, H, S, A) de archivos. |
| exit | `exit` | (captura) | Cerrar la ventana de CMD. |


---

## 2. Comandos en Kali Linux (Terminal dentro de la VM)

> “Usar los siguientes comandos y documentar para qué sirve cada uno:  
> `ls, cd, pwd, mv, cp, rm, mkdir, rmdir, touch, cat, echo, nano, grep, chmod, ifconfig, ping, netstat, nmap, curl, wget, apt-get, dpkg, tar, unzip, locate, find, history, clear, exit`.

| Comando | Ejemplo ejecutado | Salida (resumen) | Para qué sirve |
|---------|-------------------|------------------|----------------|
| ls      | `ls`              | Lista archivos   | Ver contenido de la carpeta |
| cd      | `cd /tmp`         | Cambia a /tmp    | Cambiar de directorio |
| pwd     | `pwd`             | Muestra ruta     | Saber dónde estoy |
| mv      | ...               | ...              | Mover/renombrar archivos |
| cp      | ...               | ...              | Copiar archivos |
| rm      | ...               | ...              | Borrar archivos |
| mkdir   | ...               | ...              | Crear directorios |
| rmdir   | ...               | ...              | Borrar directorios vacíos |
| touch   | ...               | ...              | Crear/actualizar archivos vacíos |
| cat     | ...               | ...              | Mostrar contenido de archivo |
| echo    | ...               | ...              | Imprimir texto/variables |
| nano    | ...               | ...              | Editor de texto en terminal |
| grep    | ...               | ...              | Buscar texto en salida/archivos |
| chmod   | ...               | ...              | Cambiar permisos |
| ifconfig| ...               | ...              | Ver interfaces (o `ip a`) |
| ping    | ...               | ...              | Probar conectividad |
| netstat | ...               | ...              | Ver conexiones/puertos (o `ss`) |
| nmap    | ...               | ...              | Escanear puertos/hosts |
| curl    | ...               | ...              | Peticiones HTTP desde terminal |
| wget    | ...               | ...              | Descargar archivos |
| apt-get | ...               | ...              | Gestionar paquetes (instalar/actualizar) |
| dpkg    | ...               | ...              | Gestionar paquetes .deb |
| tar     | ...               | ...              | Comprimir/descomprimir archivos tar |
| unzip   | ...               | ...              | Descomprimir zip |
| locate  | ...               | ...              | Buscar archivos (base actualizada) |
| find    | ...               | ...              | Buscar archivos con filtros |
| history | ...               | ...              | Ver historial de comandos |
| clear   | ...               | ...              | Limpiar pantalla |
| exit    | `exit`            | Cierra terminal  | Salir de la shell |

---


