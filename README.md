
# Proyecto Web Medio Ambiente – Flask

Este repositorio contiene una aplicación web desarrollada con Flask, enfocada en la concientización ambiental mediante diferentes secciones relacionadas con el medio ambiente, sistemas naturales, el futuro del planeta y las 3R: Reducir, Reutilizar y Reciclar.

---

## Evidencia del proyecto

🎥 Video de demostración:  
https://drive.google.com/file/d/1DSZOG1NbILY3_DlhmXC83WO8KARbUIQ7/view

<img width="1920" height="1022" alt="image" src="https://github.com/user-attachments/assets/675639ad-e579-4d18-b28b-0a44dd3bafe8" />

<img width="1920" height="1022" alt="image" src="https://github.com/user-attachments/assets/675639ad-e579-4d18-b28b-0a44dd3bafe8" />
<img width="1920" height="1032" alt="image" src="https://github.com/user-attachments/assets/83fc5c41-8341-4947-8340-f77cebc1f964" />
<img width="1920" height="961" alt="image" src="https://github.com/user-attachments/assets/78de0be4-8153-4a42-afb9-20d4fe760ddd" />
<img width="1920" height="933" alt="image" src="https://github.com/user-attachments/assets/ba77a791-e2f3-4454-b376-4101ba6eeeb7" />
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/d26595db-d8c6-4121-aafb-9675f4b8166d" />
<img width="1920" height="957" alt="image" src="https://github.com/user-attachments/assets/97023415-7f5d-4cca-bd65-76994f2760c5" />
<img width="1920" height="902" alt="image" src="https://github.com/user-attachments/assets/9bf041dd-351d-4119-8843-1adec1758570" />


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