# Modelos de distintas frutas en gazebo

Los modelos presentados en el siguiente repositorio son modelos integrados a gazebo, con el propósito de integrarlos a mundos de simulación que le permitan al brazo ejecutar rutinas de tal manera que encuentren un mundo simulado, con fines relativos al proyecto.

Para descargar los modelos se deben de ejecutar los siguientes comandos

```bash
  # Clonar el repositorio en una carpeta temporal de /tmp
  git clone https://github.com/Ivonneperezf/modelos_de_gazebo.git /tmp/modelos_gazebo

  # Copiar los modelos a ~/.gazebo/models
  cp -r /tmp/modelos_gazebo/* ~/.gazebo/models/

  # Eliminar la carpeta temporal
  rm -rf /tmp/modelos_gazebo
```

Todos los modelos contienen la siguiente estructura de carpetas, a continuación se ejemplifica con el modelo apple:

* **[apple](https://github.com/Ivonneperezf/modelos_de_gazebo/tree/main/apple):** Contiene los archivos de mallas, modelos y texturas en una jerarquía específica.
    * **[model.config](https://github.com/Ivonneperezf/modelos_de_gazebo/blob/main/apple/model.config):** Archivo que contiene los metadatos del modelo.
    * **[model.sdf](https://github.com/Ivonneperezf/modelos_de_gazebo/blob/main/apple/model.sdf):** Define toda la física y apariencia del modelo: geometría, peso, fricción, texturas y colisiones.
    * **[meshes](https://github.com/Ivonneperezf/modelos_de_gazebo/tree/main/apple/meshes):** Contiene los archivos del modelo en el aspecto visual.
        * **[apple.mtl](https://github.com/Ivonneperezf/modelos_de_gazebo/blob/main/apple/meshes/apple.mtl):** Le asigna información al modelo sobre qué texturas cargar y donde se encuentra esta textura.
        * **[apple.obj](https://github.com/Ivonneperezf/modelos_de_gazebo/blob/main/apple/meshes/apple.obj):** Contiene todo lo relativo al modelo de blender.
        * **[textures](https://github.com/Ivonneperezf/modelos_de_gazebo/tree/main/apple/meshes/textures):** Almacena todas las imagenes que se definan como texturas en el modelo.
            * **[Material_35_baseColor.png](https://github.com/Ivonneperezf/modelos_de_gazebo/blob/main/apple/meshes/textures/Material_35_baseColor.png):** Tanto el nombre como la extensión pueden variar, este archivo puede o no existir en el modelo y depende de la configuración, aunque de igual manera forma parte de la jerarquía de carpetas.

Los modelos se pueden obtener del sitio [sketchfab](https://sketchfab.com/).