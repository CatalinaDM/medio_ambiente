
# Proyecto Web Medio Ambiente – Flask

Este repositorio contiene una aplicación web desarrollada con Flask, enfocada en la concientización ambiental mediante diferentes secciones relacionadas con el medio ambiente, sistemas naturales, el futuro del planeta y las 3R: Reducir, Reutilizar y Reciclar.

---

## Evidencia del proyecto

🎥 Video de demostración:  
https://drive.google.com/file/d/1DSZOG1NbILY3_DlhmXC83WO8KARbUIQ7/view
<img width="1654" height="793" alt="image" src="https://github.com/user-attachments/assets/0f62557a-c3d6-4243-aeb9-92e8263fc9f5" />

<img width="1920" height="957" alt="image" src="https://github.com/user-attachments/assets/782062bf-f83b-4b72-988a-efbe1e200ea6" />

<img width="1920" height="1016" alt="image" src="https://github.com/user-attachments/assets/ad8bb6b8-4a0d-40ae-b7a2-ad47e8c08e60" />

<img width="1920" height="891" alt="image" src="https://github.com/user-attachments/assets/14b1d019-77a8-44f2-9488-4d7104d4a54b" />

<img width="1910" height="911" alt="image" src="https://github.com/user-attachments/assets/bd9530f1-9c8f-4000-9541-c8310353fa7d" />

<img width="1920" height="953" alt="image" src="https://github.com/user-attachments/assets/00c5de73-8ddc-4622-b954-a72e8d459926" />

<img width="1920" height="886" alt="image" src="https://github.com/user-attachments/assets/107d5a26-fc71-4b63-a12f-7fbe71e5016b" />
<img width="1918" height="980" alt="image" src="https://github.com/user-attachments/assets/b189ad3d-60ff-41b8-996f-57f004c83fa3" />

## 1. Creación del proyecto Flask desde cero

### Crear carpeta del proyecto
```bash
mkdir web_medio_ambiente
cd web_medio_ambiente

Este paso crea el entorno de desarrollo e instala Flask como framework principal.
```
### Crear entorno virtual
```bash
python -m venv venv
```
### Activar entorno virtual (Windows)
```bash
venv\Scripts\activate
```
### Instalar Flask
```bash
pip install flask
```
### Descripción:
Este paso crea el entorno de desarrollo e instala Flask como framework principal.

## 2. Estructura del proyecto
```bash
La estructura recomendada es la siguiente:

web_medio_ambiente/
│
├── app.py
│
├── templates/
│   ├── base.html
│   ├── index.html
│   ├── sistema.html
│   ├── futuro.html
│   └── tres_r.html
│
├── static/
│   └── images/
│       ├── ambiente.jpg
│       ├── sistema.jpg
│       ├── futuro.jpg
│       └── reciclaje.jpg
│
└── venv/

```
###  Convenciones de Flask

La carpeta templates/ contiene las plantillas HTML.

La carpeta static/ contiene imágenes, CSS y archivos JavaScript.

## 3. Backend Flask (app.py)
```bash
Ejemplo base del backend:

from flask import Flask, render_template

app = Flask(__name__)

@app.route('/')
def index():
    return render_template('index.html')

@app.route('/sistema')
def sistema():
    return render_template('sistema.html')

@app.route('/futuro')
def futuro():
    return render_template('futuro.html')

@app.route('/tres_r')
def tres_r():
    return render_template('tres_r.html')

if __name__ == '__main__':
    app.run(debug=True)


Este archivo administra las rutas principales del sitio y enlaza cada una con su respectiva plantilla.
```
## 4. Plantilla base con Bootstrap y migas de pan

El archivo base.html funciona como una plantilla general para todas las páginas.
Incluye encabezado, navegación, pie de página, recursos de Bootstrap y componentes reutilizables.

## 5. Página principal

El archivo index.html actúa como la página principal del proyecto.
Debe incluir contenido visual e informativo relacionado con el cuidado del medio ambiente.

## 6. Futuro del planeta

El archivo futuro.html explica escenarios futuros del planeta y acciones que pueden reducir el impacto ambiental.

## 7. Ejecución de la aplicación

### Activar entorno virtual
```bash
venv\Scripts\activate
```
## Ejecutar Flask
```bash
python app.py
```
## Abrir en navegador
```bash
http://127.0.0.1:5000
```
## Descripción:
Estos comandos inician el servidor local para visualizar la aplicación.
