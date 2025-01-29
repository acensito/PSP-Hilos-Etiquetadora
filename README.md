# 🏭 Enunciado del problema  

En una fábrica, existen varias **máquinas etiquetadoras** 🏷️ (por defecto **5**) y una **máquina productora de etiquetas** 🎟️.  
Las etiquetas se almacenan en un **depósito** 📦, del cual las máquinas etiquetadoras las toman **de una en una**.  
La máquina productora repone etiquetas en cantidades determinadas (por defecto, **de 10 en 10**).  

## ⚙️ Funcionamiento  

- Cada **máquina etiquetadora** (**consumidor**) 🏷️ necesita **500 ms** ⏳ para colocar una etiqueta.  
- El **depósito** 📦 de etiquetas comienza con **100 etiquetas**.  
- La **máquina productora** 🎟️ genera etiquetas en una cantidad determinada (**por defecto, 10**) cada vez que el depósito baja de **10 etiquetas**.  
- **Solo una máquina** puede tomar una etiqueta a la vez 🚫 (no pueden tomar etiquetas simultáneamente).  
- Cada máquina etiquetadora **empleará 100 etiquetas** antes de detenerse.  
- Cuando todas las máquinas hayan consumido **100 etiquetas cada una**, la aplicación **finalizará** 🛑.  

## 🖥️ Implementación  

Se deberán crear las siguientes clases:  
- **`Maquina`** 🏷️: Representa una máquina etiquetadora (**consumidor**).  
- **`Productor`** 🎟️: Representa la máquina que genera las etiquetas.  

Ambas clases trabajarán con **hilos** 🧵 y utilizarán **monitores** (`synchronized`) 🔒 para garantizar la sincronización.  

Al sacar una etiqueta, se deberá **visualizar cuántas etiquetas ha consumido** cada máquina 🔢.  

## ⚙️ Parámetros opcionales  

Opcionalmente, la aplicación permitirá configurar:  
1. **Número de máquinas etiquetadoras** 🏷️:  
   - [ ] Si no se especifica, se considerará el valor por defecto de **5**.  
2. **Cantidad de etiquetas que se añaden al depósito** 📦 cuando el nivel de etiquetas sea menor a **10**:  
   - [ ] Si no se especifica, se considerará el valor por defecto de **10 etiquetas**.  
