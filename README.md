# Carrito-de-compras
Se trata del carrito de compras con el diseño responsive, ahi estan los siguientes codigos, donde la condicion que se puede editar para poner atributos

HTML:
HTML:
<!-- Vista de usuario -->
<div id="cart">
  <h2>Carrito</h2>
  <div id="cart-items"></div>
  <div id="cart-total"></div>
  <button id="checkout-btn">Checkout</button>
</div>

<!-- Vista de admin -->  
<div id="admin">
  <h2>Administración de Productos</h2>
  
  <div id="product-form">
    <label>Nombre:</label>
    <input type="text" id="product-name">
    
    <label>Precio:</label>  
    <input type="number" id="product-price">
    
    <label>Descripción:</label>
    <textarea id="product-desc"></textarea>
    
    <button id="add-product">Agregar Producto</button>
  </div>
  
  <ul id="product-list"></ul>
</div>

JS: 
// Carrito
let cart = [];

// CRUD de productos
function addProduct(name, price, desc) {
  // agregar lógica
}

function editProduct(id, updates) {
  // agregar lógica  
}

function deleteProduct(id) {
  // agregar lógica
}

// Renderizar vistas
function renderProducts() {
  // agregar lógica
}

function renderCart() {
  // agregar lógica  
}

// Detectar clicks
document.getElementById('add-product').onclick = () => {
  // llamada a addProduct
};

// Persistencia local
function saveCart() {
  localStorage.setItem('cart', JSON.stringify(cart));
}

function loadCart() {
  cart = JSON.parse(localStorage.getItem('cart')) || [];
}

CSS:
/* Estilos responsive */

@media (max-width: 600px) {
  /* Estilos móvil */
}

@media (min-width: 600px) {
  /* Estilos de */


# Autor
Ruben Cerna Mendoza (rcerna@uees.edu.ec)
