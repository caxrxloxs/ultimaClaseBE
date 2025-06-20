API con postgre y ambas van a estar en contenedores distintos y se van a interconectar entre ellos(la API con la BD) para poder comunicarse
y migracion sobre la base de datos de postgree 
ruta con acceso solo si tienes rol de admin y demas van a ser accesibles por cualquier rol
osea se puede entrar a rutas con JWT pero hay rutas que son son accesible con rol de admin


Para poder trabajar con docker necesitamos archivos de docker-compose.yml
# touch docker-compose.yml


# Crear estructura básica
```bash
mkdir api && cd api/
npm init -y                # Inicializar proyecto Node crear archivo package.json
touch .env                 # Variables de entorno
mkdir src                  # Código fuente recursos
mkdir migrations           # Migraciones de base de datos
touch knexfile.js          # Configuración de Knex (para migraciones)
```

## 📦 Dependencias Principales

```bash
npm i express bcryptjs cors pg dotenv jsonwebtoken sequelize knex
```

# Es el "stack estándar" para APIs Node.js con autenticación y base de datos

## 🚀 Express
`express` es el servidor base.
## 🔐 Autenticación Segura
`bcryptjs` + `jsonwebtoken` manejan autenticación segura.
## 🗃️ Base de Datos PostgreSQL
`pg` + `sequelize`/`knex` trabajan con PostgreSQL.
## 🛡️ Seguridad
`dotenv` protege datos sensibles.
## ↔️ Comunicación Backend-Frontend
`cors` comunica backend con frontend.

