# 🎧 Ecualizador Gráfico por Tercios de Octava con Visualización FFT

Este proyecto es una aplicación interactiva desarrollada en Python que permite cargar archivos de audio `.wav`, aplicar ecualización por bandas de **tercio de octava** y visualizar el resultado en **tiempo real** tanto en el dominio de la frecuencia (FFT) como en el dominio del tiempo.

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
