1. Run emulator with Android Studio
2. Descargar frida server, mira que sea server de aqui: https://github.com/frida/frida/releases
3. Mover el server.jpg a download del sdcard
4. frida-server-15.1.3-android-arm64.xz
5. adb shell "su 0 chmod 755 sdcard/download/server.jpg"
6. adb shell "chmod +x /sdcard/download/server"
7.  Listar las apps instaladas: frida-ps -Uai
