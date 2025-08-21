<!doctype html>
<html lang="hi">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<title>Amrit Dhara Dairy Farm</title>
<style>
  :root{--green:#2f8f3f;--muted:#6b7280;--card:#fff;border-radius:10px}
  *{box-sizing:border-box}
  body{font-family:Inter, Arial, sans-serif;margin:0;background:#f7fbf7;color:#0f1720}
  header{background:linear-gradient(180deg,#f0fff4,#e6fff0);padding:20px 16px;border-bottom:1px solid #e6f5ea}
  .container{max-width:1100px;margin:0 auto;padding:18px}
  .brand{display:flex;gap:12px;align-items:center}
  .logo{width:60px;height:60px;border-radius:12px;background:linear-gradient(135deg,var(--green),#84cc16);display:inline-block}
  h1{margin:6px 0;font-size:24px;color:#174c17}
  p.lead{margin:6px 0;color:var(--muted)}
  nav{display:flex;gap:12px;flex-wrap:wrap;align-items:center}
  nav a{color:var(--green);text-decoration:none;font-weight:600}
  .hero{display:flex;gap:20px;align-items:center;justify-content:space-between;padding:28px;border-radius:12px;background:linear-gradient(90deg,#ffffff,#f6fff7);box-shadow:0 6px 18px rgba(20,60,20,0.04)}
  .cta{padding:12px 18px;background:var(--green);color:#fff;border-radius:10px;text-decoration:none;font-weight:700}
  .grid{display:grid;grid-template-columns:repeat(1,1fr);gap:16px;margin-top:18px}
  @media(min-width:760px){.grid{grid-template-columns:repeat(3,1fr)}}
  .card{background:#fff;padding:14px;border-radius:12px;border:1px solid #edf8ee;box-shadow:0 6px 18px rgba(18,52,18,0.03)}
  .product h3{margin:8px 0;font-size:18px;color:#0b3e0b}
  .price{font-weight:700;color:#0b3e0b}
  .btn{display:inline-block;padding:8px 12px;border-radius:8px;background:var(--green);color:#fff;text-decoration:none;border:none;cursor:pointer}
  .muted{color:var(--muted)}
  footer{padding:20px;text-align:center;color:var(--muted);margin-top:24px}
  /* cart / modal */
  .cart-btn{position:fixed;right:18px;bottom:18px;background:var(--green);color:#fff;padding:12px 14px;border-radius:999px;box-shadow:0 6px 20px rgba(20,60,20,0.15);border:none}
  .modal{position:fixed;left:0;top:0;width:100%;height:100%;display:none;align-items:center;justify-content:center;background:rgba(0,0,0,0.4);z-index:999}
  .modal.open{display:flex}
  .modal .inner{width:96%;max-width:720px;background:#fff;padding:18px;border-radius:12px;max-height:88vh;overflow:auto}
  label{display:block;margin:8px 0 4px}
  input[type="text"], input[type="email"], textarea, select{width:100%;padding:8px;border-radius:8px;border:1px solid #e6e6e6}
  table{width:100%;border-collapse:collapse}
  th,td{padding:8px;border-bottom:1px solid #f0f0f0;text-align:left}
  .small{font-size:13px;color:var(--muted)}
  .admin-link{font-size:13px;color:#444;text-decoration:underline;cursor:pointer}
  .pill{display:inline-block;padding:6px 10px;border-radius:999px;background:#ecfdf5;color:#065f46;font-weight:600}
</style>
</head>
<body>

<header>
  <div class="container" style="display:flex;align-items:center;justify-content:space-between;gap:12px;flex-wrap:wrap">
    <div style="display:flex;align-items:center;gap:12px">
      <span class="logo" aria-hidden="true"></span>
      <div>
        <strong style="font-size:18px">Amrit Dhara Dairy Farm</strong>
        <div class="small">ताज़ा शुद्ध दूध — Ranipur Adda, Patna City</div>
      </div>
    </div>
    <nav>
      <a href="#home" onclick="scrollToSection('home')">मुख पृष्ठ</a>
      <a href="#products" onclick="scrollToSection('products')">उत्पाद</a>
      <a href="#order" onclick="scrollToSection('order')">ऑर्डर</a>
      <a href="#contact" onclick="scrollToSection('contact')">संपर्क</a>
      <a id="myOrdersLink" href="#myorders" onclick="openMyOrders()">मेरे ऑर्डर</a>
    </nav>
  </div>
</header>

<main class="container" id="home" style="padding-top:18px">
  <section class="hero card" aria-labelledby="hero-title">
    <div>
      <h1 id="hero-title">ताज़ा दूध हर सुबह आपके घर</h1>
      <p class="lead">100% शुद्ध और ऑर्गेनिक — सीधे हमारे फार्म से। अभी ऑर्डर करें और ताज़ा दूध पायें।</p>
      <div style="margin-top:8px">
        <button class="cta btn" onclick="scrollToSection('products')">अभी ऑर्डर करें</button>
        <span class="pill" style="margin-left:12px">Contact: 9204146843</span>
      </div>
    </div>
    <div style="text-align:right">
      <img src="" alt="farm" style="width:220px;max-width:40vw" onerror="this.style.display='none'">
      <div class="small" style="margin-top:8px">ईमेल: amrit.dhara.dairy.farm1@gmail.com</div>
    </div>
  </section>

  <section id="products" style="margin-top:18px">
    <h2>हमारे उत्पाद</h2>
    <div class="grid">
      <!-- Products injected by JS -->
    </div>
  </section>

  <section id="order" style="margin-top:18px">
    <h2>ऑर्डर करें</h2>
    <div class="card" style="max-width:760px">
      <form id="checkoutForm">
        <label>नाम</label>
        <input type="text" id="custName" required placeholder="आपका नाम">

        <label>फ़ोन नंबर</label>
        <input type="text" id="custPhone" required placeholder="मोबाइल नंबर">

        <label>पता (Delivery Address)</label>
        <textarea id="custAddress" rows="2" required placeholder="नगर/कॉलोनी, Ranipur Adda, Patna City"></textarea>

        <label>उत्पाद चुनें</label>
        <select id="productSelect"></select>

        <label>मात्रा</label>
        <input type="number" id="productQty" min="1" value="1">

        <label>पेमेंट तरीका</label>
        <select id="paymentMode">
          <option>Cash on Delivery</option>
          <option>UPI / Paytm / PhonePe</option>
        </select>

        <div style="margin-top:12px;display:flex;gap:8px">
          <button type="submit" class="btn">ऑर्डर सबमिट करें</button>
          <button type="button" class="btn" style="background:#0b5" onclick="openCart()">कार्ट देखें</button>
        </div>
        <div id="checkoutMsg" class="small" style="margin-top:10px"></div>
      </form>
    </div>
  </section>

  <section id="tracking" style="margin-top:18px">
    <h2>ऑर्डर ट्रैकिंग</h2>
    <div class="card" style="max-width:720px">
      <form id="trackForm" onsubmit="event.preventDefault(); trackOrder();">
        <label>Order ID</label>
        <input type="text" id="trackId" required placeholder="उदा: 1690000000000">
        <label>ईमेल/फोन (Order पर दिया गया)</label>
        <input type="text" id="trackEmail" required placeholder="ईमेल या फ़ोन">
        <div style="margin-top:10px">
          <button class="btn" type="submit">ट्रैक करें</button>
        </div>
      </form>
      <div id="trackResult" style="margin-top:12px"></div>
    </div>
  </section>

  <section id="contact" style="margin-top:18px">
    <h2>संपर्क करें</h2>
    <div class="card" style="display:flex;flex-direction:column;gap:8px;max-width:720px">
      <div><strong>फोन:</strong> 9204146843, 7352809892</div>
      <div><strong>ईमेल:</strong> amrit.dhara.dairy.farm1@gmail.com</div>
      <div><strong>पता:</strong> Ranipur Adda, Patna City</div>
    </div>
  </section>

  <section id="about" style="margin-top:18px">
    <h2>हमारे बारे में</h2>
    <div class="card" style="max-width:720px">
      <p>Amrit Dhara Dairy Farm — प्राकृतिक तरीकों से पालित पशुओं का दूध, ताज़ा पैकिंग और सटीक डिलीवरी। हमारा लक्ष्य है कि आप हर सुबह शुद्ध दूध पायें।</p>
    </div>
  </section>

  <section id="myorders" style="margin-top:18px;display:none">
    <h2>मेरे ऑर्डर</h2>
    <div id="ordersList" class="card" style="max-width:820px"></div>
  </section>

  <section id="admin" style="margin-top:18px;display:none">
    <h2>एडमिन पैनल</h2>
    <div class="card" style="max-width:900px">
      <div style="display:flex;gap:8px;align-items:center;margin-bottom:10px">
        <label>Admin Password:</label>
        <input type="password" id="adminPass" style="width:200px">
        <button class="btn" onclick="openAdmin()">Open Admin</button>
      </div>
      <div id="adminArea"></div>
    </div>
  </section>

  <footer style="margin-top:30px">
    <div class="small">© <span id="year"></span> Amrit Dhara Dairy Farm • सभी अधिकार सुरक्षित</div>
    <div class="small">Privacy Policy | Contact Us</div>
  </footer>
</main>

<!-- Cart / Modal -->
<button class="cart-btn" onclick="openCart()">🛒 <span id="cartCount">0</span></button>

<div id="modal" class="modal" onclick="closeModal(event)">
  <div class="inner" onclick="event.stopPropagation()">
    <h3>कार्ट</h3>
    <div id="cartInner"></div>
    <div style="margin-top:12px">
      <button class="btn" onclick="checkoutFromCart()">चेकआउट</button>
      <button style="margin-left:8px" onclick="closeModal()">बंद करें</button>
    </div>
  </div>
</div>

<script>
/* ====== Initial Data ====== */
const PRODUCTS = [
  { id: 'milk-1l', title: 'दूध 1 लीटर', price: 90 },
  { id: 'milk-1-2l', title: 'दूध 1/2 लीटर', price: 50 },
  { id: 'paneer-250', title: 'पनीर 250g', price: 320 },
  { id: 'ghee-500', title: 'घी 500g', price: 600 }
];

const STORAGE_KEY = 'amrit_dhara_orders_v1';
const CART_KEY = 'amrit_dhara_cart_v1';
const ADMIN_PASSWORD = 'admin123'; // लोकल-एडमिन पासवर्ड (चाहे तो बदल दें)

/* ====== Helpers ====== */
function $(s){return document.querySelector(s)}
function $all(s){return Array.from(document.querySelectorAll(s))}
function saveOrders(orders){localStorage.setItem(STORAGE_KEY, JSON.stringify(orders))}
function loadOrders(){return JSON.parse(localStorage.getItem(STORAGE_KEY) || '[]')}
function saveCart(cart){localStorage.setItem(CART_KEY, JSON.stringify(cart))}
function loadCart(){return JSON.parse(localStorage.getItem(CART_KEY) || '[]')}
function genOrderId(){return Date.now().toString()} // सरल यूनिक id

/* ====== Render products on page ====== */
function renderProducts(){
  const grid = document.querySelector('.grid')
  grid.innerHTML = ''
  PRODUCTS.forEach(p=>{
    const div = document.createElement('div')
    div.className = 'card product'
    div.innerHTML = `<h3>${p.title}</h3><div class="price">₹ ${p.price}</div>
      <div style="margin-top:10px"><button class="btn" onclick="addToCart('${p.id}')">कार्ट में डालें</button></div>`
    grid.appendChild(div)
  })
  // product select for checkout
  const sel = document.getElementById('productSelect'); sel.innerHTML=''
  PRODUCTS.forEach(p=> sel.innerHTML += `<option value="${p.id}">${p.title} — ₹${p.price}</option>`)
}

/* ====== Cart functions ====== */
function addToCart(pid){
  const cart = loadCart()
  const existing = cart.find(i=>i.id===pid)
  if(existing){ existing.qty++ } else { cart.push({id:pid, qty:1}) }
  saveCart(cart); updateCartCount(); alert('Product added to cart')
}
function updateCartCount(){
  const cart = loadCart(); const count = cart.reduce((s,i)=>s+i.qty,0)
  document.getElementById('cartCount').innerText = count
}
function openCart(){
  const modal = document.getElementById('modal'); modal.classList.add('open')
  const inner = document.getElementById('cartInner'); const cart = loadCart()
  if(cart.length===0){ inner.innerHTML = '<p class="small">कार्ट खाली है।</p>'; return }
  let html = '<table><tr><th>उत्पाद</th><th>Qty</th><th>Price</th><th></th></tr>'
  cart.forEach(item=>{
    const p = PRODUCTS.find(pp=>pp.id===item.id)
    html += `<tr><td>${p.title}</td><td>${item.qty}</td><td>₹${p.price*item.qty}</td>
      <td><button onclick="removeItem('${item.id}')">हटाएँ</button></td></tr>`
  })
  const total = cart.reduce((s,i)=>s + PRODUCTS.find(p=>p.id===i.id).price * i.qty, 0)
  html += `<tr><td colspan="2"><strong>कुल</strong></td><td colspan="2"><strong>₹${total}</strong></td></tr></table>`
  inner.innerHTML = html
}
function removeItem(id){
  let cart = loadCart(); cart = cart.filter(i=>i.id!==id); saveCart(cart); updateCartCount(); openCart()
}
function closeModal(e){ document.getElementById('modal').classList.remove('open') }

/* ====== Checkout via main form (Order page) ====== */
document.getElementById('checkoutForm').addEventListener('submit', function(e){
  e.preventDefault();
  const name = $('#custName').value.trim()
  const phone = $('#custPhone').value.trim()
  const address = $('#custAddress').value.trim()
  const pid = $('#productSelect').value
  const qty = parseInt($('#productQty').value) || 1
  const payment = $('#paymentMode').value
  if(!name || !phone || !address){ $('#checkoutMsg').innerText = 'कृपया सभी फील्ड भरें।'; return }
  const prod = PRODUCTS.find(p=>p.id===pid)
  const orderId = genOrderId()
  const order = {
    id: orderId,
    name, phone, address,
    items: [{id:prod.id, title:prod.title, price:prod.price, qty}],
    total: prod.price * qty,
    paymentMode: payment,
    paymentStatus: payment==='Cash on Delivery' ? 'Unpaid' : 'Pending',
    status: 'Pending',
    created: new Date().toISOString()
  }
  const orders = loadOrders(); orders.push(order); saveOrders(orders)
  // clear cart & form
  saveCart([]); updateCartCount()
  $('#checkoutMsg').innerHTML = `आपका ऑर्डर जमा हो गया। Order ID: <strong>${orderId}</strong>. आपने चुना: <strong>${payment}</strong>.`
  // optionally show tracking result
  setTimeout(()=>{ $('#trackId').value = orderId; $('#trackEmail').value = phone; trackOrder() }, 500)
})

/* ====== Checkout from cart button ====== */
function checkoutFromCart(){
  const cart = loadCart()
  if(cart.length===0){ alert('कार्ट खाली है'); return }
  // prefill form with first item and qty sum
  const first = cart[0]; const prod = PRODUCTS.find(p=>p.id===first.id)
  $('#productSelect').value = prod.id; $('#productQty').value = cart.reduce((s,i)=>s + i.qty,0)
  closeModal()
  scrollToSection('order')
}

/* ====== Order Tracking ====== */
function trackOrder(){
  const id = $('#trackId').value.trim(); const key = $('#trackEmail').value.trim()
  const orders = loadOrders()
  if(!id || !key){ $('#trackResult').innerHTML = '<div class="small" style="color:#b91c1c">सभी फील्ड भरें</div>'; return }
  const order = orders.find(o => o.id === id && (o.phone===key || o.name.toLowerCase()===key.toLowerCase()))
  if(!order){ $('#trackResult').innerHTML = '<div class="small" style="color:#b91c1c">Order नहीं मिला — कृपया सही ID/फोन डालें</div>'; return }
  $('#trackResult').innerHTML = `<div><strong>Order ID:</strong> ${order.id}<br>
      <strong>स्थिति:</strong> ${order.status}<br>
      <strong>भुगतान:</strong> ${order.paymentStatus}<br>
      <strong>कुल:</strong> ₹${order.total}<br>
      <strong>ऑर्डर की तिथि:</strong> ${new Date(order.created).toLocaleString()}</div>`
}

/* ====== My Orders (customer view) ====== */
function openMyOrders(){
  const el = $('#myorders'); el.style.display = 'block'; scrollToSection('myorders')
  const container = $('#ordersList'); const orders = loadOrders()
  if(orders.length===0){ container.innerHTML = '<p class="small">कोई ऑर्डर नहीं मिला।</p>'; return }
  let html = '<table><tr><th>Order ID</th><th>नाम</th><th>आइटम</th><th>स्थिति</th><th>भुगतान</th></tr>'
  orders.slice().reverse().forEach(o=>{
    html += `<tr><td>${o.id}</td><td>${o.name} (${o.phone})</td><td>${o.items.map(i=>i.title+' ×'+i.qty).join('<br>')}</td>
      <td>${o.status}</td><td>${o.paymentStatus}</td></tr>`
  })
  html += '</table>'
  container.innerHTML = html
}

/* ====== Admin Panel ====== */
function openAdmin(){
  const pass = $('#adminPass').value
  if(pass !== ADMIN_PASSWORD){ alert('गलत पासवर्ड'); return }
  $('#admin').style.display = 'block'; scrollToSection('admin')
  renderAdmin()
}
function renderAdmin(){
  const orders = loadOrders().slice().reverse()
  if(orders.length===0){ $('#adminArea').innerHTML = '<div class="small">कोई ऑर्डर नहीं मिला।</div>'; return }
  let html = '<table><tr><th>Order ID</th><th>Customer</th><th>Items</th><th>Total</th><th>Payment</th><th>Status</th><th>Action</th></tr>'
  orders.forEach(o=>{
    html += `<tr>
      <td>${o.id}</td>
      <td>${o.name}<br><small>${o.phone}<br>${o.address}</small></td>
      <td>${o.items.map(i=>i.title+' ×'+i.qty).join('<br>')}</td>
      <td>₹${o.total}</td>
      <td>${o.paymentMode} / ${o.paymentStatus}</td>
      <td>${o.status}</td>
      <td>
        <select onchange="adminChangeStatus('${o.id}', this.value)">
          <option value="">-- Status चुनें --</option>
          <option value="Pending">Pending</option>
          <option value="Out for Delivery">Out for Delivery</option>
          <option value="Delivered">Delivered</option>
        </select>
        <br>
        <button onclick="markPaid('${o.id}')">Mark Paid</button>
      </td>
    </tr>`
  })
  html += '</table>'
  $('#adminArea').innerHTML = html
}
function adminChangeStatus(orderId, status){
  if(!status) return
  const orders = loadOrders()
  const idx = orders.findIndex(o=>o.id===orderId)
  if(idx===-1){ alert('Order not found'); return }
  orders[idx].status = status
  saveOrders(orders); renderAdmin(); alert('Status updated')
}
function markPaid(orderId){
  const orders = loadOrders()
  const idx = orders.findIndex(o=>o.id===orderId)
  if(idx===-1){ alert('Order not found'); return }
  orders[idx].paymentStatus = 'Paid'
  saveOrders(orders); renderAdmin(); alert('Payment marked Paid')
}

/* ====== Utility & Init ====== */
function scrollToSection(id){ document.getElementById(id).scrollIntoView({behavior:'smooth',block:'start'}) }
function init(){
  document.getElementById('year').innerText = new Date().getFullYear()
  renderProducts(); updateCartCount()
  // seed sample order if none (for demo) -- optional (comment out if not wanted)
  if(!localStorage.getItem(STORAGE_KEY)){
    const sample = [{ id: genOrderId(), name:'Ramesh', phone:'9000000000', address:'Ranipur Adda', items:[{id:'milk-1l',title:'दूध 1 लीटर',price:90,qty:1}], total:90, paymentMode:'Cash on Delivery', paymentStatus:'Unpaid', status:'Pending', created:new Date().toISOString() }]
    saveOrders(sample)
  }
}
init()
</script>

</body>
</html>
