# Instalación Backend BO

## Introducción
(Descripción del proyecto ?)

## Requisitos previos
Para realizar la instalación se necesitan las carpetas … visual studio code o similar … npm

## Instalación de paquetes
#### 1. Abre la carpeta del paquete y dirígete al archivo **package.json**.

![Alt text](<./assets/Paso 1 - short.png>)

#### 2. Una vez que hayas abierto el archivo **package.json**, verifica si el paquete seleccionado requiere a otros paquetes de **@club-personal**, estos se encuentran en **“dependencies”** o **“devDependencies”**.

   * **No tiene dependencias**: Si los paquetes presentes en el archivo package.json ya los has instalado previamente o simplemente no hay paquetes referenciados en el archivo, puedes continuar con el siguiente paso.

   * **Tiene Dependencias**: Si el paquete seleccionado tiene dependencias adicionales, deberás removerlas temporalmente del archivo package.json (ya que impedirán la instalación de tu paquete).

> [!IMPORTANT]
> En caso de que elimines dependencias, se recomienda guardarlas en otro documento hasta que sean requeridas nuevamente en el paso 5.

#### 3. Una vez que hayas terminado el paso anterior, según corresponda a tu caso, deberás **posicionar su terminal en la ruta del paquete**. 

>[!NOTE]
>En Visual Studio Code, esto se puede realizar de manera sencilla haciendo clic derecho en la carpeta del paquete y seleccionando **Open in Integrated Terminal** dentro del menú desplegable.

![Alt text](<./assets/Paso 2.png>)


> [!IMPORTANT]
> Asegúrate de que tu consola se encuentre en el directorio correcto.

#### 4. Una vez que tu terminal se encuentre en el directorio del paquete que deseas instalar, utiliza el comando **npm install**

> [!NOTE]
> Después de instalar, podrás ver que aparece la carpeta node_modules.

#### 5. Si eliminaste dependencias en el paso 2, deberás **restaurar** los cambios realizados en **package.json**

#### 6. Para finalizar, ejecuta el comando **npm link** seguido de los nombres de las dependencias del package.json referidas a otros paquetes **@club-personal**. 

> [!TIP]
> Ejemplo: **npm link @club-personal/club-personal-common-interfaces**

> [!NOTE]
> Si todo funcionó correctamente, podrás ver los cambios dentro de node_module>@club-personal

