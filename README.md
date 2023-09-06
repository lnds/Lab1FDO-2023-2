# Tarea 1 REST

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


Use YARC para crear un usuario

# Desafío

Este programa usa el méotodo OPTIONS para todos los endpoints. Debe reemplazarlos por los métodos que corresponden.

Ejemplo, a partir de la linea 85 tenemos este código en el archivo `index.js`:

```javascript
 // verificar usuario
app.options("/login", async (req, res) => {
  // #swagger.description = 'Endpoint para obtener un token de sesión para el usuario'
```

Debe quedar así:

```javascript
 // verificar usuario
app.post("/login", async (req, res) => {
  // #swagger.description = 'Endpoint para obtener un token de sesión para el usuario'
```

En la linea 116 tenemos este código:

```javascript
// List all users
app.options("/users", async (req, res) => {
  // #swagger.description = 'Endpoint para listar todos los usuarios registrados en el sistema'
```

Debe quedar así:

```javascript
// List all users
app.get("/users", async (req, res) => {
  // #swagger.description = 'Endpoint para listar todos los usuarios registrados en el sistema'
```

Haga estas modificaciones y las que corresponden en las lineas: 170, 186, 201, 217 y 235. 

Debe usar los métodos `post`, `get`, `put`, `delete` según corresponda.

Cuando haya realizado las modificaciones pruébelas con YARC y mande un Pull Request con su respuesta.




