
# 🎧 Ecualizador Gráfico por Tercios de Octava con Visualización FFT

Este proyecto es una aplicación interactiva desarrollada en Python que permite cargar archivos de audio `.wav`, aplicar ecualización por bandas de **tercio de octava** y visualizar el resultado en **tiempo real** tanto en el dominio de la frecuencia (FFT) como en el dominio del tiempo.

---

### 🎯 ¿Qué hace este programa?

Es una **aplicación para cargar archivos de audio `.wav`**, aplicarles **filtrado por tercios de octava** mediante faders (controles deslizantes de ganancia en dB), y visualizar:

1. El **espectro de frecuencias** (mediante FFT)
2. La **forma de onda original y filtrada** en el dominio del tiempo

---

### ✅ Funcionalidades principales:

| Funcionalidad                        | Descripción                                                                       |
| ------------------------------------ | --------------------------------------------------------------------------------- |
| 🎚️ **Faders de bandas**             | 32 faders controlan 32 bandas de frecuencia (tercios de octava de 20 Hz a 20 kHz) |
| 📁 **Carga de audio**                | Puedes seleccionar un archivo `.wav` mono o estéreo (usa solo un canal)           |
| 🎛️ **Ecualización en tiempo real**  | Cada vez que mueves un fader, se aplica el cambio y se actualiza la señal         |
| 📊 **Visualización dual**            | Muestra **FFT** (frecuencia) y **forma de onda** (tiempo) original vs filtrada    |
| 🔍 **Filtros digitales Butterworth** | Se usan para separar cada banda antes de aplicar ganancia                         |

---

## 🚀 Características

- Interfaz gráfica con `tkinter`
- Ecualización por **32 bandas** de frecuencia (20 Hz a 20 kHz)
- Controles de ganancia **por banda** de ±30 dB
- Visualización simultánea de:
  - Espectro de frecuencias (FFT logarítmica)
  - Forma de onda original y filtrada
- Filtros digitales Butterworth por banda
- Soporte para archivos `.wav` mono o estéreo (usa un solo canal)

## 🧪 Requisitos

- Python 3.7 o superior
- `numpy`
- `scipy`
- `matplotlib`
- `tkinter` (incluido en Python por defecto)

## 📦 Instalación

Instala las dependencias con pip:

```bash
pip install numpy scipy matplotlib
````

> ⚠️ Nota: `tkinter` viene con Python. Si usas Linux y no lo tienes, instala con:
> `sudo apt install python3-tk`

## 🗂️ Cómo usar

1. Ejecuta el script:

   ```bash
   python ecualizador.py
   ```

2. Haz clic en **"Cargar WAV"** y selecciona un archivo de audio `.wav`

3. Ajusta los faders de frecuencia para modificar la ganancia por banda

4. Observa cómo se actualizan en tiempo real:

   * El gráfico FFT (frecuencia)
   * La forma de onda (tiempo)

## 🎥 Vista previa

![demo](demo.gif)

## 📚 Créditos

* Filtrado por bandas basado en filtros Butterworth
* Interfaz construida con `tkinter`
* Gráficas integradas con `matplotlib`

## ⚖️ Licencia

MIT License

Copyright (c) 2025 Dilan Acosta

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights  
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell  
copies of the Software, and to permit persons to whom the Software is  
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all  
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR  
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,  
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE  
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER  
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,  
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE  
SOFTWARE.


