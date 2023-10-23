# Tarea 1: REST

Haga un fork de este repositorio.

# Preparación

En ReplIT cree un nuevo REPL a partir del repositorio creado con el fork (use el botón `import from GitHub`).

IMPORTANTE: este proceso podría crear un archivo `replit.nix`, asegurese de eliminar ese archivo.

Ingrese a ElephantSQL: https://www.elephantsql.com (ingrese usando GitHub).

Cree una instancia de base de datos.

Ejecute las queries que están en el archivo [`database.sql`](database.sql).

Obtenga el string de conexión desde ElephantSQL (tal como mostró el profesor).

Ahora cree los siguientes SECRETS en Replit:

  - PORT: 3000
  - CONNECTION_URL: coloque aca la url de conexión obgenida de ElephantSQL
  - JWT_SECRET: coloque un valor aleatorio


Ejecute ReplIT presionando el botón `RUN`.

