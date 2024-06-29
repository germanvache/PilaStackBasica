class Pila:
    def __init__(self):
        self.items = []

    def agregar(self, elemento):
        self.items.append(elemento)

    def quitar(self):
        if not self.esta_vacia():
            return self.items.pop()
        
        else:
            print("La pila esta vacia")

    def esta_vacia(self):
        return len(self.items) == 0
    
    def mostrar_conenido(self):
        print("Contenido de la pila:", self.items)

# Ejemplo de Uso
pila = Pila()
pila.agregar(5)
pila.agregar(10)
pila.mostrar_conenido()
pila.quitar()
pila.mostrar_conenido()
