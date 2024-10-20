# Angel-Alejandro-Sepulveda-Gonzalez-3W-1215-PR-2

# Angel Alejandro Sepulveda Gonzalez, 3W, 1215

# Función para crear un diccionario de traducción

def crear_diccionario():

  # Pedir al usuario que introduzca las palabras en formato <palabra>:<traducción> separadas por comas
  
  palabras = input("Introduce las palabras en español-inglés separadas por dos puntos y por comas (ej: hola:hello, casa:house): ")
    
  # Crear el diccionario usando comprensión de diccionarios
    
  diccionario = {par.split(":")[0].strip(): par.split(":")[1].strip() for par in palabras.split(",")}
    
  # Devolver el diccionario creado
  
  return diccionario

# Función para traducir una frase usando el diccionario

def traducir_frase(diccionario):

  # Pedir al usuario una frase en español
  
  frase = input("Introduce una frase en español: ")
    
  # Traducir palabra por palabra
  
  traduccion = []
    
  for palabra in frase.split():
  
  # Si la palabra está en el diccionario, traducirla; si no, dejarla igual
  
  traduccion.append(diccionario.get(palabra, palabra))
    
  # Unir las palabras traducidas en una sola cadena
  
  print("Frase traducida:", " ".join(traduccion))

# Crear el diccionario de traducción

diccionario_traduccion = crear_diccionario()

# Traducir una frase con el diccionario creado

traducir_frase(diccionario_traduccion)

![image](https://github.com/user-attachments/assets/adeb3ec7-627b-4a7e-999e-38b5075806be)  ![image](https://github.com/user-attachments/assets/ebc17ec6-50a0-4f70-b9c0-e1286035cae4)
![image](https://github.com/user-attachments/assets/512c3df5-c9c2-4b0f-ad25-1f1e48f24338)
![image](https://github.com/user-attachments/assets/efd7470b-777d-4f1c-8c61-68aed3b45866)




