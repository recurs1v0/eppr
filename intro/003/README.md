# EPPR / INTRO / 003  
# > RaspberryPi4 Primer Inicio - NOOBS Configurando tu PC Raspbian (FULL) para las clases virtuales EPPR

<a href="http://www.youtube.com/watch?feature=player_embedded&v=xNs6drvAk_A
" target="_blank"><img src="http://img.youtube.com/vi/xNs6drvAk_A/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="80%" height="auto" border="10" /></a>

# Necesitas:

1. RaspberryPi4
2. Tarjeta microSD de 32Gb con EPPR QuickBoot o con Noobs
3. Teclado con Mouse USB (No Bluetooth) <a href="https://amzn.to/2RuZ60g">Amazon</a>
4. Cable HDMI de RPI
5. Pantalla con entrada HDMI, puede ser una Tv

# Instalación Automática (recomendado):

Una tarjeta de 32Gb con EPPR QuickBoot significa que todo está listo para iniciar.

Para obtener una tarjeta pre-instalada con EPPR QuickBoot visita <a href="https://ez.link/eppr">https://ez.link/eppr</a>

> Este método te va a ahorrar un par de horas en tiempo de descarga en comparación a la Instalación Manual.

Lo único que tienes que hacer es colocar la memoria microSd como se muestra en el video.

> Lee las siguientes instrucciones por completo antes de continuar.

Conecta los cables en el siguiente orden:

1. HDMI de RPI a Pantalla
2. USB de Teclado y Mouse
3. Conecta el cable de carga primero con el RPI, pero sin conectarlo a la electricidad.
4. Finalmente y solo hasta que conectaste todo lo anterior, conecta tu RPI a la electricidad.

A continuación deberás ver un tu pantalla que tu RPI esta iniciando.

> La primera vez que inicies tu RPI tardará al menos 2 minutos, pero después tardará cerca de 20 segundos.

Cuando sea momento, ingresa la siguiente información:

User
```
eppr
```
Password
```
rpi4
```

Recuerda cambiar tu contraseña tan pronto sea posible ya que todos los RPI4 con EPPR QuickBoot tienen la misma contraseña al nacer.

Para cambiar tu contraseña, copia y pega el siguiente código en Terminal
```
passwd
```

Ahora ingresa una contraseña que puedas recordar, antes de terminar tendrás que volver a ingresar la nueva contraseña para verificar que no tengas algún error.

Listo, puedes marcar esta clase como completada.

# Instalación Manual:

Si estás leyendo esta sección es porque decidiste iniciar tu RPI4 con Noobs.

Lee las siguientes instrucciones por completo antes de continuar.

Conecta los cables en el siguiente orden:

1. HDMI de RPI a Pantalla.
2. USB de Teclado y Mouse.
3. Conecta el cable de carga primero con el RPI, pero sin conectarlo a la electricidad.
4. Finalmente y solo hasta que conectaste todo lo anterior, conecta tu RPI a la electricidad.

A continuación deberás ver en tu pantalla que tu RPI esta iniciando.

La primera vez que inicies tu RPI abriras un programa llamado Noobs.
Este programa te ayudará a instalar y configurar tu RPI4 en segundos.

Al iniciar, selecciona Raspian Buster FULL

Cuando sea momento, ingresa la siguiente información

User
```
pi
```
Password
```
raspberry
```

Recuerda cambiar tu contraseña tan pronto sea posible ya que todos los RPI4 instalados mediante NOOBS tienen la misma contraseña al nacer.

Para cambiar tu contraseña, copia y pega el siguiente código en Terminal
```
passwd
```

Ahora ingresa una contraseña que puedas recordar, antes de terminar tendrás que volver a ingresar la nueva contraseña para verificar que no tengas algún error.

Aún no terminamos, ya tenemos una PC funcional, pero necesitamos instalar la mayoría de los programas que utilizaremos en la Escuela, sin embargo para faclitar este paso y reducir errores, hemos creado una línea de comando para automatizar la configuración inicial de tu RPI4 con EPPR.

Copia y pega este código en Terminal
```
curl -sSL https://get.recurs1v0.com | sh
```
Esto instalará los programas necesarios para las clases de EPPR y además realizará lo siguiente:

1. Actualizar EEPROM Bootloader de RPI4
2. Configurar el RPI4 en modo de bajo consumo de energía
3. Configurar el puerto USB0 como un dispositivo Ethernet USB
4. Habilitar el inicio por USB0 y permitir conexión SSH con RPI4


# Para Apagar tu RPI4 de forma segura:

Como cualquier computadora, es necesario apagar la computadora antes de desconectarla de la electricidad.

Al no hacer esto, es posible que tu RPI4 se dañe.

Por lo tanto puedes apagar tu RPI4 desde tu pantalla, pero si por alguna razón deseas hacerlo desde Terminal recuerda el siguiente comando

Copia y pega lo siguiente en Terminal
```
sudo shutdown -h now
```
