# GIT

## Configuración global
```
git config --global --list
```
Listar configuración global
```
git config --list
```
Listar Configuración git


## Comandos Básicos
```
git init
```
Inicializar el repositorio

```
git add <nombre archivo>
```
Decirle a git que mape los cambies en el staging (Esos cambios esta guardado en la memoria RAM)

```
git commit -m "Mensaje Descriptivo"
```
Confirmar los cambios que estas siendo mapeados

```
git status
```
Ver el estado del flujo de trabajo. (Archivos sin mapear, sin confirmar)
## Branch (Ramas)
```
git branch <nombre de la rama>
```
Crear rama en git

```
git checkout <nombre de rama>
```
Cambiar de rama, indicando a que rama quierer ir

```
git branch -D <rama>
```
Eliminar una rama del entorno local
```
git branch -a
```
Se muestran todas las ramas tanto locales como remotas
## commit

```
git log
```
Ver commits realizados
```
git log --graph  
```
```
git log --all --graph 
```
```
git log --all --graph --decorate --oneline 
```
Ver flujo de trabajo por medio de la terminal de forma grafica

```
git log --stat
```
Ver estadisticas del cambio
```
git checkout <id commit, nombre commit>
```
Navegar por el flujo de trabajo

```
git rebase <rama>
```
Este comando une una roma en el extremo de otra. (Buena practica solo usar en entorno local, no usar en remoto) 
Primer cambio en la rama que tiene los cambios, segundo rebase a la rama final

```
git commit --amend
```
Enmienda un commit anterior
```
git log-S "cabecera" 
```
cuantas veces use la palabra cabecera en todos los commits.
## Cambios Temporales
```
git stash
```
Guardar cambios de forma temporal
```
git stash list
```
ver ubiación de los cambios temporales
```
git stash pop
```
Traer cambios guardados
```
git stash branch <rama>
```
Guardar cambios temporales en una rama
## Fusión de cambios
```
git merge <rama actualizada>
```
Fusionar dos ramas, en donde se deb estar posicionado en la rama desactualizada y desde ella llamar a la rama actualizada
## Tags
```
git tag -a <nombre tag> -m "Descripción del tag" <id commit ligado>
```
Crear tag asignado a un commit sobre la versión

```
git tag
```
Ver tags

```
git show-ref --tags
```
Ver tags con su referencia a que commit van ligados
```
git push origin --tags
```
Enviar cambios a repositorio remoto sobre los tags

# Buscar 
```
git grep <palabra a buscar> 
```
Buscar la palabra
```
git grep <palabra a buscar> -n
```
El -n es opcional indica en que archivo y en que linea encuentra la coincidencia
```
git grep -c <palabra a buscar> 
```
-c contar el número de veces que aparece la palabra
## Limpiar Repositorio Local, Archivos deseados

### Software Visual
```
gitk
```
Abre un software que se instala para ver el historial de los commits de una forma visual
## Cambios Reset
-- SOFT - Mantiene los cambios del stagfing
-- HARD - Resetea todo
```
git reset <commit>
```
Vuelve a un espacio temporal, reseteando cambios (Tener cuidado)
## Historial
```
git log
```
Ver el historial, pero lo eliminado no se ve
```
git reflog
```
Ve el historial completo del proyecto

## Colaborativos
```
git shortlog -sn  
```
muestra cuantos commit han hecho cada miembros del equipo.
```
git shortlog -sn --all
```
Muestra cuantos commit han hecho cada miembros del equipo hasta los que han sido eliminado
```
git shortlog -sn --all --no-merge
```
Muestra cuantos commit han hecho cada miembros quitando los eliminados sin los merges
```
git blame <ARCHIVO>
```
Muestra quien hizo cada cosa linea por linea
```
git COMANDO --help
```
Muestra como funciona el comando.
```
git blame ARCHIVO -Llinea_inicial,linea_final
```
Muestra quien hizo cada cosa linea por linea indicándole desde que linea ver ejemplo -L35,50
```
git branch -r
```
Se muestran todas las ramas remotas

# GITHUB
```
git remote add <nombre de la conexión remota> <url del repositorio>
```
Enlaza un repositorio local con uno remoto por medio de una conexión

```
git pull <nombre conexión> <nombre rama>
```
Traer los cambios de un repostorio remoto a local
```
git push <nombre conexión> <nombre rama>
```
Enviar cambios desde un repositorio local a uno remoto