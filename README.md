//inicializa el repositorio vacio
git init

//esto nos ayuda agregar todos los archivos modificados al directorio al crear el commit
git add .

// este comando crea un commit con los cambios que tenemos y el -m es para poder añadirle un mensaje a este
git commit -m "configuracion inicial del proyecto"

//crea una nueva rama develop 
git branch dvelop

//csmbia de la rama actual a la creada develop
git checkout develop

//crea la rama feature desde la rama develop
git branch feature/inputs-calculadora

//muestra el estado de nuestro proyecto los archivos modificados y sin seguimieto
git status

//cambio a la rama develop para integrar los cambios con un merge prosimamente
git checkout develop

//itegramos los commits de la rama feature en develop
git merge feature/inputs-calculadora

//este comando crea y al mismo tiempo entra a trabajar en ella
git checkout -b featureopcion-menu-operacion-suma

//registramos el repositorio remoto 
git remote add origin https://github.com/urrego22/calculadora.git

// sube todas las ramas locales al repositorio remoto
git push --all origin

//nos muestra la lista de ramss locales
git branch

//cambiamos a la rama master y fusionamos a develop para integrar todo lo que esta en develop
git checkout master
git merge develop

//este comando sube la rama master al remoto 
git push -u origin master

//retos enfrentados 
al cambiar de una rama git mostarba m index.js porque habia cambios locales sin guardar de esto se aprende que antes de cambiar de rama hagamos un commit para evitar traer cambios no deseados.
al intentar hacer un git merge desde la rama feature desde su misma rama salio already up to date y de esto aprendi que siempre debes estar en la rama destion donde ira las modificacion antes de ejegutar un merge.
