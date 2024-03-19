# ES23UAB-411-03
---
Pràctiques Enginyeria del Software  
Autors: Luca Meloni, Aaron Condoblea, Albert Vacas, José Ortín, Adrià Martìn
---
# Organización General
Hay varios puntos claves en la creación requisitos, organización del GitHub, Jira, etc. En este documento pretendo estandarizar el flujo de trabajo para este proyecto. 
#### Creación de Requisitos
En la carpeta '/requiremets' encontraremos una plantilla des de donde podremos crear nuestros requisitos. Estos contienen varios campos como el ID, la versión, tipo etc. En general estos campos ofrecen bastante libertad y cada uno los puede rellenar como guste, solo hay que tener en cuenta estos aspectos:
* IDs: Estos tienen que formarse de la siguiente manera. 'RQ-X.YY' donde 'X' corresponde al paragrafo CAT-XX del enunciado de la práctica y 'YY' indentifican el requisito dentro de la categoria. Ex. &rarr; RQ-1.01 corresponde al requisito nº 1 de la categoria 1.
* Comentarios: Cada vez que creemos o actualizemos un requistio abrá que dejar por escrito quien y cuando ha hecho la modificación/creación y, si es necesario, algún mensaje para que los demás integrantes puedan tener más contexto.  
Ex. &rarr;  Edited by Adri. [18/03/2024] He agrupado todos los requisitos en una misma carpeta.
* Nombre del archivo: El nombre del archivo del requisito tiene que se el mismo de el ID seguido de .md como extensión.
#### Gestión del Projecto en GitHub
Aparte de las carpetas exigidas por el enunciado de la práctica es necesario formalizar como trabajaremos en GitHub. En este aspecto optaremos por hacer una aproximación sencilla, cada uno tendrà una rama con su nombre des de donde podrá actualizar el proyecto. Entonce el flujo de trabajo será el siguiente:
1. Haremos ```git pull``` de *master* en nuestra rama personal, para tener el proyecto actualizado.
2. Procederemos ha hacer los cambios necesarios en nuestra rama.
3. Cuando hayamos acabado haremos un ```git commit``` de nuestros cambios.[^1]
4. Por último haremos ```git push``` tanto en nuestra rama como en *master*, si es una versión definitiva.[^2] 

[^1]: Los mensajes de los commits deberán seguir este formato: "CX: *Your commit message*.  
La primera X hace referencia al número de commit. **Aclaración** &rarr; Cada rama tendrá su propia seqüencia. 
[^2]: En el caso de *master* se tendrá que hacer un forward merge antes de poder hacer un push.