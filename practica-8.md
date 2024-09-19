**Edgar Edán Arriaga Quiroz**

## a.      ¿Cómo se inicializa un repositorio en Git?

```bash
git init
```

## b.      ¿Cómo creas un repositorio en GitHub?

- Entrar a la página de GitHub e iniciar sesión
- En la parte superior izquierda de la pantalla debe indicar que te encuentras en el _dashboard_, debajo de esa indicación se encuentran los repositorios, dar clic al botón verde que dice _**"New"**_
- Tras dar clic se abrirá una pantalla de configuración del repositorio. Tras configurar las opciones de nuestro repositorio, en la parte inferior de la pagina a mano derecha habrá un botón verde que diga _**Create repository**_, damos clic en este y listo, habrémos creado un repositorio.

## c.      ¿Cómo vinculas un repositorio local de Git con uno remoto en GitHub?

```bash
git remote add origin url-del-repositorio-en-GitHub
```

## d.      ¿Cuál es el flujo básico de trabajo en Git y GitHub?

```bash
git add .
git commit -m "Mensaje del commit"
git push -u origin main

git pull
```
- **add** sube los cambios al stage del repositorio
- **commit** agrega un mensaje y confirma los cambios
- **push** sube los cambios al repositorio remoto, la primera vez que se usa se debe escribir con -u origin main, despues ya solo es necesario **git push**
- **pull** actualiza los datos de tu repositorio local con los datos del remoto, en caso de que el local no esté al día.

## e.      ¿Para qué sirve el archivo .gitignore?

- Permite establecer archivos que serán ignorados por el flujo de trabajo, para no ser agregados o subidos al repositorio remoto. Si tu por ejemplo en ese archivo agregas "* .exe" estarás evitando que los ejecutables sean considerados para agregarse al repositorio remoto.

## f.       ¿Cuál es el propósito de una rama?

- Trabajar y alterar información ya sea existente, o nueva de forma separada, sin afectar a la composición de la _rama main_ del proyecto, posteriormente podemos agregar esa información a _main_

## g.      ¿Qué es una fusión?

- Agregar la información de una rama secundaria a la rama principal.

## h.      Explica los diferentes tipos de fusión que existen.

- **Rápida**: La información de ambas ramas se combina sin problemas.
- **Manual**: Cuando la información de ambas ramas se sobrepone una de otra, Visual Studio nos pide que seleccionemos y reordenemos la información de ambas ramas por nuestra cuenta.

## i.       ¿Cómo puedes ver el historial de tu repositorio?

```bash
git log
```

## j.       ¿Cuál es el propósito de una etiqueta?

- Agregar información de la versión de nuestro repositorio, por ejemplo v1.0.0