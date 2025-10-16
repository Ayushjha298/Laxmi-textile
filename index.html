<!doctype html>

<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Laxmi Textile — Inventory & Customization</title>
  <style>
    :root{--bg:#f7f8fb;--sidebar:#0f1724;--accent:#0b71ea;--card:#ffffff;--muted:#6b7280;--success:#16a34a;--danger:#dc2626}
    html,body{height:100%;margin:0;font-family:Inter, system-ui, Arial;background:var(--bg);color:#0f1724}
    .app{display:flex;min-height:100vh}
    nav{width:260px;background:var(--sidebar);color:#fff;padding:18px;box-sizing:border-box}
    nav .brand{display:flex;align-items:center;gap:10px;margin-bottom:18px}
    nav h1{font-size:18px;margin:0;color:#fde68a}
    nav .navbtn{display:flex;align-items:center;gap:10px;padding:12px;border-radius:8px;background:transparent;border:none;color:#fff;width:100%;text-align:left;cursor:pointer;font-size:16px}
    nav .navbtn:hover{background:rgba(255,255,255,0.04)}
    main{flex:1;padding:18px;overflow:auto}
    .grid{display:grid;grid-template-columns:1fr 350px;gap:16px}
    .card{background:var(--card);padding:14px;border-radius:12px;box-shadow:0 6px 18px rgba(16,24,40,.04)}
    .row{display:flex;gap:8px;align-items:center;margin-bottom:8px}
    input[type=text], input[type=number], select, textarea{padding:10px;border-radius:8px;border:1px solid #e6e6e6;font-size:15px;width:100%;box-sizing:border-box}
    button.btn{background:var(--accent);color:#fff;border:none;padding:10px 12px;border-radius:8px;cursor:pointer}
    button.ghost{background:#fff;border:1px solid #e5e7eb;color:#111}
    .small{font-size:13px;color:var(--muted)}
    .dashboard-tiles{display:flex;gap:10px}
    .tile{flex:1;padding:12px;border-radius:10px;background:linear-gradient(180deg,#fff,#f1f9ff);text-align:left}
    .tile .num{font-size:22px;font-weight:800}
    .list{max-height:420px;overflow:auto}
    .alerts .alert{padding:10px;border-radius:8px;background:rgba(220,38,38,0.06);color:var(--danger);margin-bottom:8px}
    .ok{padding:8px;border-radius:8px;background:rgba(16,185,129,0.06);color:var(--success)}/* Report table clearer colors */
table{width:100%;border-collapse:collapse}
th,td{padding:10px;border-bottom:1px solid #eef2ff;text-align:left}
th{background:#0b5ed7;color:#fff}
tr:nth-child(even){background:#e6f0ff}

/* customization queue list */
.job{padding:10px;border-radius:8px;border:1px solid #eef2ff;margin-bottom:8px;background:#fff}
.job .meta{display:flex;justify-content:space-between;align-items:center}
.job .badges{display:flex;gap:6px}
.badge{padding:4px 8px;border-radius:999px;font-size:12px;background:#eef2ff;color:#0b5ed7}

/* toast */
.toast{position:fixed;right:18px;top:18px;background:#111;color:#fff;padding:12px 14px;border-radius:10px;box-shadow:0 8px 30px rgba(2,6,23,.3);display:none;z-index:9999}

/* responsive */
@media (max-width:900px){
  nav{position:fixed;left:0;top:0;height:100vh;width:64px;padding:12px;align-items:center}
  nav h1{display:none}
  nav .navbtn{font-size:0;padding:10px}
  nav .navbtn span{display:none}
  main{padding:12px;margin-left:64px}
  .grid{grid-template-columns:1fr}
}

  </style>
</head>
<body>
  <div class="app" role="application">
    <nav aria-label="Main navigation">
      <div class="brand"><div style="width:36px;height:36;border-radius:8px;background:#fff;display:flex;align-items:center;justify-content:center;color:#0b71ea;font-weight:800">L</div><h1>Laxmi Textile</h1></div>
      <button class="navbtn" onclick="showSection('dashboard')">🏠 <span>Dashboard</span></button>
      <button class="navbtn" onclick="showSection('addStock')">➕ <span>Add / Receive Stock</span></button>
      <button class="navbtn" onclick="showSection('sellProduct')">💳 <span>Sell Product</span></button>
      <button class="navbtn" onclick="showSection('orders')">📦 <span>Orders</span></button>
      <button class="navbtn" onclick="showSection('custom')">🪡 <span>Customization</span></button>
      <button class="navbtn" onclick="showSection('reports')">📊 <span>Reports</span></button>
    </nav><main>
  <div id="toast" class="toast" role="status" aria-live="polite"></div>

  <section id="dashboard" class="card">
    <div style="display:flex;justify-content:space-between;align-items:center">
      <div>
        <div class="small">Dashboard</div>
        <h2 style="margin:6px 0">Real-time overview (Inventory + Customization)</h2>
      </div>
      <div class="small">Updated: <span id="lastUpdated">-</span></div>
    </div>

    <div style="margin-top:12px" class="dashboard-tiles">
      <div class="tile"><div class="small">Total Products</div><div class="num" id="totalProducts">0</div></div>
      <div class="tile"><div class="small">Total Stock</div><div class="num" id="totalStock">0</div></div>
      <div class="tile"><div class="small">Today's Sales</div><div class="num" id="todaySales">₹0</div></div>
    </div>

    <div style="margin-top:12px;display:flex;gap:12px;flex-wrap:wrap">
      <div class="card" style="flex:1;min-width:260px">
        <div class="small">Active Customization Queue</div>
        <div id="queue" style="margin-top:8px"></div>
        <div style="margin-top:8px" class="small">Queue length: <span id="queueLen">0</span> • Est. wait: <span id="estWait">0 min</span></div>
      </div>

      <div class="card" style="width:320px">
        <div class="small">Recent Orders / Jobs</div>
        <div id="dashRecent" style="margin-top:8px"></div>
      </div>
    </div>
  </section>

  <div class="grid" style="margin-top:12px">
    <div>
      <section id="addStock" class="card" style="display:none">
        <h3>Add / Receive Stock</h3>
        <div class="small">Quick add with friendly UI</div>
        <div style="margin-top:10px">
          <div class="row"><input id="pName" type="text" placeholder="Product name (e.g. Red Saree)" /></div>
          <div class="row"><input id="pCat" type="text" placeholder="Category (e.g. Saree)" /></div>
          <div class="row"><input id="pQty" type="number" min="1" placeholder="Quantity" /></div>
          <div class="row"><input id="pPrice" type="number" min="0" placeholder="Price per unit" /></div>
          <div class="row"><input id="pLocation" type="text" placeholder="Storage location (Rack A)" /></div>
          <div style="display:flex;gap:8px;margin-top:8px"><button class="btn" onclick="handleAddStock()">Add Stock</button><button class="ghost" onclick="clearAddForm()">Clear</button></div>
        </div>
      </section>

      <section id="sellProduct" class="card" style="display:none">
        <h3>Sell Product</h3>
        <div class="small">Select product from inventory</div>
        <div style="margin-top:10px">
          <div class="row"><select id="sellSelect"><option value="">-- Select product --</option></select></div>
          <div class="row"><input id="sellQty" type="number" min="1" placeholder="Quantity to sell" /></div>
          <div class="row"><input id="sellBuyer" type="text" placeholder="Customer (optional)" /></div>
          <div style="display:flex;gap:8px;margin-top:8px"><button class="btn" onclick="handleSell()">Sell</button><button class="ghost" onclick="clearSellForm()">Clear</button></div>
        </div>
      </section>

      <section id="orders" class="card" style="display:none">
        <h3>Place Order</h3>
        <div class="small">Only existing inventory items can be ordered</div>
        <div style="margin-top:10px">
          <div class="row"><select id="orderSelect"><option value="">-- Select product --</option></select></div>
          <div class="row"><input id="orderQty" type="number" min="1" placeholder="Quantity to order" /></div>
          <div class="row"><input id="orderEta" type="text" placeholder="ETA (optional)" /></div>
          <div style="display:flex;gap:8px;margin-top:8px"><button class="btn" onclick="handleOrder()">Place Order</button><button class="ghost" onclick="clearOrderForm()">Clear</button></div>
        </div>
      </section>

      <section id="custom" class="card" style="display:none">
        <h3>Customization — New Job</h3>
        <div class="small">Create a customization job for a customer (in-store)</div>
        <div style="margin-top:10px">
          <div class="row"><input id="jobCustomer" type="text" placeholder="Customer name" /></div>
          <div class="row"><select id="jobProduct"><option value="">-- Select product (or choose new) --</option></select></div>
          <div class="row"><select id="jobType"><option value="pattern">Pattern</option><option value="border">Border</option><option value="embroidery">Embroidery</option><option value="tailoring">Tailoring</option></select></div>
          <div class="row"><input id="jobDetails" type="text" placeholder="Details (colors, size, notes)" /></div>
          <div class="row"><input id="jobEstMins" type="number" min="5" placeholder="Estimated time (minutes)" /></div>
          <div class="row"><select id="assignTailor"><option value="">-- Assign tailor (optional) --</option></select></div>
          <div style="display:flex;gap:8px;margin-top:8px"><button class="btn" onclick="createJob()">Create Job</button><button class="ghost" onclick="clearJobForm()">Clear</button></div>
        </div>

        <hr style="margin:12px 0" />
        <h4>Active Jobs (in this device)</h4>
        <div id="jobList" style="margin-top:8px"></div>
      </section>

      <section id="reports" class="card" style="display:none">
        <h3>Reports (Today)</h3>
        <div class="small">Shows today's inventory & customization activity</div>
        <div style="margin-top:10px">
          <h4>Inventory Snapshot</h4>
          <table aria-live="polite"><thead><tr><th>Product</th><th>Qty</th><th>Price</th></tr></thead><tbody id="reportTable"></tbody></table>

          <h4 style="margin-top:12px">Today's Activity</h4>
          <table><thead><tr><th>Type</th><th>Product / Job</th><th>Qty</th><th>Value</th></tr></thead><tbody id="activityTable"></tbody></table>
        </div>
      </section>
    </div>

    <aside>
      <div class="card">
        <div class="small">Inventory List</div>
        <div class="list" style="margin-top:8px"><table><thead><tr><th>Product</th><th>Cat</th><th>Qty</th><th>Price</th></tr></thead><tbody id="inventoryBody"></tbody></table></div>
      </div>

      <div class="card" style="margin-top:12px">
        <div class="small">Tailors (Manage)</div>
        <div style="margin-top:8px"><div id="tailorList"></div><div style="margin-top:8px"><input id="newTailor" placeholder="New tailor name" /><button class="btn" onclick="addTailor()">Add</button></div></div>
      </div>
    </aside>
  </div>
</main>

  </div>  <script>
    const KEY = 'laxmi_inventory_v2';
    const defaultState = { products:[], sales:[], orders:[], jobs:[], tailors:[] };
    function load(){ try{ return JSON.parse(localStorage.getItem(KEY))||structuredClone(defaultState) }catch(e){return structuredClone(defaultState)} }
    function save(s){ localStorage.setItem(KEY, JSON.stringify(s)); }
    let state = load();

    // helpers
    function now(){ return new Date(); }
    function iso(d=new Date()){ return d.toISOString(); }
    function todayString(d=new Date()){ return d.toDateString(); }
    function toast(msg){ const t=document.getElementById('toast'); t.textContent=msg; t.style.display='block'; setTimeout(()=>t.style.display='none',3000); }

    // UI navigation
    function showSection(id){ document.querySelectorAll('main section').forEach(s=>s.style.display='none'); document.getElementById(id).style.display='block'; if(id==='sellProduct' || id==='orders' || id==='custom') populateSelects(); if(id==='dashboard') updateUI(); }

    // seed
    if(state.products.length===0){ state.products.push({id:1,name:'Red Saree',category:'Saree',qty:12,price:499,location:'Rack A',history:[]}); state.products.push({id:2,name:'Cotton Kurta',category:'Kurta',qty:8,price:699,location:'Rack B',history:[]}); save(state); }

    // populate selects
    function populateSelects(){ const sell = document.getElementById('sellSelect'); const orderSel = document.getElementById('orderSelect'); const jobProd = document.getElementById('jobProduct'); const assign = document.getElementById('assignTailor'); sell.innerHTML='<option value="">-- Select product --</option>'; orderSel.innerHTML=sell.innerHTML; jobProd.innerHTML='<option value="">-- Select product (or new) --</option>'; assign.innerHTML='<option value="">-- Assign tailor (optional) --</option>';
      state.products.forEach(p=>{ const opt=`<option value="${p.id}">${p.name} — ${p.qty} left</option>`; sell.insertAdjacentHTML('beforeend',opt); orderSel.insertAdjacentHTML('beforeend',opt); jobProd.insertAdjacentHTML('beforeend',opt); });
      state.tailors.forEach(t=> assign.insertAdjacentHTML('beforeend', `<option value="${t.id}">${t.name}</option>`)); renderTailors(); }

    function renderTailors(){ const el=document.getElementById('tailorList'); el.innerHTML = state.tailors.map(t=>`<div style="padding:8px;border-bottom:1px solid #f2f4f7">${t.name} <small class="small">(${t.activeJobs||0} jobs)</small> <button class="ghost" onclick="removeTailor(${t.id})">Remove</button></div>`).join('')||'<div class="small">No tailors</div>'; }

    function addTailor(){ const name=document.getElementById('newTailor').value.trim(); if(!name) return alert('Enter name'); const t={id:Date.now(),name,activeJobs:0}; state.tailors.push(t); save(state); document.getElementById('newTailor').value=''; populateSelects(); toast('Tailor added'); }
    function removeTailor(id){ state.tailors = state.tailors.filter(t=>t.id!==id); save(state); populateSelects(); }

    // stock functions
    function handleAddStock(){ const name=document.getElementById('pName').value.trim(); const cat=document.getElementById('pCat').value.trim()||'general'; const qty=parseInt(document.getElementById('pQty').value)||0; const price=parseFloat(document.getElementById('pPrice').value)||0; const loc=document.getElementById('pLocation').value.trim(); if(!name||qty<=0){ return alert('Enter name and qty'); }
      let prod = state.products.find(p=>p.name.toLowerCase()===name.toLowerCase()); if(!prod){ prod={id:Date.now(),name,category:cat,qty:0,price:price||0,location:loc,history:[]}; state.products.push(prod);} prod.qty += qty; prod.price = price||prod.price; prod.history = prod.history||[]; prod.history.push({type:'received',when:iso(),qty,price,location:loc}); state.orders.push({id:Date.now(),type:'received',when:iso(),product:prod.name,qty,price,location:loc}); save(state); toast(`${qty} ${prod.name} added`); clearAddForm(); populateSelects(); showSection('dashboard'); updateUI(); }
    function clearAddForm(){ ['pName','pCat','pQty','pPrice','pLocation'].forEach(id=>document.getElementById(id).value=''); }

    function handleSell(){ const id = parseInt(document.getElementById('sellSelect').value); const qty = parseInt(document.getElementById('sellQty').value)||0; const buyer = document.getElementById('sellBuyer').value.trim(); if(!id||qty<=0){ return alert('Select product and qty'); }
      const prod = state.products.find(p=>p.id===id); if(!prod){ return alert('Product not found'); }
      if(prod.qty < qty){ return alert('Not enough stock'); }
      prod.qty -= qty; prod.history = prod.history||[]; prod.history.push({type:'sold',when:iso(),qty,price:prod.price,buyer}); state.sales.push({id:Date.now(),when:iso(),product:prod.name,qty,price:prod.price,buyer}); save(state); toast(`${qty} ${prod.name} sold`); clearSellForm(); populateSelects(); showSection('dashboard'); updateUI(); }
    function clearSellForm(){ ['sellSelect','sellQty','sellBuyer'].forEach(id=>document.getElementById(id).value=''); }

    function handleOrder(){ const id = parseInt(document.getElementById('orderSelect').value); const qty = parseInt(document.getElementById('orderQty').value)||0; const eta = document.getElementById('orderEta').value.trim(); if(!id||qty<=0) return alert('Select product and qty'); const prod = state.products.find(p=>p.id===id); if(!prod) return alert('Product not in inventory—cannot place order'); state.orders.push({id:Date.now(),type:'order',when:iso(),product:prod.name,qty,eta}); save(state); toast(`Order placed: ${qty} ${prod.name}`); clearOrderForm(); showSection('dashboard'); updateUI(); }
    function clearOrderForm(){ ['orderSelect','orderQty','orderEta'].forEach(id=>document.getElementById(id).value=''); }

    // customization jobs
    function createJob(){ const customer=document.getElementById('jobCustomer').value.trim()||'Walk-in'; const prodId = document.getElementById('jobProduct').value; const prodName = prodId? (state.products.find(p=>p.id==prodId)||{}).name : document.getElementById('jobProduct').querySelector('option:checked')?.textContent || 'Custom'; const type=document.getElementById('jobType').value; const details=document.getElementById('jobDetails').value.trim(); const est = parseInt(document.getElementById('jobEstMins').value)||30; const tailorId = document.getElementById('assignTailor').value||null; // job allowed only if product exists in inventory or customer provided
      if(!prodName) return alert('Select or enter product'); const job = { id:Date.now(),customer,product:prodName,type,details,estMins:est,status:'pending',created:iso(),tailorId:tailorId?parseInt(tailorId):null,started:null,completed:null };
      state.jobs.push(job); save(state); toast('Customization job created'); clearJobForm(); populateSelects(); showSection('dashboard'); updateUI(); }

    function clearJobForm(){ ['jobCustomer','jobDetails','jobEstMins'].forEach(id=>document.getElementById(id).value=''); document.getElementById('jobProduct').value=''; document.getElementById('assignTailor').value=''; }

    // job controls
    function startJob(id){ const job = state.jobs.find(j=>j.id===id); if(!job) return; job.status='in-progress'; job.started=iso(); if(job.tailorId){ const t=state.tailors.find(x=>x.id===job.tailorId); if(t) t.activeJobs=(t.activeJobs||0)+1; } save(state); toast(`Started job ${job.product}`); updateUI(); }
    function completeJob(id){ const job = state.jobs.find(j=>j.id===id); if(!job) return; job.status='completed'; job.completed=iso(); // free tailor count
      if(job.tailorId){ const t=state.tailors.find(x=>x.id===job.tailorId); if(t) t.activeJobs=Math.max(0,(t.activeJobs||1)-1); }
      save(state); toast(`Completed job ${job.product}`); updateUI(); }
    function cancelJob(id){ state.jobs = state.jobs.map(j=> j.id===id?{...j,status:'cancelled',completed:iso()}:j); save(state); toast('Job cancelled'); updateUI(); }

    // queue metrics
    function queueMetrics(){ const q = state.jobs.filter(j=>j.status==='pending'); const len = q.length; // estimate wait as sum of estMins of pending / number of tailors (if any)
      const tailors = Math.max(1,state.tailors.length); const totalMins = q.reduce((s,j)=>s+(j.estMins||30),0); const est = Math.round(totalMins / tailors); return {len,est}; }

    // render queue and jobs
    function renderJobs(){ const qEl=document.getElementById('queue'); const jobs = state.jobs.filter(j=> j.status==='pending' || j.status==='in-progress').sort((a,b)=>a.created-b.created);
      qEl.innerHTML = jobs.map(j=>{
        const tName = j.tailorId? (state.tailors.find(t=>t.id===j.tailorId)?.name||'') : '';
        const actions = j.status==='pending' ? `<button class="btn" onclick="startJob(${j.id})">Start</button> <button class="ghost" onclick="cancelJob(${j.id})">Cancel</button>` : `<button class="btn" onclick="completeJob(${j.id})">Complete</button>`;
        return `<div class="job"><div class="meta"><div><strong>${j.product}</strong> <div class="small">${j.customer} • ${j.type}</div></div><div class="badges"><div class="badge">${j.status}</div>${tName?`<div class="badge">${tName}</div>`:''}</div></div><div style="margin-top:8px" class="small">${j.details || ''} • Est: ${j.estMins} min</div><div style="margin-top:8px">${actions}</div></div>`;
      }).join('')||'<div class="small">No active jobs</div>';
      document.getElementById('queueLen').textContent = queueMetrics().len; document.getElementById('estWait').textContent = queueMetrics().est + ' min';

      // job list in custom page
      const jobList = document.getElementById('jobList'); if(jobList) jobList.innerHTML = state.jobs.slice().reverse().map(j=>`<div class="job"><div class="meta"><div><strong>${j.product}</strong><div class="small">${j.customer} • ${j.type} • ${new Date(j.created).toLocaleString()}</div></div><div class="badges"><div class="badge">${j.status}</div></div></div><div style="margin-top:8px" class="small">${j.details||''}</div></div>`).join('')||'<div class="small">No jobs</div>';
    }

    // recent orders/jobs for dashboard
    function renderRecent(){ const el=document.getElementById('dashRecent'); const items = [...state.orders.slice(-6).reverse().map(o=>({t:o.when,html:`<div style=\"padding:8px;border-bottom:1px solid #f3f4f6\"><strong>${o.product}</strong> <div class=\"small\">order • ${o.qty} • ${new Date(o.when).toLocaleString()}</div></div>`})), ...state.jobs.slice(-6).reverse().map(j=>({t:j.created,html:`<div style=\"padding:8px;border-bottom:1px solid #f3f4f6\"><strong>${j.product}</strong> <div class=\"small\">job • ${j.customer} • ${j.status}</div></div>`}))]; el.innerHTML = items.map(i=>i.html).join('')||'<div class="small">No recent activity</div>' }

    // reports
    function generateReport(){ const report = document.getElementById('reportTable'); report.innerHTML = state.products.map(p=>`<tr><td>${p.name}</td><td>${p.qty}</td><td>₹${p.price}</td></tr>`).join('')||'<tr><td colspan="3">No items</td></tr>';
      const act = document.getElementById('activityTable'); const today = todayString(); const activities = [];
      state.sales.filter(s=> new Date(s.when).toDateString()===today).forEach(s=> activities.push({type:'sale',product:s.product,qty:s.qty,value:s.price*s.qty}));
      state.orders.filter(o=> new Date(o.when).toDateString()===today).forEach(o=> activities.push({type:o.type,product:o.product,qty:o.qty,value:(o.price?o.price*o.qty:0)}));
      state.jobs.filter(j=> new Date(j.created).toDateString()===today).forEach(j=> activities.push({type:'job',product:j.product,qty:1,value:0}));
      if(activities.length===0) act.innerHTML = '<tr><td colspan="4">No activity today</td></tr>'; else act.innerHTML = activities.map(a=>`<tr><td>${a.type}</td><td>${a.product}</td><td>${a.qty}</td><td>₹${(a.value||0).toFixed(2)}</td></tr>`).join(''); }

    // dashboard update
    function updateUI(){ document.getElementById('lastUpdated').textContent = (new Date()).toLocaleString(); // inventory
      const inv = document.getElementById('inventoryBody'); inv.innerHTML = state.products.map(p=>`<tr><td>${p.name}</td><td>${p.category}</td><td>${p.qty}</td><td>₹${p.price}</td></tr>`).join('') || '<tr><td colspan="4">No items</td></tr>';
      document.getElementById('totalProducts').textContent = state.products.length;
      document.getElementById('totalStock').textContent = state.products.reduce((s,p)=>s+p.qty,0);
      const today = todayString(); const todaysales = state.sales.filter(s=> new Date(s.when).toDateString()===today);
      const salesAmt = todaysales.reduce((sum,s)=> sum + (s.price*s.qty), 0);
      document.getElementById('todaySales').textContent = '₹' + salesAmt.toFixed(2);

      // alerts
      const low = state.products.filter(p=>p.qty<=5);
      const alerts = document.getElementById('alerts'); alerts.innerHTML = low.length? low.map(p=>`<div class="alert"><b>${p.name}</b> — ${p.qty} left</div>`).join('') : '<div class="ok">No low stock</div>';

      renderJobs(); renderRecent(); generateReport(); populateSelects(); }

    // simulate real-time processing: auto-start pending jobs if tailors available
    setInterval(()=>{
      // find pending jobs and free tailors
      const pending = state.jobs.filter(j=>j.status==='pending');
      if(pending.length>0 && state.tailors.length>0){ // assign to idle tailors and start
        const idleTailors = state.tailors.filter(t=> (t.activeJobs||0) < 2); // each tailor can handle 2 concurrently
        if(idleTailors.length>0){ const job = pending[0]; const tailor = idleTailors[0]; job.tailorId = tailor.id; job.status='in-progress'; job.started=iso(); tailor.activeJobs=(tailor.activeJobs||0)+1; save(state); toast(`Job ${job.product} started by ${tailor.name}`); updateUI(); }
      }
    }, 5000);

    // initial render
    populateSelects(); updateUI(); showSection('dashboard');

    // expose
    window.Laxmi = { state, saveState: ()=>save(state), createJob, startJob, completeJob };
  </script></body>
</html>
