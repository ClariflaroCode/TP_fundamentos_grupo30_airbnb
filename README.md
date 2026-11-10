# Análisis de Airbnb en Buenos Aires · Grupo 30

El notebook `Entrega.ipynb` contiene la limpieza de los datos, los gráficos y las pruebas de las hipótesis del grupo y de la cátedra.

## 1. Preparar la carpeta del proyecto

Necesitás Python 3.12 y conexión a internet para instalar las dependencias y descargar los datos la primera vez. El calendario supera los diez millones de filas, por lo que su análisis puede tardar varios minutos.

Si ya descargaste el proyecto, abrí una terminal en la carpeta que contiene `Entrega.ipynb` y `requirements.txt`, y continuá con el paso 2. Si todavía necesitás descargarlo, podés clonarlo con Git:

```bash
git clone https://github.com/ClariflaroCode/TP_fundamentos_grupo30_airbnb.git
cd TP_fundamentos_grupo30_airbnb
```

## 2. Crear y activar el entorno

En Linux o macOS:
```bash
python3.12 -m venv .venv
source .venv/bin/activate
```

En Windows, desde el Símbolo del sistema (cmd):
```bat
py -3.12 -m venv .venv
.venv\Scripts\activate.bat
```

Con el entorno activo, instalá las dependencias:
```bash
python -m pip install -r requirements.txt
```

## 3. Cargar los datos
La primera sección del notebook busca `listings.csv` (publicaciones) y `calendar.csv` (disponibilidad por fecha) en la misma carpeta que `Entrega.ipynb`. Si falta alguno, intenta descargarlo desde Google Drive y descomprimirlo si corresponde. Si ambos archivos ya están presentes, los reutiliza.

Si la descarga automática falla o Google Drive devuelve una página HTML, descargá los archivos desde los enlaces del proyecto: [publicaciones](https://drive.google.com/file/d/1JMwdMy8mXA8OgIH9O_6LmbxnWJ7h7e3X/view) y [calendario](https://drive.google.com/file/d/1ENXJDLDOoANo7pZgBvTFCRvImVSwXQ1J/view). Si recibís un archivo comprimido, extraé el CSV. Guardalos con los nombres exactos `listings.csv` y `calendar.csv` junto al notebook y volvé a ejecutar la sección de inicialización.

## 4. Ejecutar el análisis

Desde la carpeta del proyecto, con el entorno activo, ejecutá:

```bash
jupyter notebook Entrega.ipynb
```

1. Si el navegador no se abre automáticamente, copiá la dirección local que muestra Jupyter en la terminal.
2. Si Jupyter te pide elegir un kernel, seleccioná **Python 3 (ipykernel)**.
3. Seleccioná **Restart Kernel and Run All Cells** (reiniciar el kernel y ejecutar todas las celdas). El orden importa porque las secciones de análisis reutilizan los datos preparados en las primeras celdas.
4. Esperá a que el kernel quede inactivo y comprobá que aparezcan los resultados y gráficos sin errores de ejecución. Guardá el notebook si querés conservar las nuevas salidas.

Para cerrar Jupyter, volvé a la terminal y presioná **Ctrl+C**. En futuras sesiones alcanza con activar el mismo entorno y repetir el paso 4.
