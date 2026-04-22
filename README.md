<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Amineha — Premium Brass Parts Manufacturer</title>
<link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet">
<style>
  * { box-sizing: border-box; margin: 0; padding: 0; }
  html { scroll-behavior: smooth; }
  body { font-family: 'Inter', Arial, sans-serif; background: #111; color: #fff; }
 
  nav {
    position: sticky; top: 0; z-index: 99;
    background: rgba(10,10,10,0.95);
    backdrop-filter: blur(10px);
    border-bottom: 1px solid rgba(184,115,51,0.3);
    padding: 0 40px; height: 64px;
    display: flex; align-items: center; justify-content: space-between;
  }
  .logo { font-family: 'Bebas Neue', sans-serif; font-size: 1.7rem; letter-spacing: 0.1em; color: #D4A055; }
  .logo span { color: #fff; }
  .nav-links { display: flex; align-items: center; gap: 28px; }
  .nav-links a { color: rgba(255,255,255,0.7); text-decoration: none; font-size: 0.8rem; font-weight: 500; letter-spacing: 0.1em; text-transform: uppercase; transition: color 0.2s; }
  .nav-links a:hover { color: #D4A055; }
 
  .btn { display: inline-block; padding: 11px 22px; background: #B87333; color: #000; font-family: 'Inter', sans-serif; font-size: 0.78rem; font-weight: 600; letter-spacing: 0.12em; text-transform: uppercase; text-decoration: none; border: none; border-radius: 2px; cursor: pointer; transition: background 0.2s, transform 0.15s; }
  .btn:hover { background: #D4A055; transform: translateY(-1px); }
  .btn-outline { background: transparent; color: #fff; border: 1px solid rgba(255,255,255,0.3); }
  .btn-outline:hover { border-color: #D4A055; color: #D4A055; background: transparent; }
  .btn-green { background: #25D366; color: #fff; }
  .btn-green:hover { background: #1ebe5a; }
 
  .section { padding: 80px 40px; }
  .label { font-size: 0.68rem; letter-spacing: 0.3em; text-transform: uppercase; color: #B87333; margin-bottom: 12px; display: flex; align-items: center; gap: 10px; }
  .label::before { content: ''; width: 30px; height: 1px; background: #B87333; }
  h1 { font-family: 'Bebas Neue', sans-serif; font-size: clamp(3rem, 7vw, 6rem); letter-spacing: 0.04em; line-height: 1; margin-bottom: 20px; }
  h1 span { color: #D4A055; }
  h2 { font-family: 'Bebas Neue', sans-serif; font-size: clamp(2rem, 4vw, 3rem); letter-spacing: 0.05em; margin-bottom: 10px; }
  h2 span { color: #D4A055; }
  p { color: rgba(255,255,255,0.6); line-height: 1.7; font-size: 0.95rem; }
 
  #hero { min-height: 90vh; display: flex; flex-direction: column; justify-content: center; background: radial-gradient(ellipse 70% 60% at 80% 50%, rgba(184,115,51,0.1) 0%, transparent 70%), #111; border-bottom: 1px solid rgba(184,115,51,0.15); }
  #hero p { max-width: 480px; margin-bottom: 32px; font-size: 1.05rem; }
  .hero-btns { display: flex; gap: 12px; flex-wrap: wrap; }
 
  .marquee { background: #B87333; padding: 12px 0; overflow: hidden; white-space: nowrap; }
  .marquee-inner { display: inline-block; animation: marquee 18s linear infinite; }
  .marquee-inner span { font-family: 'Bebas Neue', sans-serif; font-size: 0.9rem; letter-spacing: 0.2em; color: #000; padding: 0 24px; opacity: 0.75; }
  @keyframes marquee { from { transform: translateX(0); } to { transform: translateX(-50%); } }
 
  #about { background: #1a1714; border-top: 1px solid rgba(184,115,51,0.1); border-bottom: 1px solid rgba(184,115,51,0.1); }
  .about-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 16px; margin-top: 32px; }
  .about-card { background: rgba(184,115,51,0.06); border: 1px solid rgba(184,115,51,0.15); border-radius: 4px; padding: 20px; }
  .about-card .icon { font-size: 1.8rem; margin-bottom: 10px; }
  .about-card h4 { font-size: 0.88rem; font-weight: 600; color: #fff; margin-bottom: 6px; }
  .about-card p { font-size: 0.78rem; }
 
  #products { background: #111; }
  .tabs { display: flex; gap: 8px; flex-wrap: wrap; margin: 16px 0 28px; }
  .tab { padding: 6px 16px; font-size: 0.72rem; letter-spacing: 0.1em; text-transform: uppercase; border: 1px solid rgba(184,115,51,0.25); border-radius: 2px; color: rgba(255,255,255,0.5); cursor: pointer; background: transparent; font-family: 'Inter', sans-serif; transition: all 0.2s; }
  .tab:hover, .tab.active { background: #B87333; border-color: #B87333; color: #000; font-weight: 600; }
  .products-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(260px, 1fr)); gap: 2px; background: rgba(184,115,51,0.08); }
  .product-card { background: #111; padding: 24px; transition: background 0.2s; }
  .product-card:hover { background: #1a1714; }
  .product-icon { font-size: 2.8rem; margin-bottom: 14px; }
  .product-cat { font-size: 0.62rem; letter-spacing: 0.2em; text-transform: uppercase; color: #B87333; margin-bottom: 6px; }
  .product-name { font-size: 1.1rem; font-weight: 600; color: #fff; margin-bottom: 8px; }
  .product-desc { font-size: 0.78rem; color: rgba(255,255,255,0.45); line-height: 1.6; margin-bottom: 14px; }
  .product-tags { display: flex; flex-wrap: wrap; gap: 6px; margin-bottom: 16px; }
  .tag { font-size: 0.62rem; padding: 3px 8px; background: rgba(184,115,51,0.08); border: 1px solid rgba(184,115,51,0.2); color: rgba(255,255,255,0.5); border-radius: 1px; }
  .product-footer { display: flex; justify-content: space-between; align-items: center; padding-top: 14px; border-top: 1px solid rgba(184,115,51,0.1); }
  .moq { font-size: 0.68rem; color: rgba(255,255,255,0.3); }
 
  #process { background: #1a1714; }
  .process-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(160px, 1fr)); gap: 0; margin-top: 36px; }
  .step { padding: 24px 16px; text-align: center; border-right: 1px solid rgba(184,115,51,0.1); }
  .step:last-child { border-right: none; }
  .step-num { font-family: 'Bebas Neue', sans-serif; font-size: 0.75rem; letter-spacing: 0.2em; color: #B87333; margin-bottom: 12px; }
  .step-icon { font-size: 1.8rem; margin-bottom: 10px; }
  .step h4 { font-size: 0.9rem; font-weight: 600; color: #fff; margin-bottom: 6px; }
  .step p { font-size: 0.74rem; }
 
  #why { background: #111; }
  .why-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(200px, 1fr)); gap: 12px; margin-top: 32px; }
  .why-card { background: #1a1714; border: 1px solid rgba(184,115,51,0.1); border-radius: 4px; padding: 24px 20px; text-align: center; transition: border-color 0.2s, transform 0.2s; }
  .why-card:hover { border-color: rgba(184,115,51,0.4); transform: translateY(-3px); }
  .why-icon { font-size: 2rem; margin-bottom: 10px; }
  .why-card h4 { font-size: 0.9rem; font-weight: 600; margin-bottom: 6px; }
  .why-card p { font-size: 0.76rem; }
 
  #contact { background: #1a1714; display: grid; grid-template-columns: 1fr 1fr; gap: 60px; align-items: start; }
  .contact-item { display: flex; gap: 14px; margin-bottom: 20px; align-items: flex-start; }
  .contact-icon { width: 38px; height: 38px; border: 1px solid rgba(184,115,51,0.3); border-radius: 50%; display: flex; align-items: center; justify-content: center; font-size: 1rem; flex-shrink: 0; }
  .contact-label { font-size: 0.65rem; letter-spacing: 0.15em; text-transform: uppercase; color: #B87333; margin-bottom: 4px; }
  .contact-val { font-size: 0.88rem; color: rgba(255,255,255,0.65); }
  .contact-val a { color: inherit; text-decoration: none; }
  .contact-btns { display: flex; flex-direction: column; gap: 10px; margin-top: 24px; }
 
  .form-row { margin-bottom: 14px; }
  .form-row-2 { display: grid; grid-template-columns: 1fr 1fr; gap: 14px; margin-bottom: 14px; }
  label { display: block; font-size: 0.65rem; letter-spacing: 0.15em; text-transform: uppercase; color: rgba(255,255,255,0.45); margin-bottom: 6px; }
  input, select, textarea { width: 100%; background: #111; border: 1px solid rgba(184,115,51,0.2); border-radius: 2px; color: #fff; font-family: 'Inter', sans-serif; font-size: 0.88rem; padding: 10px 14px; outline: none; transition: border-color 0.2s; appearance: none; }
  input:focus, select:focus, textarea:focus { border-color: #B87333; }
  textarea { resize: vertical; min-height: 100px; }
  .form-submit { width: 100%; margin-top: 4px; font-size: 0.82rem; padding: 13px; }
  .form-note { font-size: 0.68rem; color: rgba(255,255,255,0.25); margin-top: 8px; text-align: center; }
 
  footer { background: #0a0a0a; border-top: 1px solid rgba(184,115,51,0.15); padding: 28px 40px; display: flex; justify-content: space-between; align-items: center; flex-wrap: wrap; gap: 16px; }
  .footer-logo { font-family: 'Bebas Neue', sans-serif; font-size: 1.4rem; letter-spacing: 0.1em; color: #D4A055; }
  .footer-logo span { color: #fff; }
  .footer-links { display: flex; gap: 20px; }
  .footer-links a { font-size: 0.72rem; letter-spacing: 0.1em; text-transform: uppercase; color: rgba(255,255,255,0.35); text-decoration: none; transition: color 0.2s; }
  .footer-links a:hover { color: #D4A055; }
  .footer-copy { font-size: 0.7rem; color: rgba(255,255,255,0.2); }
 
  @media (max-width: 768px) {
    nav { padding: 0 20px; }
    .nav-links a:not(.btn) { display: none; }
    .section { padding: 50px 20px; }
    #contact { grid-template-columns: 1fr; gap: 40px; padding: 50px 20px; }
    .form-row-2 { grid-template-columns: 1fr; gap: 0; }
    .step { border-right: none; border-bottom: 1px solid rgba(184,115,51,0.1); }
    footer { padding: 20px; flex-direction: column; align-items: flex-start; }
  }
</style>
</head>
<body>
 
<nav>
  <div class="logo">AMINE<span>HA</span></div>
  <div class="nav-links">
    <a href="#about">About</a>
    <a href="#products">Products</a>
    <a href="#process">Process</a>
    <a href="#contact">Contact</a>
    <a href="https://wa.me/919426260398?text=Hello%2C%20I%20want%20to%20request%20a%20quote" target="_blank" class="btn">Request Quote</a>
  </div>
</nav>
 
<div id="hero" class="section">
  <div class="label">Precision Brass Manufacturing</div>
  <h1>Premium <span>Brass</span><br>Parts & Components</h1>
  <p>High-quality brass inserts, fasteners, fittings and custom CNC parts for industrial and commercial applications. Reliable. Precise. Built to last.</p>
  <div class="hero-btns">
    <a href="#products" class="btn">Explore Products</a>
    <a href="https://wa.me/919426260398?text=Hello%2C%20I%20want%20to%20request%20a%20quote" target="_blank" class="btn btn-outline">💬 WhatsApp Quote</a>
  </div>
</div>
 
<div class="marquee">
  <div class="marquee-inner">
    <span>Brass Inserts ◆</span><span>CNC Machined Parts ◆</span><span>Brass Fittings ◆</span>
    <span>Electrical Components ◆</span><span>Precision Fasteners ◆</span><span>Custom Brass Parts ◆</span>
    <span>Thread Inserts ◆</span><span>Brass Screws ◆</span>
    <span>Brass Inserts ◆</span><span>CNC Machined Parts ◆</span><span>Brass Fittings ◆</span>
    <span>Electrical Components ◆</span><span>Precision Fasteners ◆</span><span>Custom Brass Parts ◆</span>
    <span>Thread Inserts ◆</span><span>Brass Screws ◆</span>
  </div>
</div>
 
<div id="about" class="section">
  <div class="label">About Amineha</div>
  <h2>Where <span>Precision</span> Meets Reliability</h2>
  <p style="max-width:560px; margin-top:10px;">Amineha is a specialist manufacturer of high-quality brass components, supplying industries from automotive and electronics to plumbing and construction.</p>
  <div class="about-grid">
    <div class="about-card"><div class="icon">🔬</div><h4>Precision Engineering</h4><p>Tolerances down to ±0.01mm on CNC machined parts.</p></div>
    <div class="about-card"><div class="icon">🏅</div><h4>Certified Quality</h4><p>ISO-compliant processes with full quality documentation.</p></div>
    <div class="about-card"><div class="icon">🔩</div><h4>Premium Materials</h4><p>Certified Brass C360, C260 and other grades for every application.</p></div>
    <div class="about-card"><div class="icon">💼</div><h4>B2B Focused</h4><p>Flexible MOQ and dedicated support for volume buyers.</p></div>
  </div>
</div>
 
<div id="products" class="section">
  <div class="label">Our Catalogue</div>
  <h2>Brass <span>Products</span></h2>
  <div class="tabs">
    <button class="tab active" onclick="filterP('all',this)">All</button>
    <button class="tab" onclick="filterP('inserts',this)">Inserts</button>
    <button class="tab" onclick="filterP('fasteners',this)">Fasteners</button>
    <button class="tab" onclick="filterP('fittings',this)">Fittings</button>
    <button class="tab" onclick="filterP('electrical',this)">Electrical</button>
    <button class="tab" onclick="filterP('cnc',this)">CNC Parts</button>
  </div>
  <div class="products-grid" id="grid"></div>
</div>
 
<div id="process" class="section">
  <div style="text-align:center">
    <div class="label" style="justify-content:center">How We Work</div>
    <h2>From <span>Inquiry</span> to Delivery</h2>
  </div>
  <div class="process-grid">
    <div class="step"><div class="step-num">01</div><div class="step-icon">📋</div><h4>Submit Inquiry</h4><p>Share requirements via form or WhatsApp.</p></div>
    <div class="step"><div class="step-num">02</div><div class="step-icon">💬</div><h4>Quotation</h4><p>We respond within 24 hours with a quote.</p></div>
    <div class="step"><div class="step-num">03</div><div class="step-icon">🔧</div><h4>Manufacturing</h4><p>Parts precision-machined with quality checks.</p></div>
    <div class="step"><div class="step-num">04</div><div class="step-icon">✅</div><h4>QC & Approval</h4><p>Dimensional inspection before shipment.</p></div>
    <div class="step"><div class="step-num">05</div><div class="step-icon">📦</div><h4>Delivery</h4><p>Securely packed and shipped worldwide.</p></div>
  </div>
</div>
 
<div id="why" class="section">
  <div style="text-align:center">
    <div class="label" style="justify-content:center">Why Choose Us</div>
    <h2>Trusted by <span>Industry Leaders</span></h2>
  </div>
  <div class="why-grid">
    <div class="why-card"><div class="why-icon">🏅</div><h4>ISO Certified</h4><p>International quality standards for consistency and reliability.</p></div>
    <div class="why-card"><div class="why-icon">🔩</div><h4>Premium Materials</h4><p>Certified Brass C360, C260 and other grades.</p></div>
    <div class="why-card"><div class="why-icon">📐</div><h4>Custom Engineering</h4><p>Fully custom parts from your drawings or samples.</p></div>
    <div class="why-card"><div class="why-icon">💼</div><h4>B2B Focused</h4><p>Competitive pricing and flexible MOQ for volume buyers.</p></div>
    <div class="why-card"><div class="why-icon">⚡</div><h4>Fast Response</h4><p>24-hour quote turnaround with dedicated support.</p></div>
  </div>
</div>
 
<div id="contact" class="section">
  <div>
    <div class="label">Get In Touch</div>
    <h2>Request a <span>Quote</span></h2>
    <p style="max-width:360px; margin: 10px 0 28px;">Tell us what you need and we'll get back within 24 hours.</p>
    <div class="contact-item">
      <div class="contact-icon">📧</div>
      <div><div class="contact-label">Email</div><div class="contact-val"><a href="mailto:virajharia2202@gmail.com">virajharia2202@gmail.com</a></div></div>
    </div>
    <div class="contact-item">
      <div class="contact-icon">📞</div>
      <div><div class="contact-label">Phone / WhatsApp</div><div class="contact-val">+91 9426260398</div></div>
    </div>
    <div class="contact-btns">
      <a href="tel:+917777914174" class="btn btn-outline">📞 Call Now</a>
      <a href="https://wa.me/919426260398?text=Hello%2C%20I%20want%20to%20enquire%20about%20brass%20products" target="_blank" class="btn btn-green">💬 Chat on WhatsApp</a>
    </div>
  </div>
  <div>
    <div class="form-row-2">
      <div><label>Full Name *</label><input id="f-name" type="text" placeholder="Your name"></div>
      <div><label>Company</label><input id="f-company" type="text" placeholder="Company name"></div>
    </div>
    <div class="form-row-2">
      <div><label>Email *</label><input id="f-email" type="email" placeholder="you@company.com"></div>
      <div><label>Phone</label><input id="f-phone" type="tel" placeholder="+91 00000 00000"></div>
    </div>
    <div class="form-row">
      <label>Product Category</label>
      <select id="f-cat">
        <option value="" disabled selected>Select a category</option>
        <option>Brass Inserts</option><option>Brass Fasteners</option>
        <option>Brass Fittings</option><option>Brass Electrical Parts</option>
        <option>CNC Brass Parts</option><option>Custom / Other</option>
      </select>
    </div>
    <div class="form-row">
      <label>Requirements *</label>
      <textarea id="f-msg" placeholder="Describe your requirements: quantity, size, material grade, application..."></textarea>
    </div>
    <button class="btn form-submit" onclick="sendWA()">Send via WhatsApp →</button>
    <p class="form-note">Opens WhatsApp with your inquiry pre-filled.</p>
  </div>
</div>
 
<footer>
  <div class="footer-logo">AMINE<span>HA</span></div>
  <div class="footer-links">
    <a href="#about">About</a><a href="#products">Products</a>
    <a href="#process">Process</a><a href="#contact">Contact</a>
  </div>
  <div class="footer-copy">© 2024 Amineha. All rights reserved.</div>
</footer>
 
<script>
const products = [
  {cat:'inserts',    icon:'🔩', name:'Threaded Brass Inserts',    desc:'Heat-set and ultrasonic threaded inserts for plastic molding. M2–M12 thread sizes.',       tags:['M2–M12','C360 Brass','DIN 16903'],    moq:'MOQ: 500 pcs'},
  {cat:'inserts',    icon:'⚙️', name:'Knurled Press-Fit Inserts',  desc:'Knurled body inserts for high torque resistance in thermoplastic assemblies.',             tags:['Metric/UNC','C360','Various lengths'], moq:'MOQ: 500 pcs'},
  {cat:'fasteners',  icon:'🔧', name:'Brass Machine Screws',       desc:'Precision turned brass screws in Phillips, slotted and hex socket drive.',                 tags:['M3–M10','C360 Brass','ISO 4762'],      moq:'MOQ: 1000 pcs'},
  {cat:'fasteners',  icon:'🔩', name:'Brass Hex Nuts',             desc:'Standard and nylon insert locking hex nuts in full brass.',                                 tags:['M4–M16','DIN 934','C360'],             moq:'MOQ: 1000 pcs'},
  {cat:'fittings',   icon:'🪛', name:'Brass Compression Fittings', desc:'Push-to-connect and compression fittings for gas, water and pneumatic lines.',             tags:['6mm–25mm','150 PSI','BSP/NPT'],        moq:'MOQ: 200 pcs'},
  {cat:'fittings',   icon:'🔗', name:'Brass Elbow Fittings',       desc:'90° and 45° elbow connectors for plumbing and HVAC systems.',                              tags:['1/4"–1" BSP','C260','ASTM B16'],       moq:'MOQ: 200 pcs'},
  {cat:'electrical', icon:'⚡', name:'Brass Electrical Terminals', desc:'Machined brass terminals for switchgear, panel boards and earthing systems.',              tags:['Custom sizes','C260/C360','IEC 60947'],moq:'MOQ: 500 pcs'},
  {cat:'electrical', icon:'🔌', name:'Brass Cable Glands',         desc:'IP68 rated brass cable glands for industrial and marine enclosures.',                      tags:['PG7–PG48','IP68','Nickel plated'],     moq:'MOQ: 100 pcs'},
  {cat:'cnc',        icon:'🏭', name:'Custom CNC Brass Parts',     desc:'Fully custom precision CNC turned and milled brass components from your drawings.',        tags:['Per drawing','C360/C260','±0.01mm'],   moq:'MOQ: 50 pcs'},
  {cat:'cnc',        icon:'🔄', name:'Brass Valve Bodies',         desc:'Precision machined valve bodies for fluid control applications.',                          tags:['1/4"–2"','C377 Brass','ASTM B283'],    moq:'MOQ: 50 pcs'},
];
 
function filterP(cat, el) {
  document.querySelectorAll('.tab').forEach(t => t.classList.remove('active'));
  el.classList.add('active');
  const list = cat === 'all' ? products : products.filter(p => p.cat === cat);
  document.getElementById('grid').innerHTML = list.map(p => `
    <div class="product-card">
      <div class="product-icon">${p.icon}</div>
      <div class="product-cat">${p.cat}</div>
      <div class="product-name">${p.name}</div>
      <div class="product-desc">${p.desc}</div>
      <div class="product-tags">${p.tags.map(t=>`<span class="tag">${t}</span>`).join('')}</div>
      <div class="product-footer">
        <span class="moq">${p.moq}</span>
        <a href="https://wa.me/919426260398?text=${encodeURIComponent('Hi, I am interested in: '+p.name)}" target="_blank" class="btn" style="padding:7px 14px;font-size:0.68rem;">Quote →</a>
      </div>
    </div>`).join('');
}
 
function sendWA() {
  const name = document.getElementById('f-name').value.trim();
  const company = document.getElementById('f-company').value.trim();
  const email = document.getElementById('f-email').value.trim();
  const phone = document.getElementById('f-phone').value.trim();
  const cat = document.getElementById('f-cat').value;
  const msg = document.getElementById('f-msg').value.trim();
  if (!name || !email || !msg) { alert('Please fill in Name, Email and Requirements.'); return; }
  const text = ['🔩 *New Quote Request — Amineha*','',`*Name:* ${name}`,company?`*Company:* ${company}`:'',`*Email:* ${email}`,phone?`*Phone:* ${phone}`:'',cat?`*Category:* ${cat}`:'','',`*Requirements:*\n${msg}`].filter(Boolean).join('\n');
  window.open('https://wa.me/919426260398?text='+encodeURIComponent(text),'_blank');
}
 
filterP('all', document.querySelector('.tab'));
</script>
</body>
</html>









