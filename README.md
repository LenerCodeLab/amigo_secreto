<div align="center">

# 🎁 Amigo Secreto — Web App

Aplicación web para organizar sorteos de _amigo secreto_: añade participantes a una lista y realiza el sorteo de manera aleatoria.

### Oracle ONE & Alura Challenge Completado

<img width="500" height="500" alt="ff043987-239b-4661-bdb1-7f4ca6092c48" src="https://github.com/user-attachments/assets/11c18b91-1857-4754-bc76-c7bceef42c1e" />

### 🎯 Challenge: Amigo Secreto

<img width="493" height="399" alt="image" src="https://github.com/user-attachments/assets/8f8cbe1e-ebad-4bb2-9cda-40b14f0068bc" />

[🌐 Demo en vivo](https://lenercodelab.github.io/amigo_secreto/) ·
[💻 Repositorio](https://github.com/LenerCodeLab/amigo_secreto) ·
[👤 Portafolio GitHub](https://github.com/LenerCodeLab) ·
[🔗 LinkedIn](https://www.linkedin.com/in/lenerhuamanperales/)

<p>
<img src="https://img.shields.io/badge/STATUS-FINISHED-success">
<img src="https://img.shields.io/badge/HTML-5-E34F26?logo=html5&logoColor=white">
<img src="https://img.shields.io/badge/CSS-3-1572B6?logo=css3&logoColor=white">
<img src="https://img.shields.io/badge/JavaScript-ES6-F7DF1E?logo=javascript&logoColor=black">
</p>

</div>

---

## 📌 Descripción

**Amigo Secreto** permite ingresar nombres en una lista y realizar un sorteo aleatorio que muestra un único resultado por ronda. El enfoque del proyecto es practicar **lógica de programación**, **manipulación del DOM**, **validaciones** y **control de eventos** usando **HTML, CSS y JavaScript puro (vanilla)**.

> Metodología: desafío del programa **Oracle ONE & Alura** basado en _Challenge-Based Learning_ (Apple).

---

## ✨ Características

- ➕ **Agregar participantes:** campo de texto + botón _Añadir_.
- 📝 **Lista dinámica:** renderiza los nombres agregados en `<ul>`.
- 🎲 **Sorteo aleatorio:** selección de un participante al azar por ronda.
- 🧯 **Validaciones:** evita sorteos sin participantes y entradas vacías.
- ♿ **Accesibilidad básica:** `aria-live` para resultados y roles de lista.
- 🎨 **UI limpia:** tipografías de Google Fonts y paleta consistente.

---

## 🎮 Cómo usar

1. Escribe un nombre en el campo **"Escribe un nombre"** y pulsa **Añadir**.
2. Repite el proceso para todos los participantes.
3. Presiona **Sortear amigo** para obtener el resultado.
4. El resultado se mostrará en la sección **resultado**.

> Tip: puedes limpiar el campo y seguir agregando más nombres antes de volver a sortear.

---

## 🧠 Algoritmos implementados

- **Inserción y renderizado:** almacena los nombres en un array `amigos` y actualiza el DOM con `createElement/appendChild`.
- **Validación de entrada:** evita valores vacíos y muestra alertas informativas.
- **Sorteo aleatorio:** `Math.floor(Math.random() * amigos.length)` garantiza un índice válido.
- **Reinicio visual:** limpia la lista visible antes de mostrar el resultado del sorteo.

```js
// Sorteo principal
function sortearAmigo() {
  //Valida si hay amigos en el array
  if (amigos.length < 1) {
    alert("Ingresa los amigos para hacer el sorteo!");
    return;
  }

  amigoSecreto = Math.floor(Math.random() * amigos.length); //Realiza el sorteo

  const lista = document.getElementById("listaAmigos"); // Selecciona la lista <ul> y la borra por completo
  lista.innerHTML = "";

  const resultado = document.getElementById("resultado"); // Selecciona la lista <ul> resultado

  const nuevoElemento = document.createElement("li"); // Crea el <li>

  nuevoElemento.innerHTML = `Tu amigo secreto es ${amigos[amigoSecreto]}`; // Le pone el texto

  resultado.appendChild(nuevoElemento); // Lo agrega a la lista
}
```

---

## 🛠️ Stack y arquitectura de archivos

**Tecnologías:** HTML5 · CSS3 · JavaScript (Vanilla)

```
amigo_secreto/
│
├── index.html        # Estructura principal y accesibilidad
├── style.css         # Estilos: variables CSS, layout y componentes
├── app.js            # Lógica: agregar, listar y sortear amigos
├── assets/
│   ├── amigo-secreto.png
│   ├── play_circle_outline.png
│   └── image.png
└── README.md
```

---

## 📸 Capturas

<p align="center">
  <img src="https://github.com/user-attachments/assets/b747f0c3-b418-4d59-8b63-a6037bcce742" alt="Vista del banner" width="420">
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/5c34f40d-edbe-4fd4-984b-bf94dec08124" alt="Vista del banner" width="420">
</p>

---

## 🚀 Instalación y ejecución local

1. Clona el repositorio:

   ```bash
   git clone https://github.com/LenerCodeLab/amigo_secreto
   ```

2. Navegar al directorio del proyecto:

   ```bash
   cd amigo_secreto
   ```

3. Abrir el archivo HTML en tu navegador:
   ```bash
   open index.html
   # o simplemente haz doble clic en el archivo
   ```

---

## 🧩 Retos superados (learning outcomes)

- ✅ Manipulación de arrays y del DOM sin librerías.
- ✅ Validación de entradas y manejo de estados simples.
- ✅ Diseño UI con variables CSS y componentes reutilizables.
- ✅ Estructuración de funciones y limpieza del flujo de interacción.

---

## 🎓 Formación relacionada

**Lógica de Programación — Alura/ONE**

- [ ] Muestra mensajes en pantalla de forma interactiva.
- [ ] Uso de variables y buenas prácticas.
- [ ] Desarrollo de una app de principio a fin, inspirada en el mundo real.
- [ ] Adaptación de soluciones del lenguaje a problemas concretos.

**Lógica de Programación (Funciones y listas) — Alura/ONE**

- [ ] Uso de funciones y manipulación del DOM.
- [ ] Profundización en lógica con proyecto real.
- [ ] Publicación de proyectos con GitHub.
- [ ] Uso de listas (estructuras de datos), manipulación de palabras y números.

**Builds y Control de versiones — Git/GitHub**

- [ ] Diferencias entre Git y GitHub.
- [ ] Comandos esenciales y control de versiones.
- [ ] Estrategias de ramificación y navegación con `git log`.

---

## 🙌 Agradecimientos

Gracias a **Alura Latam** y **Oracle ONE** por el acompañamiento y la metodología basada en desafíos, que potencia el pensamiento lógico y la resolución de problemas.
<img width="561" height="230" alt="aluraoracle" src="https://github.com/user-attachments/assets/4586a001-d3be-403e-bd46-7164753001b3" />

---

## 👤 Autor

**Lener Augusto Nil Huamán Perales — LenerCodeLab**

- GitHub: https://github.com/LenerCodeLab
- LinkedIn: https://www.linkedin.com/in/lenerhuamanperales/

---

## 📝 Nota breve en inglés (summary)

**Secret Friend — Web App.** Add participants to a list and randomly draw one at a time. Built with HTML, CSS and vanilla JavaScript to practice DOM manipulation, validations and simple game logic. Live demo and repository above.
