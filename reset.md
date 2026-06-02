# Comando git reset
Deshace todos los commits después del commit especificado y mantiene los cambios de manera local.

# git reset --soft
Resetea cambios de commits desde el head y todo lo que vuelve para atras se guarda.

# git reset --hard
Resetea cambios de commits desde el head y todo lo que vuelve para atras se pierde.

-- Por ejemplo:
Si se hace un reset --hard con cambios sin commitear estos se pierden para siempre, porque no hay registro del commit en reflog.
Esto no sucede si se hizo un reset --soft, porque los commits que se vuelven hacia atras estan presentes en el reflog.