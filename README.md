# ob-angular-spring-deploy

🇪🇸 [Español](#-español) | 🇬🇧 [English](#-english)

---

## 🇪🇸 Español

Aplicación web full-stack con frontend en **Angular** y backend en **Spring Boot**, con autenticación basada en JWT (login / registro) y gestión de un recurso de vehículos ("cars"). Proyecto de práctica desarrollado en el marco de un curso (Open Bootcamp).

### 🚀 Funcionalidades

- 🔐 Registro e inicio de sesión de usuarios (`login`, `register`) con autenticación JWT.
- 🔑 Interceptor HTTP (`auth.interceptor.ts`) que adjunta el token a cada petición.
- 🗄️ Almacenamiento del token de sesión (`token-storage.service.ts`).
- 🚗 Consumo de un recurso de vehículos vía `cars.service.ts`.
- 👋 Endpoint de prueba (`hello.service.ts`).
- 🏠 Vista principal protegida (`home`).

### 🔧 Tecnologías

- **Angular 12** (Angular CLI 12.1.3)
- TypeScript
- RxJS
- Karma / Jasmine (pruebas unitarias)
- Backend: **Spring Boot** (API REST consumida por este frontend)

### 🏗️ Estructura del proyecto

```
src/app/
├── _helpers/
│   └── auth.interceptor.ts     # Adjunta el JWT a las peticiones HTTP
├── _services/
│   ├── auth.service.ts         # Login / registro
│   ├── cars.service.ts         # CRUD de vehículos
│   ├── hello.service.ts        # Endpoint de prueba
│   └── token-storage.service.ts # Guardado del token en el navegador
├── home/          # Vista principal (protegida)
├── login/         # Formulario de inicio de sesión
├── register/      # Formulario de registro
├── app-routing.module.ts
└── app.module.ts
```

### 🚀 Cómo ejecutar

```bash
npm install
npm start        # equivalente a: ng serve
```

La aplicación queda disponible en `http://localhost:4200/`. Requiere que el backend de Spring Boot esté corriendo y accesible según la configuración de `src/environments/environment.ts`.

### 🧪 Pruebas

```bash
npm test          # ng test (Karma)
```

### 📄 Licencia

Proyecto académico / de práctica.

---

## 🇬🇧 English

A full-stack web application with an **Angular** frontend and a **Spring Boot** backend, featuring JWT-based authentication (login / register) and management of a vehicle ("cars") resource. A hands-on practice project built as part of a bootcamp course (Open Bootcamp).

### 🚀 Features

- 🔐 User registration and login (`login`, `register`) with JWT authentication.
- 🔑 HTTP interceptor (`auth.interceptor.ts`) that attaches the token to every request.
- 🗄️ Session token storage (`token-storage.service.ts`).
- 🚗 Consumes a vehicle ("cars") resource via `cars.service.ts`.
- 👋 Test endpoint (`hello.service.ts`).
- 🏠 Protected home view (`home`).

### 🔧 Technologies

- **Angular 12** (Angular CLI 12.1.3)
- TypeScript
- RxJS
- Karma / Jasmine (unit testing)
- Backend: **Spring Boot** (REST API consumed by this frontend)

### 🏗️ Project Structure

```
src/app/
├── _helpers/
│   └── auth.interceptor.ts     # Attaches the JWT to HTTP requests
├── _services/
│   ├── auth.service.ts         # Login / registration
│   ├── cars.service.ts         # Vehicle CRUD
│   ├── hello.service.ts        # Test endpoint
│   └── token-storage.service.ts # Stores the token in the browser
├── home/          # Main (protected) view
├── login/         # Login form
├── register/      # Registration form
├── app-routing.module.ts
└── app.module.ts
```

### 🚀 How to Run

```bash
npm install
npm start        # equivalent to: ng serve
```

The app will be available at `http://localhost:4200/`. It requires the Spring Boot backend to be running and reachable according to the settings in `src/environments/environment.ts`.

### 🧪 Testing

```bash
npm test          # ng test (Karma)
```

### 📄 License

Academic / practice project.
