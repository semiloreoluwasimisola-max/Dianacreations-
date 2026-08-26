const products = [
  {id:1, name:"Luxury Crochet Tote Bag", price:25000, img:"https://images.unsplash.com/photo-1591561954557-26941169b49e?w=500", category:"Bags", rating:5, desc:"Handmade with premium cotton yarn"},
  {id:2, name:"Crochet Summer Dress", price:35000, img:"https://images.unsplash.com/photo-1618354691792-d1d0572ce68b?w=500", category:"Dresses", rating:5, desc:"Beautiful handmade dress"},
  {id:3, name:"Baby Crochet Set", price:18000, img:"https://images.unsplash.com/photo-1515488042361-ee00e0ad8fe4?w=500", category:"Baby", rating:4, desc:"Soft and cozy for your little one"},
  {id:4, name:"Crochet Bucket Hat", price:12000, img:"https://images.unsplash.com/photo-1586790170532-2f9aef9f2f7c?w=500", category:"Hats", rating:5, desc:"Trendy and breathable"},
  {id:5, name:"Crochet Flower Bouquet", price:15000, img:"https://images.unsplash.com/photo-1457089328109-e5d9bd499191?w=500", category:"Flowers", rating:5, desc:"Never wilts, forever beautiful"},
  {id:6, name:"Crochet Slippers", price:10000, img:"https://images.unsplash.com/photo-1560769629-975ec94e6a86?w=500", category:"Accessories", rating:4, desc:"Comfortable and stylish"}
];
let cart = JSON.parse(localStorage.getItem('cart')) || [];
function updateCartCount(){const c=document.getElementById('cart-count');if(c)c.innerText=cart.length;}
function loadProducts(id){const g=document.getElementById(id);if(!g)return;products.forEach(p=>{g.innerHTML+=`<div class="product-card"><img src="${p.img}"><h3>${p.name}</h3><p>${p.desc}</p><p class="price">₦${p.price.toLocaleString()}</p><button onclick="addToCart(${p.id})" class="btn btn-gold">Add to Cart</button><a href="https://wa.me/2348025246991?text=Hello%20Diana%20Creations,%20I%20would%20like%20to%20order%20${encodeURIComponent(p.name)}" class="btn btn-rose">Order on WhatsApp</a></div>`});}
function addToCart(id){cart.push(products.find(p=>p.id===id));localStorage.setItem('cart',JSON.stringify(cart));updateCartCount();alert('Added to cart!');}
function toggleMenu(){document.getElementById('nav-menu').classList.toggle('active');}
loadProducts('featured-products');updateCartCount();
