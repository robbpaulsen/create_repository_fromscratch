# create_repository_fromscratch

Breve manual/instructivo revelando la verdad que casi todo usuari de github o pentester a buscado, los pasos que se deben de seguir para crear tu primer repositorio, configruar tus credenciales de usuario para identificacion por medio de "SSH" o navegador.

## Este es Breve manual/instructivo

 Revelando la verdad que casi todo usuari de github o pentester a buscado, los pasos que se deben de seguir para crear tu primer repositorio, configruar tus credenciales de usuario para identificacion por medio de "SSH" o navegador (sugiero que de escoger esta opcion tengan buen sentido de la privacidad y no mezclen su pestanas de Facebook y cuentas de banco en el mismo navegador ya que es muy facil el filtrado de contrasenas cuado se esta trabjando con conexiones remotas.

Por que escribir este breve instructivo? , por el hecho de que en la plataforma tiene mas de 10 mil enciclopedias y tutoriales no exlica en ningun momemnto ni de forma clara/definitiva como se crea un repositorio por primera vez desde cero, todo el tiempo aborda el tema de una perspectiva que estaras agregando y/o apoyando a algun proyecto ya hecho por alguien mas, asi que despues de 5 meses de estar ebrio frente a mi monitor y gritandole a youtubers que pakabra por palabra solo leen en voz alta el manual/documentacion del sitio, asi que decidi intentar todas las combinaciones posibles de los comandos que en la Wiki de Github muestran, sin mencionar que ignoran los otros mas de 20 comandos que faltan.

```

"Parece chiste pero es anecdota"


-- Franco Escamilla

```

Antes que nada advierto que sin ser muy conciente al respecto cambio de idioma al escribir, estas avisado. Github es la plataforma Online de codigo abierto y en su mayoria gratuita mas grande del mundo y fue adquirida por Microsoft hace aproximadamente 5 anos (ano en el que escribo esto es el 2023). Su plataforma tiene el exito debido a que todos los desarrolladores (No necesariamnte con algun certificado de institucion educativa) pueden almacenar todo su codigo gratuitamente y no te limitan o revisan a que solo puedan ser archivo hecho en tu bloque den notas siempre y cuando se respeten derechos de autor y se de el credito a quien se le debe de otorgar se puede cargar a sus nube hasta las fotos de tus vacacaciones en Acapulco.

La regla que existe y que se respeta entre la comunidad es que todo lo publicado debera de ser, valg ala redundancia "Publico" por el tiempo que ese codigo resida en su plataforma , si el desarrollador decide que vendera su patente o servicio lo unico que sucede que se convierte en un cliente de paga en su plataforma la cual cuesta 200 dolares anuales, lo cual no es nada descabellado.

## Ya en la siguiente parte estara toda la guia.


## Todo esto se realiza en tu terminal de de comandos favorita, aqui no contamos y no sabemos como se hace de otra forma. De nuevo estas avisado ;)

Open Terminal.

```
** Set a Git username:

$ git config --global user.name "Mona Lisa"

** Confirm that you have set the Git username correctly:

$ git config --global user.name

Mona Lisa
```

** Setting your commit email address in Git:

You can use the git config command to change the email address you associate with your Git commits. The new email address you set will be visible in any future commits you push to GitHub.com from the command line. Any commits you made prior to changing your commit email address are still associated with your previous email address.
Setting your email address for every repository on your computer

    Open Terminal.

** Set an email address in Git. You can use your GitHub-provided noreply email address or any email address:

```
   
    $ git config --global user.email "YOUR_EMAIL"

** Confirm that you have set the email address correctly in Git:

    $ git config --global user.email
    email@example.com
```

Add the email address to your account on GitHub, so that your commits are attributed to you and appear in your contributions graph. For more information, see "Adding an email address to your GitHub account."

## Start a new repository and publish it to GitHub

First, you will need to create a new repository on GitHub. For more information, see "Hello World." Do not initialize the repository with a README, .gitignore or License file. This empty repository will await your code.

## create a new directory, and initialize it with git-specific functions

```

$ git init my-repo
```

## change into the `my-repo` directory

```

 cd my-repo
```

## create the first file in the project

```

touch README.md
```

## git isn't aware of the file, stage it

```

git add README.md
```
 
## take a snapshot of the staging area

```

git commit -m "add README to initial commit"
```

## provide the path for the repository you created on github

```

git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY-NAME.git
```

## push changes to github

```

git push --set-upstream origin main
```


## Contribute to an existing repository

** download a repository on GitHub to our machine
** Replace `owner/repo` with the owner and name of the repository to clone

```

git clone https://github.com/owner/repo.git
```

## change into the `repo` directory

```

cd repo
```
## create a new branch to store any new changes

```

git branch my-branch
```

## switch to that branch (line of development)

```

git checkout my-branch
```

_make changes, for example, edit `file1.md` and `file2.md` using the text editor_


## stage the changed files

```

git add file1.md file2.md
```

## take a snapshot of the staging area (anything that's been added)

```

git commit -m "my snapshot"
```

## push changes to github

```

git push --set-upstream origin my-branch
```