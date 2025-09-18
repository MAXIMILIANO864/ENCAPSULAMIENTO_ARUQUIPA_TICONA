# ENCAPSULAMIENTO_ARUQUIPA_TICONA
Punto 2):
class Persona:
    def __init__(self, nombre: str, edad: int, sexo: str):
        self.nombre = nombre
        self.edad = edad
        self.sexo = sexo
    def cambiar_edad(self, nueva_edad: int):
        if nueva_edad < 0:
            print("Edad inválida: no puede ser negativa.")
            return
        self.edad = nueva_edad
    def mostrar_info(self):
        print(f"Nombre: {self.nombre} | Edad: {self.edad} | Sexo: {self.sexo}")
if __name__ == "__main__":
    p = Persona("Maríano", 25, "Masculino")
    p.mostrar_info()
    p.cambiar_edad(26)
    p.mostrar_info()
