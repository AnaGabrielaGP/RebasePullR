#   *__Tarea N°. 2__*
##   *Aplicaciones Móviles*
##   *Ana Gabriela García Páramo*

---
___Tarea:___  _Para qué nos sirve git rebase y sus aplicaciones en un pull request._ 

---
Para realizar la unión de ramas en Git existen dos maneras de realizarlo, ___marge___ y ___rebase___. Cuando se utiliza _rebase_, git duplica uno a uno todos los cambios realizados en la rama de trabajo y los lleva hacia la rama donde se requieren unir, los ubica uno tras otros en el orden que se crearon.  

_Rebase_ es una herramienta muy útil al momento de unir ramas ya que evitamos conflictos, un punto muy importante es que funciona siempre y cuando se realice con commits que no son públicos. ___Pull request___ nos permite realizar una petición para integrar nuestros cambios de código en algún proyecto que se encuentre en etapa de desarrollo.  

_Pull request_ es una herramienta de mucha utilidad cuando trabajamos en equipo pues se debe tener más precaución y es ahí cuando comienza su uso, dado que, en cada ocasión que se realice un cambio lo ideal es subir al repositorio la nueva rama y aquí es donde entra en el juego _git rebase_ para realizar la unión de las ramas. De esta manera se puede obtener de forma más detallada lo que hace el código, así, quien sea el encargado de la integración del proyecto pueda descargar la rama, realizar pruebas a los cambios y aprobar a rechazar la petición, además de realizar comentarios para futuras modificaciones.