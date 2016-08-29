___Tarea 01. Diferencia entre los comandos:___

    git reset --mixed (commit)    
    git reset --soft (commit)  

___

En un proyecto (en git), existen algunas maneras para regresar a un estado anterior. A continuación se hace mención de estos comandos que nos permiten realizar la acción anterior:  

___Hard:___   git reset --hard (commit)  
* Ignora por completo todos los cambios que se han realizado (los commits más nuevos).  
* Reestablece el indice y la rama del trabajo al punto donde se encontraban.  

___Soft:___   git reset --soft (commit)  
* No deshace el estado actual del proyecto para regresar a un punto específico.
* Cuando se utiliza este comando, todos los archivos que pertenecen a commits anteriores se quedan en "stage" para alguna oeración extra que se desee realizar.  

___Mixed:___    git reset --mixed (commit)  
* Actua e forma similar o parecida a soft.
* Una de las diferencias respecto a soft es que los cambios no se quedan en el "stage".
* Git usa por defecto este comando cuando no se asigna una bandera (hard, soft, mixed).  

Los comandos anteriormente mencionados nos permiten reestablecer un proyecto a estados anteriores, puede ser de manera parcial o total dependiendo la circunstancia. 
 

    
