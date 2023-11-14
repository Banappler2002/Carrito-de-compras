# Carrito-de-compras
Se trata del carrito de compras con el diseño responsive, ahi estan los siguientes codigos, donde la condicion que se puede editar para poner atributos


# Codigo HTML:
<!-- Vista de usuario -->
<div id="cart">
  <h2>Carrito</h2>
  <div id="cart-items"></div>
  <div id="cart-total"></div>
</div>

<!-- Vista de admin -->  
<div id="admin">
  <h2>Administración de productos</h2>
  
  <div id="product-list"></div>
  
  <div id="product-form">
    <label for="name">Nombre:</label>
    <input type="text" id="name">
    
    <label for="price">Precio:</label>  
    <input type="number" id="price">
    
    <label for="color">Color:</label>
    <input type="text" id="color">
    
    <button id="save-product">Guardar Producto</button>
  </div>
</div>

# Codigo Javascript
// Almacenamiento local
let store = window.localStorage;

// Obtener productos
function getProducts() {
  return JSON.parse(store.getItem('products')) || [];
}

// Guardar productos
function saveProducts(products) {
  store.setItem('products', JSON.stringify(products));
}

// CRUD de productos
const productList = document.getElementById('product-list');
const productForm = document.getElementById('product-form');

// Mostrar productos
function renderProducts() {
  let products = getProducts();
  
  // Código para pintar productos...  
}

renderProducts();

// Agregar producto
productForm.addEventListener('submit', e => {
  e.preventDefault();
  
  let products = getProducts();
  
  // obtener datos del formulario
  
  let newProduct = {
    name, 
    price,
    color
  };
  
  products.push(newProduct);
  
  saveProducts(products);
  
  renderProducts();
}); 

// Eliminar producto
function deleteProduct(productId) {
  let products = getProducts();
  // filtrar productos
  
  saveProducts(products);
  
  renderProducts();
}

// Editar producto
function editProduct(productId, updates) {
  let products = getProducts();
  
  // encontrar y actualizar producto 
  
  saveProducts(products);
  
  renderProducts();
}

// Lógica del carrito
let cart = [];

// Agregar al carrito
function addToCart(productId) {
  // encontrar el producto
  // agregar al carrito
  
  renderCart();
}

// Renderizar carrito
const cartDiv = document.getElementById('cart');

function renderCart() {
  // pintar productos del carrito
}

renderCart();

# Codigo CSS:
/* Estilos responsive */

@media (max-width: 600px) {
  /* Estilos móvil */
}

@media (min-width: 600px) {
  /* Estilos de */


# Autor
Ruben Cerna Mendoza (rcerna@uees.edu.ec)
