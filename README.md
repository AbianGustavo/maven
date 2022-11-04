# Instalación de Maven en el SO

###### Nombre del alumno:
Abián Castañeda Méndez

## Indice

- **[Introducción](#punto0)**
- **[1. Instalar Apache Maven](#punto1)**
  - **[1.1 Instalar Apache Maven con apt](#punto1.1)**
  - **[1.2 Instalar una versión concreta de Apache Maven](#punto1.2)**
  - **[1.3 Establecer variables de entorno](#punto1.3)**
  - **[1.4 Verificar la instalación](#punto1.4)**

### Introducción <a name="punto0"></a>

Apache Maven es una herramienta de gestión y comprensión de proyectos de código abierto que se utiliza principalmente para proyectos Java. Maven usa un modelo de objetos de proyecto (POM), que es esencialmente un archivo XML que contiene información del proyecto, detalles de configuración, dependencias del proyecto, etc.

### 1. Instalar Apache Maven <a name="punto1"></a>

#### 1.1 Instalar Apache Maven con apt <a name="punto1.1"></a>

Instalaremos Maven en Ubuntu usando apt pero antes de ello actualizaremos los paquetes.

<img src="img\1.png">

Después de haber instalado lo anterior, verificaremos la instalación.

<img src="img\2.png">

#### 1.2 Instalar una versión concreta de Apache Maven <a name="punto1.2"></a>

Primero de todo, descargaremos Apache Maven en el directorio **/tmp**.

<img src="img\3.png">

Una vez que se complete la descarga, extraeremos el archivo en el directorio **/opt**.

<img src="img\4.png">

Para tener más control sobre las versiones y actualizaciones de Maven, crearemos un enlace simbólico que apunte al directorio de instalación de Maven.

<img src="img\5.png">

#### 1.3 Establecer variables de entorno <a name="punto1.3"></a>

A continuación, necesitaremos establecer las variables de entorno. Para hacer esto, abriremos nuestro editor de texto y crearemos un nuevo archivo llamado **maven.sh** en el directorio **/etc/profile.d/**. Ahí pegaremos el código de la siguiente imagen:

<img src="img\6.png">

Después de haber guardado y cerrado el archivo, haremos que el script sea ejecutable con chmod para finalmente, cargar las variables de entorno usando el comando de source.

<img src="img\7.png">

#### 1.4 Verificar la instalación <a name="punto1.4"></a>

Verificaremos que Maven está instalado de la siguiente manera:

<img src="img\8.png">
