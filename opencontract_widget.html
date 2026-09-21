<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <script src="https://www.gstatic.com/antigravity/web/dev/tailwindcss.min.js"></script>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  <style>
    ::-webkit-scrollbar { width: 5px; height: 5px; }
    ::-webkit-scrollbar-thumb { background: rgba(150, 150, 150, 0.3); border-radius: 3px; }
  </style>
</head>
<body class="bg-transparent text-[var(--foreground)] antialiased p-2 sm:p-4">

  <div class="bg-[var(--card)] text-[var(--foreground)] border border-[var(--border)] rounded-2xl shadow-lg overflow-hidden max-w-2xl mx-auto">
    <!-- Header Banner -->
    <div class="bg-[#714B67] text-white p-3.5 px-4 flex items-center justify-between">
      <div class="flex items-center gap-2.5">
        <div class="w-8 h-8 rounded-lg bg-white/20 flex items-center justify-center font-bold text-sm">OC</div>
        <div>
          <div class="flex items-center gap-2">
            <h2 class="font-bold text-sm tracking-tight">OpenContract</h2>
            <span class="text-[10px] bg-white/20 px-1.5 py-0.5 rounded font-mono">v17.0 Community</span>
          </div>
          <p class="text-[11px] text-white/80">Contract Lifecycle &amp; Renewal Engine</p>
        </div>
      </div>
      <div class="flex items-center gap-2">
        <span class="text-[11px] bg-emerald-500/30 text-emerald-200 border border-emerald-400/40 px-2 py-0.5 rounded-full font-medium flex items-center gap-1">
          <span class="w-1.5 h-1.5 rounded-full bg-emerald-400 animate-pulse"></span>
          8/8 Tests Pass
        </span>
      </div>
    </div>

    <!-- KPI Quick Stats Row -->
    <div class="grid grid-cols-4 gap-2 p-3 bg-[var(--card)] border-b border-[var(--border)] text-center text-xs">
      <div class="p-2 rounded-lg bg-slate-500/5">
        <span class="text-[10px] uppercase font-bold text-[var(--muted-foreground)]">Total</span>
        <div class="text-base font-extrabold text-[var(--foreground)]">8</div>
      </div>
      <div class="p-2 rounded-lg bg-emerald-500/10">
        <span class="text-[10px] uppercase font-bold text-emerald-600">Active</span>
        <div class="text-base font-extrabold text-emerald-600">4</div>
      </div>
      <div class="p-2 rounded-lg bg-amber-500/10">
        <span class="text-[10px] uppercase font-bold text-amber-600">Expiring &le; 30d</span>
        <div class="text-base font-extrabold text-amber-600">2</div>
      </div>
      <div class="p-2 rounded-lg bg-purple-500/10">
        <span class="text-[10px] uppercase font-bold text-purple-600">Value</span>
        <div class="text-base font-extrabold text-purple-600">$348.5K</div>
      </div>
    </div>

    <!-- Navigation Tabs -->
    <div class="flex items-center justify-between px-3 pt-2.5 border-b border-[var(--border)] text-xs">
      <div class="flex space-x-1">
        <button onclick="setTab('contracts')" id="tab-btn-contracts" class="px-3 py-1.5 font-bold border-b-2 border-[#714B67] text-[#714B67]">Contracts (8)</button>
        <button onclick="setTab('lineage')" id="tab-btn-lineage" class="px-3 py-1.5 font-medium text-[var(--muted-foreground)] hover:text-[var(--foreground)]">Renewal Lineage</button>
        <button onclick="setTab('tests')" id="tab-btn-tests" class="px-3 py-1.5 font-medium text-[var(--muted-foreground)] hover:text-[var(--foreground)]">Test Logs</button>
      </div>
      <button onclick="simulateCron()" class="text-[11px] px-2 py-1 bg-slate-100 hover:bg-slate-200 dark:bg-slate-800 dark:hover:bg-slate-700 text-[var(--foreground)] rounded font-medium transition">
        <i class="fa fa-clock text-amber-500 mr-1"></i> Run Cron
      </button>
    </div>

    <!-- TAB 1: CONTRACTS LIST & DETAIL -->
    <div id="view-contracts" class="p-3 space-y-3">
      <!-- Filter Badges -->
      <div class="flex items-center gap-1.5 overflow-x-auto pb-1 text-[11px]">
        <button onclick="filterBy('all')" id="f-all" class="f-btn px-2.5 py-0.5 rounded-full font-bold bg-[#714B67] text-white">All</button>
        <button onclick="filterBy('active')" id="f-active" class="f-btn px-2.5 py-0.5 rounded-full font-semibold bg-slate-100 dark:bg-slate-800 text-[var(--muted-foreground)]">Active</button>
        <button onclick="filterBy('expiring')" id="f-expiring" class="f-btn px-2.5 py-0.5 rounded-full font-semibold bg-slate-100 dark:bg-slate-800 text-[var(--muted-foreground)]">Expiring &le; 30d</button>
        <button onclick="filterBy('pending')" id="f-pending" class="f-btn px-2.5 py-0.5 rounded-full font-semibold bg-slate-100 dark:bg-slate-800 text-[var(--muted-foreground)]">Pending</button>
        <button onclick="filterBy('renewed')" id="f-renewed" class="f-btn px-2.5 py-0.5 rounded-full font-semibold bg-slate-100 dark:bg-slate-800 text-[var(--muted-foreground)]">Renewed</button>
      </div>

      <!-- Contracts Scrollable List -->
      <div class="space-y-2 max-h-56 overflow-y-auto pr-1" id="contract-list">
        <!-- Rendered by JS -->
      </div>

      <!-- Selected Contract Detail Card -->
      <div id="selected-card" class="p-3 rounded-xl border border-[var(--border)] bg-slate-500/5 text-xs space-y-2">
        <!-- Injected by JS -->
      </div>
    </div>

    <!-- TAB 2: RENEWAL LINEAGE -->
    <div id="view-lineage" class="p-4 space-y-3 hidden text-xs">
      <div class="p-3 bg-purple-500/10 border border-purple-500/20 rounded-xl">
        <h3 class="font-bold text-purple-700 dark:text-purple-300 flex items-center gap-1.5">
          <i class="fa fa-history"></i> Lineage Chain Architecture (Zero Data Loss)
        </h3>
        <p class="text-[11px] text-[var(--muted-foreground)] mt-1">
          Contracts are legal records. When renewed, predecessor contracts are permanently locked in <strong>Renewed</strong> status, preserving their dates and values, while spawning a linked successor contract.
        </p>
      </div>

      <div class="flex items-center justify-center gap-3 p-3 bg-[var(--card)] border border-[var(--border)] rounded-xl">
        <!-- Predecessor -->
        <div class="p-2.5 rounded-lg border border-purple-300 dark:border-purple-800 bg-purple-50 dark:bg-purple-950/40 text-center flex-1">
          <span class="text-[9px] uppercase font-bold text-purple-600 dark:text-purple-400">Predecessor (Frozen)</span>
          <div class="font-mono font-bold text-xs mt-0.5">OC/2024/00004</div>
          <div class="text-[11px] font-semibold text-slate-700 dark:text-slate-300">Term 1 ($45,000)</div>
          <span class="inline-block mt-1 bg-purple-200 text-purple-800 dark:bg-purple-900 dark:text-purple-200 text-[9px] px-1.5 py-0.2 rounded font-bold">Renewed</span>
        </div>

        <div class="text-[#714B67] font-bold text-base flex flex-col items-center">
          <i class="fa fa-arrow-right"></i>
          <span class="text-[9px] text-slate-400">renews to</span>
        </div>

        <!-- Successor -->
        <div class="p-2.5 rounded-lg border-2 border-emerald-500 bg-emerald-50 dark:bg-emerald-950/40 text-center flex-1">
          <span class="text-[9px] uppercase font-bold text-emerald-600 dark:text-emerald-400">Successor (Current)</span>
          <div class="font-mono font-bold text-xs mt-0.5">OC/2025/00005</div>
          <div class="text-[11px] font-semibold text-slate-700 dark:text-slate-300">Term 2 ($52,000)</div>
          <span class="inline-block mt-1 bg-emerald-200 text-emerald-800 dark:bg-emerald-900 dark:text-emerald-200 text-[9px] px-1.5 py-0.2 rounded font-bold">Active</span>
        </div>
      </div>
    </div>

    <!-- TAB 3: TEST LOGS -->
    <div id="view-tests" class="p-4 space-y-3 hidden text-xs">
      <div class="flex items-center justify-between">
        <h3 class="font-bold text-xs flex items-center gap-1 text-emerald-600">
          <i class="fa fa-check-circle"></i> 8 Tests Passed in 0.02s
        </h3>
        <span class="text-[10px] text-[var(--muted-foreground)]">pytest opencontract/tests/run_tests.py</span>
      </div>

      <div class="space-y-1.5 max-h-52 overflow-y-auto font-mono text-[11px]">
        <div class="p-1.5 rounded bg-emerald-500/10 border border-emerald-500/20 flex justify-between">
          <span>&check; test_manifest_configuration</span><span class="text-emerald-600 font-bold">PASS</span>
        </div>
        <div class="p-1.5 rounded bg-emerald-500/10 border border-emerald-500/20 flex justify-between">
          <span>&check; test_xml_syntax_validity (15 files)</span><span class="text-emerald-600 font-bold">PASS</span>
        </div>
        <div class="p-1.5 rounded bg-emerald-500/10 border border-emerald-500/20 flex justify-between">
          <span>&check; test_acl_coverage (6 models)</span><span class="text-emerald-600 font-bold">PASS</span>
        </div>
        <div class="p-1.5 rounded bg-emerald-500/10 border border-emerald-500/20 flex justify-between">
          <span>&check; test_date_validations</span><span class="text-emerald-600 font-bold">PASS</span>
        </div>
        <div class="p-1.5 rounded bg-emerald-500/10 border border-emerald-500/20 flex justify-between">
          <span>&check; test_notice_deadline_validation</span><span class="text-emerald-600 font-bold">PASS</span>
        </div>
        <div class="p-1.5 rounded bg-emerald-500/10 border border-emerald-500/20 flex justify-between">
          <span>&check; test_days_to_expire_and_urgency</span><span class="text-emerald-600 font-bold">PASS</span>
        </div>
        <div class="p-1.5 rounded bg-emerald-500/10 border border-emerald-500/20 flex justify-between">
          <span>&check; test_renewal_lineage_chain</span><span class="text-emerald-600 font-bold">PASS</span>
        </div>
        <div class="p-1.5 rounded bg-emerald-500/10 border border-emerald-500/20 flex justify-between">
          <span>&check; test_cron_idempotency_simulation</span><span class="text-emerald-600 font-bold">PASS</span>
        </div>
      </div>
    </div>

    <!-- Notification Toast -->
    <div id="toast" class="hidden mx-3 mb-3 p-2 rounded bg-slate-900 text-white text-[11px] text-center">
      Notification message
    </div>
  </div>

  <script>
    const items = [
      { id: 1, ref: "OC/2025/00001", title: "Lead Systems Architect Agreement", party: "Mitchell Admin", type: "Permanent (PERM)", start: "2025-03-24", end: "2027-03-14", days: 540, value: "$120,000", state: "active" },
      { id: 2, ref: "OC/2025/00002", title: "Cloud Infrastructure SLA", party: "AWS Cloud Services", type: "Vendor (VENDOR)", start: "2025-10-10", end: "2026-10-10", days: 20, value: "$48,000", state: "active" },
      { id: 3, ref: "OC/2026/00003", title: "ISO 27001 Security Audit", party: "CyberTrust Group", type: "Consultant (CONS)", start: "2026-10-05", end: "2027-04-03", days: 195, value: "$25,000", state: "pending" },
      { id: 4, ref: "OC/2025/00003", title: "ERP Maintenance & Support", party: "OpenERP Solutions", type: "SLA (SERV)", start: "2025-09-25", end: "2026-09-25", days: 5, value: "$36,000", state: "expiring" },
      { id: 5, ref: "OC/2024/00004", title: "Marketing Strategy (Term 1)", party: "GrowthScale Media", type: "Fixed Term (FIXED)", start: "2024-09-20", end: "2025-09-19", days: -366, value: "$45,000", state: "renewed" },
      { id: 6, ref: "OC/2025/00005", title: "Marketing Strategy (Term 2)", party: "GrowthScale Media", type: "Fixed Term (FIXED)", start: "2025-09-20", end: "2026-09-21", days: 1, value: "$52,000", state: "active" },
      { id: 7, ref: "OC/2025/00006", title: "Engineering Internship", party: "Alex Rivers", type: "Internship (INTERN)", start: "2025-05-23", end: "2025-08-21", days: -30, value: "$4,500", state: "expired" },
      { id: 8, ref: "OC/2025/00007", title: "Mobile App Flutter Eng.", party: "AppDev Studio", type: "Freelance (FREE)", start: "2025-06-22", end: "2025-12-19", days: -90, value: "$18,000", state: "terminated" }
    ];

    let currentFilter = 'all';
    let selectedId = 2; // default to expiring cloud SLA

    function renderList() {
      const container = document.getElementById('contract-list');
      let filtered = items;
      if (currentFilter === 'active') filtered = items.filter(x => x.state === 'active');
      else if (currentFilter === 'expiring') filtered = items.filter(x => (x.state === 'active' && x.days <= 30) || x.state === 'expiring');
      else if (currentFilter === 'pending') filtered = items.filter(x => x.state === 'pending');
      else if (currentFilter === 'renewed') filtered = items.filter(x => x.state === 'renewed');

      container.innerHTML = filtered.map(c => {
        const isSelected = c.id === selectedId;
        let badge = '<span class="bg-emerald-100 text-emerald-800 text-[10px] px-1.5 py-0.5 rounded font-bold">Active</span>';
        if (c.days <= 30 && c.days > 0) badge = `<span class="bg-amber-100 text-amber-800 text-[10px] px-1.5 py-0.5 rounded font-bold">${c.days}d left</span>`;
        else if (c.state === 'pending') badge = '<span class="bg-blue-100 text-blue-800 text-[10px] px-1.5 py-0.5 rounded font-bold">Pending</span>';
        else if (c.state === 'renewed') badge = '<span class="bg-purple-100 text-purple-800 text-[10px] px-1.5 py-0.5 rounded font-bold">Renewed</span>';
        else if (c.state === 'expired' || c.state === 'terminated') badge = `<span class="bg-rose-100 text-rose-800 text-[10px] px-1.5 py-0.5 rounded font-bold">${c.state}</span>`;

        return `
          <div onclick="selectContract(${c.id})" class="p-2 rounded-lg border cursor-pointer transition flex items-center justify-between text-xs ${isSelected ? 'border-[#714B67] bg-[#714B67]/5' : 'border-[var(--border)] hover:bg-slate-50 dark:hover:bg-slate-800/50'}">
            <div>
              <div class="flex items-center gap-1.5">
                <span class="font-mono font-bold text-[#714B67] text-[11px]">${c.ref}</span>
                <span class="font-semibold text-[var(--foreground)] truncate max-w-[190px]">${c.title}</span>
              </div>
              <div class="text-[10px] text-[var(--muted-foreground)] mt-0.5">${c.party} &bull; ${c.value}</div>
            </div>
            <div>${badge}</div>
          </div>
        `;
      }).join('');

      renderSelected();
    }

    function renderSelected() {
      const c = items.find(x => x.id === selectedId) || items[0];
      const card = document.getElementById('selected-card');
      card.innerHTML = `
        <div class="flex items-start justify-between">
          <div>
            <span class="font-mono font-bold text-xs text-[#714B67]">${c.ref}</span>
            <h4 class="font-bold text-sm text-[var(--foreground)] mt-0.5">${c.title}</h4>
            <p class="text-[11px] text-[var(--muted-foreground)]">Party: <strong>${c.party}</strong> &bull; Type: <strong>${c.type}</strong></p>
          </div>
          <span class="font-bold text-sm text-emerald-600">${c.value}</span>
        </div>
        <div class="grid grid-cols-2 gap-2 text-[11px] pt-1.5 border-t border-[var(--border)]">
          <div><span class="text-[var(--muted-foreground)]">Duration:</span> ${c.start} &rarr; ${c.end}</div>
          <div><span class="text-[var(--muted-foreground)]">Manager:</span> Mitchell Admin</div>
        </div>
        <div class="flex items-center gap-2 pt-1">
          <button onclick="showToast('Renewal wizard launched for ${c.ref}')" class="px-2.5 py-1 bg-[#714B67] hover:bg-[#5a3b52] text-white rounded text-[11px] font-semibold">
            <i class="fa fa-refresh mr-1"></i> Renew Contract
          </button>
          <button onclick="showToast('Contract summary dossier generated')" class="px-2.5 py-1 border border-[var(--border)] hover:bg-slate-100 dark:hover:bg-slate-800 rounded text-[11px] font-semibold">
            <i class="fa fa-file-pdf mr-1 text-rose-500"></i> Export PDF
          </button>
        </div>
      `;
    }

    function selectContract(id) {
      selectedId = id;
      renderList();
    }

    function filterBy(filter) {
      currentFilter = filter;
      document.querySelectorAll('.f-btn').forEach(b => {
        b.classList.remove('bg-[#714B67]', 'text-white');
        b.classList.add('bg-slate-100', 'text-[var(--muted-foreground)]');
      });
      document.getElementById('f-' + filter).classList.add('bg-[#714B67]', 'text-white');
      document.getElementById('f-' + filter).classList.remove('bg-slate-100', 'text-[var(--muted-foreground)]');
      renderList();
    }

    function setTab(tab) {
      document.getElementById('view-contracts').classList.toggle('hidden', tab !== 'contracts');
      document.getElementById('view-lineage').classList.toggle('hidden', tab !== 'lineage');
      document.getElementById('view-tests').classList.toggle('hidden', tab !== 'tests');

      ['contracts', 'lineage', 'tests'].forEach(t => {
        const btn = document.getElementById('tab-btn-' + t);
        if (t === tab) {
          btn.className = "px-3 py-1.5 font-bold border-b-2 border-[#714B67] text-[#714B67]";
        } else {
          btn.className = "px-3 py-1.5 font-medium text-[var(--muted-foreground)] hover:text-[var(--foreground)]";
        }
      });
    }

    function simulateCron() {
      showToast("&check; Expiry Cron: 1 contract expired, 2 activity alerts scheduled (deduplicated).");
    }

    function showToast(msg) {
      const t = document.getElementById('toast');
      t.innerHTML = msg;
      t.classList.remove('hidden');
      setTimeout(() => t.classList.add('hidden'), 3500);
    }

    // Init
    renderList();
  </script>
</body>
</html>
