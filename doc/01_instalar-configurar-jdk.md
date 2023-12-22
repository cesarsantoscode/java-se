### 01. Instalar y configurar JDK
El primer paso para desarrollar con Java es instalar el JDK 
y configurar la variable de entorno JAVA_HOME.

#### A. Instalar el JDK
- Se tiene diferentes opciones para descargar el JDK. Algunas de 
ellas son: 

  - [JDK de Oracle](https://www.oracle.com/pe/java/technologies/downloads/)
  - [OpenJDK de Adoptium](https://adoptium.net/es/)

#### B. Configurar la variable de entorno JAVA_HOME
- Copiar la ruta de instalación del JDK, en mi caso es: 
  ``` bash
  /Users/<user>/Documents/Software/JDK/jdk-17.0.9+9/Contents/Home
  ```

- Ubicarse en el directorio home:
  ```bash
  cd ~
  ```

- Crear o editar el archivo de configuración de usuario:
  ```bash
  vi .bash_profile
  ```  
  > Nota: Si está utilizando "oh-my-zsh.sh" debe editar el archivo ".zshrc"

- Agregar el valor a la variable de entorno JAVA_HOME:
  ```bash
  export JAVA_HOME=/Users/<user>/Documents/Software/JDK/jdk-17.0.9+9/Contents/Home
  ```

- Finalmente validamos la versión de Java:
  ```bash
  java -version
  ```

- El resultado será como el siguiente:
  ```bash
  openjdk version "17.0.9" 2023-10-17
  OpenJDK Runtime Environment Temurin-17.0.9+9 (build 17.0.9+9)
  OpenJDK 64-Bit Server VM Temurin-17.0.9+9 (build 17.0.9+9, mixed mode)
  ```