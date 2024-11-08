# Pilas
#### Las **Pilas** almacenan datos siguiendo un concepto llamado FILO  (First In Last Off). Es decir, solo se  puede llamar al _ultimo_ elemento ingresado en ella, y al hacerlo el mismo es _eliminado_ de la estructura. Su declaracion puede ser algo similar a lo siguiente:
```python
    class Pila:
        
        def __init__(self):
            self.ls = []
            self.last_element = lambda : self.ls[len(self.ls)-1]   # Funcion lamda, puede ser remplazada por una funcion normal.
        
            
        def push(self,element):                                    # Tipicamente, se usa el comando "push(elemento)" para añadir a la estructura
            self.ls.append(element)                                # el elemento que deseemos. Siempre es añadido al final.
        
            
        def pop(self):                                             # Es el comando clasico que se usa para llamar al elemento correspondiente, en
            element = self.last_element()                          # el caso de las pilas llama al ultimo elemento. Luego es eliminado. 
            self.ls.remove(self.last_element())
            return element
```
# Colas
#### Las **Colas** almacenan datos siguiendo un concepto llamado FIFO  (First In First Off). Es decir, solo se  puede llamar al _primer_ elemento ingresado en ella, y al hacerlo el mismo es _eliminado_ de la estructura. Su declaracion puede ser algo similar a lo siguiente:
```python
class Cola:
    
    def __init__(self):
        self.ls = []
        self.first_element = lambda : self.ls[0]               # Funcion lamda, puede ser remplazada por una funcion normal.
    
        
    def push(self,element):                                    # Tipicamente, se usa el comando "push(elemento)" para añadir a la estructura
        self.ls.append(element)                                # el elemento que deseemos. Siempre es añadido al final.
    
        
    def pop(self):                                             # Es el comando clasico que se usa para llamar al elemento correspondiente, en
        element = self.first_element()                         # el caso de las colas llama al primer elemento. Luego es eliminado.
        self.ls.remove(self.first_element())
        return element
```

# Ejemplo visual:
```python
print("EJEMPLO, PILAS:")
pila = pila()

for i in range(10):
    pila.push(i)
    
for _ in range(10):
    print(f"\tUltimo elmento llamado: {pila.pop()}. Ahora fue eliminado.")
    print(f"\tElementos en la estructura: {pila.ls}")
    

print("----------------------------------------------------")
print("EJEMPLO, COLA:")

cola = cola()

for i in range(10):
    cola.push(i)
    
for _ in range(10):
    print(f"\tUltimo elmento llamado: {cola.pop()}. Ahora fue eliminado.")
    print(f"\tElementos en la estructura: {cola.ls}")
```
### Resultado:
```
EJEMPLO, PILAS:
        Ultimo elmento llamado: 9. Ahora fue eliminado.
        Elementos en la estructura: [0, 1, 2, 3, 4, 5, 6, 7, 8]
        Ultimo elmento llamado: 8. Ahora fue eliminado.
        Elementos en la estructura: [0, 1, 2, 3, 4, 5, 6, 7]
        Ultimo elmento llamado: 7. Ahora fue eliminado.
        Elementos en la estructura: [0, 1, 2, 3, 4, 5, 6]
        Ultimo elmento llamado: 6. Ahora fue eliminado.
        Elementos en la estructura: [0, 1, 2, 3, 4, 5]
        Ultimo elmento llamado: 5. Ahora fue eliminado.
        Elementos en la estructura: [0, 1, 2, 3, 4]
        Ultimo elmento llamado: 4. Ahora fue eliminado.
        Elementos en la estructura: [0, 1, 2, 3]
        Ultimo elmento llamado: 3. Ahora fue eliminado.
        Elementos en la estructura: [0, 1, 2]
        Ultimo elmento llamado: 2. Ahora fue eliminado.
        Elementos en la estructura: [0, 1]
        Ultimo elmento llamado: 1. Ahora fue eliminado.
        Elementos en la estructura: [0]
        Ultimo elmento llamado: 0. Ahora fue eliminado.
        Elementos en la estructura: []
----------------------------------------------------
EJEMPLO, COLA:
        Ultimo elmento llamado: 0. Ahora fue eliminado.
        Elementos en la estructura: [1, 2, 3, 4, 5, 6, 7, 8, 9]
        Ultimo elmento llamado: 1. Ahora fue eliminado.
        Elementos en la estructura: [2, 3, 4, 5, 6, 7, 8, 9]
        Ultimo elmento llamado: 2. Ahora fue eliminado.
        Elementos en la estructura: [3, 4, 5, 6, 7, 8, 9]
        Ultimo elmento llamado: 3. Ahora fue eliminado.
        Elementos en la estructura: [4, 5, 6, 7, 8, 9]
        Ultimo elmento llamado: 4. Ahora fue eliminado.
        Elementos en la estructura: [5, 6, 7, 8, 9]
        Ultimo elmento llamado: 5. Ahora fue eliminado.
        Elementos en la estructura: [6, 7, 8, 9]
        Ultimo elmento llamado: 6. Ahora fue eliminado.
        Elementos en la estructura: [7, 8, 9]
        Ultimo elmento llamado: 7. Ahora fue eliminado.
        Elementos en la estructura: [8, 9]
        Ultimo elmento llamado: 8. Ahora fue eliminado.
        Elementos en la estructura: [9]
        Ultimo elmento llamado: 9. Ahora fue eliminado.
        Elementos en la estructura: []
```
