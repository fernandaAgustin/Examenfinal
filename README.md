# 🧑‍💼 Proyecto de React: Sistema de Gestión de Usuarios

Esta es una aplicación web desarrollada en **React.js** que permite a los usuarios registrarse, iniciar sesión, editar su información y eliminar su cuenta. La lista de usuarios está paginada y organizada en un diseño limpio de formularios. La app se conecta a una API backend (por ejemplo, Flask + PostgreSQL) mediante peticiones HTTP.

---

## 🧱 Estructura del Proyecto
/src │ ├── /components │ ├── LoginForm.jsx │ ├── UserCreateForm.jsx │ ├── UserEditForm.jsx │ └── UsersList.jsx │ ├── /hooks │ └── useUsers.js │ ├── /services │ └── UserService.js 
/public └── index.html

## ⚙️ Instalación del Proyecto
### 1. Requisitos previos

- Node.js y npm instalados ([descargar aquí](https://nodejs.org/))
- Navegador moderno (Chrome, Firefox, etc.)

### 2. Crear y preparar el proyecto

```bash
npx create-react-app exam_react
cd exam_react
npm install react-icons
'''

### Detalles de los componentes
###1. LoginForm.jsx


Formulario de inicio de sesión con validación de campos. Usa íconos (react-icons) y maneja errores en pantalla. Ejecuta onLogin para validar credenciales en el backend.

### 2. UserCreateForm.jsx
Formulario de registro de nuevos usuarios. Incluye verificación si el correo ya está en uso antes de enviar la solicitud POST a la API.

### 3. UsersList.jsx
Lista paginada de usuarios que consume la API (GET /users). Incluye botones para editar y eliminar usuarios.

### 4. UserEditForm.jsx
Formulario que permite editar la información de un usuario existente. Utiliza una ruta PUT para enviar los cambios al backend.

### Detalles de hook
Este custom hook se encarga de toda la lógica relacionada con usuarios:

Obtener todos los usuarios

Crear nuevos

Editar existentes

Eliminar usuarios

Login de usuario

Verificación de email

#Correr React dentro de local:
npm start
