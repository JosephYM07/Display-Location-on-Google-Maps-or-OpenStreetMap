# Aplicación de Mostrar Ubicación en OpenStreetMap

Esta es una aplicación desarrollada con Ionic y Angular que utiliza Leaflet para mostrar la ubicación actual del dispositivo en un mapa de OpenStreetMap. La aplicación obtiene las coordenadas geográficas mediante Geolocation y muestra la dirección correspondiente utilizando NativeGeocoder. Además, envía las coordenadas a Firebase para su almacenamiento en tiempo real.

## Instalación de Dependencias

Para comenzar, asegúrate de tener Node.js y npm instalados en tu máquina. Luego, sigue estos pasos:

1. **Clonar el Repositorio:**
    
    ```bash
    git clone https://github.com/JosephYM07/Display-Location-on-Google-Maps-or-OpenStreetMap.git
    cd tu-repositorio
    
    ```
    
2. **Instalar Ionic CLI (si no está instalado):**
    
    ```bash
    
    npm install -g @ionic/cli
    
    ```
    
3. **Instalar Dependencias del Proyecto:**
    
    ```bash
    
    npm install
    
    ```
    
    Esto instalará todas las dependencias necesarias, incluyendo Ionic, Angular, Leaflet, Geolocation, NativeGeocoder y Firebase.
    

## Configuración de Firebase

Para que la aplicación funcione correctamente con Firebase, sigue estos pasos:

1. Crea un proyecto en Firebase Console.
2. Configura la autenticación y la base de datos Firestore según sea necesario.
3. Obtén las credenciales de tu proyecto Firebase.

## Configuración de Variables de Entorno

Asegúrate de configurar las variables de entorno necesarias para Firebase. En el archivo `environment.ts` en `src/environments/environment.ts`, agrega las credenciales de tu proyecto Firebase:

```tsx

export const environment = {
  production: false,
  firebaseConfig: {
    apiKey: "TU_API_KEY",
    authDomain: "TU_AUTH_DOMAIN",
    projectId: "TU_PROJECT_ID",
    storageBucket: "TU_STORAGE_BUCKET",
    messagingSenderId: "TU_MESSAGING_SENDER_ID",
    appId: "TU_APP_ID"
  }
};

```

Reemplaza `"TU_API_KEY"`, `"TU_AUTH_DOMAIN"`, `"TU_PROJECT_ID"`, `"TU_STORAGE_BUCKET"`, `"TU_MESSAGING_SENDER_ID"` y `"TU_APP_ID"` con tus propias credenciales de Firebase.

## Ejecutar la Aplicación Localmente

Una vez configuradas las dependencias y Firebase, puedes ejecutar la aplicación localmente:

```bash

ionic serve

```

Esto abrirá la aplicación en tu navegador web predeterminado. Asegúrate de probar la funcionalidad en un dispositivo móvil para ver la geolocalización en acción.

## Estructura del Proyecto

- `src/app/`: Contiene los componentes y servicios principales de la aplicación.
    - `home/`: Componente principal donde se encuentra la lógica de la página principal (`home.page.ts`, `home.page.html`, `home.page.scss`).


