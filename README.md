# Stream25import streamlit as st
import random

# Lista de temas para charadas
temas = [
    "Películas",
    "Famosos",
    "Acciones",
    "Animales",
    "Objetos de la casa",
    "Profesiones",
    "Países",
    "Deportes",
    "Superhéroes",
    "Canciones",
    "Historias famosas",
    "Comida",
]

# Título de la aplicación
st.title("Generador de Temas para Charadas")

# Instrucciones
st.write("""
    Este generador te ayudará a encontrar un tema para jugar a las charadas.
    Haz clic en el botón para obtener un tema aleatorio.
""")

# Botón para generar un tema
if st.button('Generar Tema'):
    tema_aleatorio = random.choice(temas)
    st.write(f"**Tema seleccionado:** {tema_aleatorio}")
else:
    st.write("Haz clic en el botón para generar un tema.")
