# 4 - Creación y Gestión de Máquinas Virtuales (Inicial → Intermedio+)

**Objetivo**  
Completar los niveles Inicial, Intermedio e Intermedio+ del apartado  
“Creación y Gestión de máquinas virtuales” del itinerario #INCLUDE.

---

## 1. Nivel Inicial – Descarga e instalación de hypervisores

Según el documento:  
> “Inicial (…) descarga VirtualBox (https://www.virtualbox.org/) y Vmware (https://www.vmware.com/) de la página principal.”

| Tool | Versión | Link oficial | Captura instalación |
|------|:-------:|--------------|---------------------|
| **Oracle VirtualBox** | 7.2.4 | [VirtualBox](https://www.virtualbox.org/) | ![VirtualBox Screenshot](https://github.com/user-attachments/assets/271fab2d-b1cf-4763-8708-0436e45c5922) |
| **VMware Workstation Pro** | 25H2 | [VMware](https://www.vmware.com/products/desktop-hypervisor/workstation-and-fusion) | ![VMware Screenshot](https://github.com/user-attachments/assets/66f78035-8dea-4e9d-bafa-935082eaadcf) |

## 2. Nivel Intermedio – Descarga de ISOs

El documento indica descargar las siguientes ISOs: 
> “Kali Linux, Windows 10, Windows 11”

En mi caso, por disponibilidad actual, usaré **Windows 11** en lugar de Windows 10, manteniendo el mismo objetivo (una VM Windows + una VM Kali).[2]

| VM | Fuente | Link descarga | Captura VM en hypervisor |
|----|--------|----------------|--------------------------|
| **Kali Linux** | Offensive Security | [Pre-built Virtual Machines](https://www.kali.org/get-kali/#kali-virtual-machines) | <img width="898" height="533" alt="Kali VM Screenshot" src="https://github.com/user-attachments/assets/ce2401b4-71f6-4c6d-b5e2-5573ee1f45f4" /> |
| **Windows 11** | Microsoft | [Windows 11](https://www.microsoft.com/es-es/software-download/windows11/) | <img width="1097" height="751" alt="Windows 11 VM Screenshot" src="https://github.com/user-attachments/assets/4ed684ac-1ee4-41d6-aad8-0f76a76c0796" /> |

## 3. Nivel Intermedio+ – Creación de VMs (Windows 11 y Kali)

El documento pide:
> “Crear una máquina virtual de Windows 10 y documentar cómo has realizado la instalación paso a paso.  
> Crear una máquina virtual Kali Linux y documentar cómo has realizado la instalación paso a paso.”

Yo lo adapto a **Windows 11** como sistema Windows principal (mismo objetivo técnico).

### 3.1 VM Windows 11 en VirtualBox

#### 3.1.1 Configuración de la VM

- Nombre: `Win11-PreInclude`
- Hypervisor: VirtualBox
- Tipo: Microsoft Windows
- Versión: Windows 11 (64-bit)
- RAM asignada: 8 GB
- Procesadores: 4
- Disco virtual: 40 GB, VDI, dinámico
- Red: NAT
- ISO asociada: ISO oficial Windows 11

#### 3.1.2 Instalación paso a paso (resumen)

1. Arranque desde la ISO → pantalla de idioma y edición.  
2. Acepto términos, instalación personalizada, selecciono el disco virtual creado.  
3. Proceso de copia de archivos y reinicios automáticos.  
4. Configuración inicial (zona horaria, usuario `AlumnoInclude`, sin contraseña / con contraseña sencilla).  
5. Llegada al escritorio de Windows 11.

<img width="946" height="559" alt="Screenshot 2026-01-23 214430" src="https://github.com/user-attachments/assets/3855c9a6-2435-4dc6-a50c-6657e7aab6ee" />
<img width="946" height="559" alt="Screenshot 2026-01-23 214449" src="https://github.com/user-attachments/assets/52b9c49a-3b57-4714-b65b-747c97028595" />
<img width="946" height="559" alt="Screenshot 2026-01-23 214506" src="https://github.com/user-attachments/assets/752b0b83-e311-46ce-80b5-3c71be38769f" />
<img width="946" height="559" alt="Screenshot 2026-01-23 214519" src="https://github.com/user-attachments/assets/ca5b7150-e6c3-41b3-858c-fceace83bc4b" />
<img width="1920" height="1080" alt="Screenshot 2026-01-23 214649" src="https://github.com/user-attachments/assets/d6db313e-9a4f-4459-9875-85b0848460b7" />
<img width="1920" height="1080" alt="Screenshot 2026-01-23 214705" src="https://github.com/user-attachments/assets/8ef946e7-1cd7-4c8d-b057-063f7cf556d4" />
<img width="1920" height="1080" alt="Screenshot 2026-01-23 214740" src="https://github.com/user-attachments/assets/f22c3466-e64c-4e0b-a629-54f214879643" />
<img width="1920" height="1080" alt="Screenshot 2026-01-23 232552" src="https://github.com/user-attachments/assets/5d000fbe-eec4-45c9-9b07-8d2b75f73645" />


