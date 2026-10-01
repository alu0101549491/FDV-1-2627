# FDV-1-2627

## Guión de la Práctica

1. Crear un proyecto Unity que incluya 2 objetos 3D. Crea un repositorio Git para el proyecto Unity. Posteriormente agrega un material para cada objeto siguiendo el flujo de trabajo de Unity.

2. Crea un repositorio Git LFS para el proyecto Unity del ejercicio anterior. Configura el fichero .gitattribute adecuado. Una segunda versión del fichero debe incluir un fichero de al menos 100 MB (por ejemplo un video en una carpeta Media) y un segundo script que muestre el mensaje en consola "Script tarea 1.1". Obtener capturas de pantalla del proceso para realizar la entrega de la práctica.

## Ejercicio 1

Dentro del editor de Unity se crearon dos objetos 3D simples: una esfera y un plano, a ambos se les aplicó dos materiales distintos, uno de ellos un color rojo y el otro un color azul.

![alt text](Media/scene.png)

Además, dentro de GitHub se creó el repositorio donde estaría almacenado el proyecto, con un .gitignore creado especialmente para proyectos de Unity.

![alt text](Media/repo.png)

## Ejercicio 2

Mediante los comandos de Git LFS el repositorio se convirtió en uno compatible con Git LFS creando el archivo .gitattributes.

```powershell
git lfs install

git lfs track "*.png"
git lfs track "*.fbx"
git lfs track "*.mp4"
git lfs track "*.gif"
```

Para comprobar su funcionamiento se agregó un vídeo al proyecto de más de 170 MB.

![alt text](Media/lfs.png)

Finalmente se creó un Script que escriba en consola la cadena "Script tarea 1.1", tal y como se puede observar en el código y en la propia ejecución del programa.

```cs
using System;
using UnityEngine;

public class Script1 : MonoBehaviour
{
    // Start is called once before the first execution of Update after the MonoBehaviour is created
    void Start()
    {
        Debug.Log("Script tarea 1.1");
    }
}
```

## Gif de Ejecución

![alt text](Media/1.gif)
