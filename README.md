# DiceRoller — Axel Adrian Gaviña Gonzalez

Adaptación del proyecto oficial del codelab de Android Developers a dos dados independientes.

## Base del ejercicio

- [Tutorial de Jetpack Compose](https://developer.android.com/codelabs/basic-android-kotlin-compose-build-a-dice-roller-app?hl=es-419)
- [Código base de Google](https://github.com/google-developer-training/basic-android-kotlin-compose-training-dice-roller)

Se conservan Kotlin, Jetpack Compose, DiceRollerApp(), DiceWithButtonAndImage(),
el tema y las seis imágenes originales. El código original mantiene su licencia Apache 2.0.

## Cambios solicitados

1. Se muestran dos elementos Image en una Row.
2. Cada imagen tiene un estado propio, conservado con rememberSaveable.
3. El botón llama dos veces a private fun getRandomDiceImage(): Int.
4. La función elige un número de 1 a 6 y devuelve R.drawable.dice_1 hasta dice_6.

Los dados pueden coincidir. Independencia no significa que deban ser distintos.

Archivo modificado: app/src/main/java/com/example/diceroller/MainActivity.kt.
También se tradujo el botón y se añadieron descripciones accesibles en strings.xml.

## Abrir y comprobar

1. Abrir esta carpeta desde File > Open en Android Studio.
2. Usar JDK 17 e instalar Android SDK Platform 35 si se solicita.
3. Sincronizar Gradle y ejecutar app en Android 7.0 (API 24) o posterior.
4. Pulsar «Lanzar dados» varias veces y comprobar los dos resultados.
5. Girar el dispositivo: los resultados se conservan.

Se verificaron los XML, los seis recursos y las dos llamadas independientes.
La compilación y ejecución siguen pendientes porque el entorno de preparación
no tiene JDK ni Android SDK instalados.

## Versionado

El repositorio local contiene un commit con la base oficial y otro con el ajuste.
Destino de la entrega: https://github.com/Axel421-yn/DiceRollerAxelAdrianGavi-aGonzalez
La publicación remota debe verificarse antes de entregar el enlace.
