Ya disponíamos de una cuenta de github por lo que no hemos necesitado crear ninguna nueva. Hemos dado de alta un proyecto llamado dca-scv. 

Crearemos un alias global para branch como br con este comando 
git config --global alias.br branch

Y como alias local hemos puesto status como st
git config alias.st status

Para provocar el fallo, vamos a introducir en una calculadora que a la hora de sumar reste, posteriormente llegamos a ese commit y lo solucionamos. Para solucionarlo hemos utilizado git bisect. Hemos introducido git bisect start tagbueno tagmalo y nos ha llevado a la mitad, en este hemos encontrdado el error y lo hemos solucionado.

He introducido el hook pre-commit, el cual imprimirá "Ejecutando el script pre-commit" cada vez que realice un commit. Para ello en la carpeta .git/hooks he creado el archivo pre-commit, he introducido las reglas a seguir y lo he convertido en un ejecutable.
