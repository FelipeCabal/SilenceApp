# SilenceApp

Una aplicación Android desarrollada con Jetpack Compose y Kotlin.

## 📋 Requisitos Previos

### Android Studio
- **Android Studio Koala Feature Drop** (2024.1.2) o superior
- **Versión recomendada**: Android Studio Ladybug (2024.2.1) o más reciente

### Tecnologías y Versiones

#### Sistema Operativo Soportado
- **Android API Level**: 26 (Android 8.0) como mínimo
- **Target SDK**: API Level 36 (Android 15)

#### Lenguajes de Programación
- **Kotlin**: 2.0.21
- **Java**: Compatible con Java 11

#### Framework y Herramientas de Desarrollo
- **Android Gradle Plugin (AGP)**: 8.13.0
- **Gradle Wrapper**: Incluido en el proyecto
- **Jetpack Compose**: 2024.09.00 (BOM)

## 🛠️ Tecnologías Utilizadas

### Framework Principal
- **Jetpack Compose**: Framework moderno para crear interfaces de usuario nativas de Android
- **Material Design 3**: Sistema de diseño de Google para interfaces consistentes

### Librerías Core
- **AndroidX Core KTX**: 1.17.0 - Extensiones de Kotlin para Android
- **Lifecycle Runtime KTX**: 2.6.1 - Manejo del ciclo de vida de componentes
- **Activity Compose**: 1.8.0 - Integración de Activity con Compose

### Testing
- **JUnit**: 4.13.2 - Framework de testing unitario
- **AndroidX Test JUnit**: 1.3.0 - Testing para Android
- **Espresso Core**: 3.7.0 - Testing de UI
- **Compose UI Test**: Testing específico para Compose

## 🚀 Configuración del Entorno de Desarrollo

### 1. Instalación de Android Studio

1. Descarga Android Studio desde [developer.android.com](https://developer.android.com/studio)
2. Instala Android Studio siguiendo las instrucciones para tu sistema operativo
3. Durante la instalación, asegúrate de incluir:
   - Android SDK
   - Android SDK Platform-Tools
   - Android Virtual Device (AVD)

### 2. Configuración del SDK

1. Abre Android Studio
2. Ve a **File > Settings** (o **Android Studio > Preferences** en macOS)
3. Navega a **Appearance & Behavior > System Settings > Android SDK**
4. En la pestaña **SDK Platforms**, asegúrate de tener instalado:
   - Android API 36 (Android 15.0)
   - Android API 26 (Android 8.0) como mínimo
5. En la pestaña **SDK Tools**, verifica que tengas:
   - Android SDK Build-Tools
   - Android Emulator
   - Android SDK Platform-Tools

### 3. Configuración de Java

El proyecto requiere **Java 11**. Android Studio generalmente incluye una JDK compatible, pero puedes verificar:

1. Ve a **File > Project Structure**
2. En **SDK Location**, verifica que la **JDK Location** apunte a Java 11

## 📱 Configuración del Proyecto

### Clonar el Repositorio

```bash
git clone [URL_DEL_REPOSITORIO]
cd SilenceApp
```

### Abrir en Android Studio

1. Abre Android Studio
2. Selecciona **File > Open**
3. Navega hasta la carpeta del proyecto y selecciónala
4. Android Studio sincronizará automáticamente el proyecto con Gradle

### Sincronización de Gradle

Si es necesario sincronizar manualmente:
1. Haz clic en **Sync Now** en la barra de notificaciones
2. O usa **File > Sync Project with Gradle Files**

## 🏃‍♂️ Ejecutar la Aplicación

### En un Dispositivo Virtual (Emulador)

1. Ve a **Tools > AVD Manager**
2. Crea un nuevo dispositivo virtual o usa uno existente
3. Asegúrate de que tenga API Level 26 o superior
4. Haz clic en el botón **Run** (▶️) o presiona `Shift + F10`

### En un Dispositivo Físico

1. Habilita las **Opciones de Desarrollador** en tu dispositivo Android
2. Activa la **Depuración USB**
3. Conecta tu dispositivo via USB
4. Selecciona tu dispositivo en la lista de dispositivos disponibles
5. Haz clic en **Run**

## 🧪 Ejecutar Tests

### Tests Unitarios
```bash
./gradlew test
```

### Tests de Instrumentación (Android)
```bash
./gradlew connectedAndroidTest
```

## 📦 Generar APK

### Debug APK
```bash
./gradlew assembleDebug
```

### Release APK
```bash
./gradlew assembleRelease
```

Los archivos APK se generarán en: `app/build/outputs/apk/`

## 🔧 Configuración Adicional

### Variables de Entorno
- **JAVA_HOME**: Debe apuntar a Java 11
- **ANDROID_HOME**: Debe apuntar al directorio del Android SDK

### Memoria de Gradle
El proyecto está configurado para usar 2GB de memoria heap para Gradle. Si experimentas problemas de memoria, puedes ajustar en `gradle.properties`:

```properties
org.gradle.jvmargs=-Xmx2048m -Dfile.encoding=UTF-8
```

## 📋 Estructura del Proyecto

```
SilenceApp/
├── app/
│   ├── src/main/
│   │   ├── java/           # Código fuente Kotlin
│   │   ├── res/            # Recursos (layouts, strings, etc.)
│   │   └── AndroidManifest.xml
│   └── build.gradle.kts    # Configuración del módulo app
├── gradle/
│   └── libs.versions.toml  # Catálogo de versiones de dependencias
├── build.gradle.kts        # Configuración del proyecto raíz
└── README.md
```

## 🤝 Contribución

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📄 Licencia

[Especificar la licencia del proyecto]

## 📞 Contacto

[Información de contacto del desarrollador]

---

**Nota**: Este proyecto utiliza las últimas tecnologías de desarrollo Android. Asegúrate de mantener Android Studio actualizado para una mejor experiencia de desarrollo.