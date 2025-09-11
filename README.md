<div align="center">
  <img src="https://raw.githubusercontent.com/bottlesdevs/Bottles/main/data/icons/hicolor/scalable/apps/com.usebottles.bottles.svg" width="64">
  <h1 align="center">Bottles</h1>
  <p align="center">¡¡¡Abre facilmente programas de windows usando Bottles!!!</p>
</div>

### ¿Como instalar Bottles en Void Linux?<br/><br/></b>
```
sudo xbps-install -Sy libunwind
sudo xbps-install -S wget cabextract
sudo xbps-install -S gtksourceview5
sudo xbps-install -S libportal libportal-gtk3 libportal-gtk4
 sudo xbps-install -S fluidsynth
pip install --break-system-packages pyFluidSynth==1.3.1
 sudo xbps-install -f python3-yaml
wget https://github.com/franckey02/bottles-Void-version/releases/download/51.24.26/bottles-51.24.26_1.x86_64.xbps
xbps-rindex -a bottles-2022.12.14.1_6.x86_64.xbps
sudo xbps-install -R $PWD bottles-2022.12.14.1_6
sudo pip3 install --break-system-packages pycurl icoextract fvs patool PyYAML requests markdown mutagen pycryptodomex websockets brotli pathvalidate
wget https://gitlab.com/TheEvilSkeleton/vkbasalt-cli/-/archive/v3.1.1/vkbasalt-cli-v3.1.1.tar.bz2
tar xvfa vkbasalt-cli-v3.1.1.tar.bz2
cd vkbasalt-cli-v3.1.1
python setup.py install --user
cd ..
sudo glib-compile-schemas /usr/share/glib-2.0/schemas/ 
```

<div align="center">
  <a href="https://hosted.weblate.org/engage/bottles">
    <img src="https://hosted.weblate.org/widgets/bottles/-/bottles/svg-badge.svg" />
  </a>
  <a href="https://www.codefactor.io/repository/github/bottlesdevs/bottles/overview/main">
    <img src="https://www.codefactor.io/repository/github/bottlesdevs/bottles/badge/main" />
  </a>
  <a href="https://github.com/bottlesdevs/Bottles/blob/main/LICENSE">
    <img src="https://img.shields.io/badge/License-GPL--3.0-blue.svg">
  </a>
  <a href="https://github.com/bottlesdevs/Bottles/actions">
    <img src="https://github.com/bottlesdevs/Bottles/workflows/Build%20release%20packages/badge.svg">
  </a>
  <br>
  <a href="https://stopthemingmy.app" title="Please do not theme this app">
    <img src="https://stopthemingmy.app/badge.svg">
  </a>

  <hr />

  <a href="https://docs.usebottles.com">Documentation</a> ·
  <a href="https://forums.usebottles.com">Forums</a> · 
  <a href="https://t.me/usebottles">Telegram group</a> · 
  <a href="https://usebottles.com/funding">Funding</a>
</div>

<br/>


## 📚 Documentación
Antes de abrir un nuevo tema, comprueba si ya se ha tratado el tema 
en nuestra [documentación](https://docs.usebottles.com).

Ten en cuenta que algunas páginas de la documentación aún se están redactando.


## 🦾 Características
- Creación de botellas basadas en entornos (un conjunto de reglas y dependencias)
- Acceso a un entorno personalizable para todos tus experimentos
- Instaladores automatizados
- Ejecución de todos los ejecutables (.exe/.msi/.bat) en tus botellas, utilizando el menú contextual de tu administrador de archivos
- Gestión y almacenamiento integrados para argumentos de archivos ejecutables.
- Compatibilidad con variables de entorno personalizadas.
- Sustituciones DLL simplificadas.
- Gestiona e instala múltiples versiones de Wine/Proton/dxvk y cambia sobre la marcha.
- Varias optimizaciones para un mejor rendimiento en juegos (esync, fsync, dxvk, caché, compilador de sombreadores, descarga... y mucho más).
- Ajuste diferentes configuraciones de prefijos de Wine sin salir de Bottles.
- Instalación automatizada de dxvk.
- Sistema para comprobar las actualizaciones de Runner para la botella y reparación automática en caso de avería.
- Instalador de dependencias integrado con comprobación de compatibilidad basada en un [repositorio](https://github.com/bottlesdevs/dependencies) impulsado por la comunidad.
- Detección de programas instalados.
- Administrador de tareas integrado para procesos Wine.
- Fácil acceso a ProtonDB y WineHQ para obtener asistencia.
- Sistema de actualización de configuraciones en todas las versiones de Bottles.
- Copia de seguridad e importación de Bottles desde versiones anteriores y desde otros administradores (Lutris, POL, etc.).
- Control de versiones de Bottles.
- ¡Y mucho más que podrás descubrir al instalar Bottles!

Traducción realizada con la versión gratuita del traductor DeepL.com

### 🚧 En desarrollo
- Capas (dependencias y programas en diferentes capas) [#510](https://github.com/bottlesdevs/Bottles/issues/510)

## ↗️ Instalar
Bottles se proporciona oficialmente como [Flatpak](https://flathub.org/apps/details/com.usebottles.bottles).

Lee [Aqui](https://docs.usebottles.com/getting-started/installation) Como instalar bottles en tu distribucion

### Avisos para los mantenedores de paquetes
Nos complace ver paquetes Bottles, pero les pedimos que respeten algunas pequeñas reglas:
- El paquete debe ser «bottles». En otras distribuciones es posible utilizar sufijos (por ejemplo, «bottles-git» en Arch Linux para el paquete basado en git), mientras que en otras se requiere el formato RDNN (por ejemplo, «com.usebottles.bottles» en elementary OS y el repositorio Flathub). Se desaconseja cualquier otra nomenclatura.
- No empaquete archivos externos y no realice cambios en el código, ni scripts duros. Obviamente, con la excepción de los archivos esenciales para el empaquetado.
- La versión del paquete debe seguir el modelo CalVer (año.mes.día) y el ciclo de lanzamiento del proyecto. Bottles tiene dos lanzamientos al mes: uno el día 14 y otro el día 28. Cuando se lanza una revisión, esta se añade a la versión de lanzamiento (por ejemplo, 2022.2.14-1). Bottles también tiene un nombre en clave que no es obligatorio y que actualmente solo utiliza Flatpak.

## Shortcuts
| Atajo    |         Acción           |
|:--------:|:------------------------:|
| `Ctrl+Q` |      Cerrar Bottles      |
| `Ctrl+R` | Recargar lista de Bottles|
|   `F1`   | Ir a la documentación    |
|  `Esc`   |       Ir atras           |

## Preguntas frecuentes
- [¿Porqué Bottles?](https://docs.usebottles.com/faq/why-bottles)
- [Donde esta Winetricks?](https://docs.usebottles.com/faq/where-is-winetricks)
- [¿Las versiones anteriores quedarán obsoletas?](https://docs.usebottles.com/faq/updates-and-old-versions#older-versions-will-be-deprecated)
- [¿Compatibilidad con versiones anteriores?](https://docs.usebottles.com/faq/updates-and-old-versions#backward-compatibility)

## Código de conducta
Este proyecto sigue el [Código de conducta de GNOME](https://wiki.gnome.org/Foundation/CodeOfConduct) Se espera que lo sigas en todos los espacios de Bottles, como este repositorio, las redes sociales del proyecto, los chats de mensajería y los foros. No se tolerará la intolerancia ni el acoso.

## PAtrocinadores
<a href="https://www.gitbook.com/?ref=bottles"><img height="55" src="https://www.gitbook.com/cdn-cgi/image/height=55,fit=contain,dpr=1,format=auto/https%3A%2F%2F2775338190-files.gitbook.io%2F~%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FNkEGS7hzeqa35sMXQZ4X%252Flogo%252FTO5E3RjWKeaJmYYWMGWV%252Fspaces_gitbook_avatar-rectangle.png%3Falt%3Dmedia%26token%3Da34e957e-f044-4bee-abee-23946d2e9cfb" /></a>&nbsp;&nbsp;&nbsp;
<a href="https://www.linode.com/?from=bottles"><img height="48" src="https://usebottles.com/uploads/linode-brand.png" /></a>&nbsp;&nbsp;&nbsp;
<a href="https://appwrite.io?from=bottles"><img height="48" src="https://usebottles.com/uploads/built-with-appwrite.svg" /></a>
