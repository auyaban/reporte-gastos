# Email Transaction Extractor

Este script en Python se conecta a tu cuenta de correo electrónico, filtra correos bancarios que contienen transacciones de tarjeta de crédito, y extrae la fecha, monto y lugar de cada compra. Los datos se guardan en un archivo CSV, facilitando el control de gastos mensuales de forma automática y organizada.

## Características

- Conexión automática al servidor de correo utilizando IMAP.
- Filtrado de correos electrónicos que contienen transacciones de tarjetas de crédito específicas.
- Extracción de detalles de transacciones como fecha, monto y lugar de compra.
- Generación de un archivo CSV con los datos extraídos para facilitar la gestión de gastos.

## Requisitos

- Python 3.7 o superior
- Acceso a una cuenta de correo electrónico con IMAP habilitado
- Librerías de Python:
  - `imaplib`
  - `email`
  - `datetime`
  - `pytz`
  - `chardet`
  - `quopri`
  - `bs4` (BeautifulSoup)
  - `re`
  - `csv`
  - `tqdm`

## Instalación

1. **Clona el repositorio:**

    ```bash
    git clone https://github.com/tuusuario/email-transaction-extractor.git
    cd email-transaction-extractor
    ```

2. **Instala las dependencias necesarias:**

    Ejecuta el siguiente comando para instalar las dependencias usando pip:

    ```bash
    pip install -r requirements.txt
    ```

    Si no tienes un archivo `requirements.txt`, crea uno con el siguiente contenido:

    ```text
    pytz
    chardet
    beautifulsoup4
    tqdm
    ```

3. **Configura tus credenciales de correo:**

    Asegúrate de que tu cuenta de correo esté configurada para permitir acceso IMAP y que tengas las credenciales necesarias configuradas en tus variables de entorno:

    - `EMAIL`: tu dirección de correo electrónico.
    - `PASSWORD`: tu contraseña de correo electrónico.

    En Windows, puedes configurarlo en la terminal con:

    ```bash
    set EMAIL=tu_email@gmail.com
    set PASSWORD=tu_contraseña
    ```

    En macOS/Linux:

    ```bash
    export EMAIL=tu_email@gmail.com
    export PASSWORD=tu_contraseña
    ```

## Uso

1. **Ejecuta el script:**

    Ejecuta el script principal para iniciar la extracción y análisis de los correos electrónicos:

    ```bash
    python email_transaction_extractor.py
    ```

2. **Revisa el archivo CSV generado:**

    Después de que el script haya terminado, encontrarás un archivo `transacciones.csv` en el directorio del proyecto con todas las transacciones extraídas.

## Contribución

¡Las contribuciones son bienvenidas! Siéntete libre de abrir issues y pull requests para mejorar el script.

## Licencia

Este proyecto está bajo la Licencia MIT. Consulta el archivo `LICENSE` para más detalles.

## Contacto

Para preguntas o comentarios, contacta a [tu_email@dominio.com](mailto:tu_email@dominio.com).

