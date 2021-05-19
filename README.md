# Frida-Tutorial
Tutorial para el uso de Frida

## Explicación

Este repositorio pretende ayudar a todos aquellos programadores que desean utilizar el paquete de herramientas de Frida, vitaminado con el uso de comandos para la gestión de los emuladores mediante ADB.

La intención es desarrollar el tutorial con los pasos naturales sobre el proceso al completo.

## Requisitos

Este manual requiere contar con Python instalado y Android Studio.

## Manual

## 1. Instalación de Frida
Ejecutamos en consola el comando "pip install frida-tools".

## 2. Automatización de emulador
Para la apertura del emulador de Android Studio vamos a utilizar "subprocess" de Python, definiendo el string identificativo del emulador Android.

  subprocess.Popen(["export ANDROID_SDK=$HOME/Library/Android/sdk && export PATH=$ANDROID_SDK/emulator:$ANDROID_SDK/tools:$PATH && emulator @Pixel_3a_API_30_x86"],shell=True)

time.sleep(70)


subprocess.Popen(["adb shell monkey -p com.car2go -c android.intent.category.LAUNCHER 1"],shell=True)
