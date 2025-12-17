<!DOCTYPE html><html lang="pt-BR">
<head>
<meta charset="UTF-8">
<title>Nyscolar Online</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
<script src="https://cdn.jsdelivr.net/npm/qrcodejs/qrcode.min.js"></script>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
<style>
*{box-sizing:border-box}
body{margin:0;font-family:'Poppins',sans-serif;min-height:100vh;background:linear-gradient(135deg,#0f2027,#203a43,#2c5364);color:#fff}
.hidden{display:none}
.center{display:flex;align-items:center;justify-content:center;height:100vh}
.card{background:rgba(255,255,255,.12);backdrop-filter:blur(18px);border-radius:22px;padding:25px;margin:15px;box-shadow:0 15px 40px rgba(0,0,0,.35)}
h2,h3{margin-top:0}
input,select{width:100%;padding:12px;border:none;border-radius:14px;margin:6px 0;font-family:'Poppins'}
button{padding:12px 18px;border:none;border-radius:14px;background:linear-gradient(135deg,#00c6ff,#0072ff);color:#fff;font-weight:600;cursor:pointer;transition:.3s}
button:hover{transform:translateY(-2px);box-shadow:0 8px 20px rgba(0,0,0,.35)}
nav{display:flex;flex-wrap:wrap;gap:10px}
nav button{background:linear-gradient(135deg,#667eea,#764ba2)}
table{width:100%;border-collapse:collapse;margin-top:10px}
th,td{padding:8px;border-bottom:1px solid rgba(255,255,255,.2);text-align:left}
.alert{color:#ff6b6b;font-weight:600}
</style>
</head>
<body><!-- LOGIN --><div id="login" class="center">
  <div class="card" style="max-width:380px;width:100%">
    <h2>🔐 Nyscolar Online</h2>
    <input id="matricula" placeholder="Matrícula">
    <input id="senha" type="password" placeholder="Senha">
    <button type="button" id="btnLogin">Entrar</button>
  </div>
</div><!-- GESTOR --><div id="gestor" class="hidden">
  <nav class="card">
    <button onclick="show('g-dashboard')">Dashboard</button>
    <button onclick="show('g-alunos')">Alunos</button>
    <button onclick="show('g-professores')">Professores</button>
    <button onclick="show('g-horarios')">Horários</button>
    <button onclick="logout()">Sair</button>
  </nav>  <div id="g-dashboard" class="card hidden">
    <h3>📊 Dashboard Geral</h3>
    <canvas id="grafico"></canvas>
  </div>  <div id="g-alunos" class="card hidden">
    <h3>🎓 Cadastro de Aluno</h3>
    <input id="alunoNome" placeholder="Nome do aluno">
    <button onclick="addAluno()">Cadastrar</button>
    <div id="listaAlunos"></div>
  </div>  <div id="g-professores" class="card hidden">
    <h3>👨‍🏫 Cadastro de Professor</h3>
    <input id="profNome" placeholder="Nome">
    <input id="profDisc" placeholder="Disciplina">
    <button onclick="addProfessor()">Cadastrar</button>
    <div id="listaProf"></div>
  </div>  <div id="g-horarios" class="card hidden">
    <h3>📅 Cadastro de Horários</h3>
    <select id="hProf"></select>
    <input id="hDisc" placeholder="Disciplina">
    <input id="hDia" placeholder="Dia da semana">
    <input id="hHora" placeholder="Horário">
    <button onclick="addHorario()">Salvar</button>
    <div id="listaHorarios"></div>
  </div>
</div><!-- PROFESSOR --><div id="professor" class="hidden">
  <nav class="card">
    <button onclick="show('p-diario')">Diário</button>
    <button onclick="show('p-alertas')">Alertas</button>
    <button onclick="logout()">Sair</button>
  </nav>  <div id="p-diario" class="card hidden">
    <h3>📘 Diário de Classe</h3>
    <p>Área exclusiva do professor.</p>
  </div>  <div id="p-alertas" class="card hidden">
    <h3>🚨 Alertas</h3>
    <p class="alert">Nenhum aluno com excesso de faltas.</p>
  </div>
</div><!-- ALUNO --><div id="aluno" class="hidden">
  <nav class="card">
    <button onclick="show('a-boletim')">Boletim</button>
    <button onclick="show('a-horario')">Horário</button>
    <button onclick="logout()">Sair</button>
  </nav>  <div id="a-boletim" class="card hidden">
    <h3>📄 Boletim</h3>
    <p>Notas e médias do aluno.</p>
  </div>  <div id="a-horario" class="card hidden">
    <h3>📅 Meu Horário</h3>
    <div id="horarioAluno"></div>
  </div>
</div><script>
// EVENTO DO BOTÃO (CORRIGIDO PARA MOBILE)
const btnLogin = document.getElementById('btnLogin');
if(btnLogin){
  btnLogin.addEventListener('click', login);
}

  if(btn){
    btn.addEventListener('click', login);
  }
});

const el = id => document.getElementById(id);
let alunos = [], professores = [], horarios = [];

// ===== LOGIN =====
function login(){
  const m = el('matricula').value.trim();
  const s = el('senha').value.trim();

  if(s !== '123'){
    alert('Senha incorreta');
    return;
  }

  el('login').classList.add('hidden');

  if(m === '999999'){
    el('gestor').classList.remove('hidden');
    show('g-dashboard');
    setTimeout(initDashboard, 50);
  } else if(m === '111111'){
    el('professor').classList.remove('hidden');
    show('p-diario');
  } else {
    el('aluno').classList.remove('hidden');
    show('a-boletim');
  }
}

  el('login').classList.add('hidden');

  if(m === '999999'){
    el('gestor').classList.remove('hidden');
  } else if(m === '111111'){
    el('professor').classList.remove('hidden');
  } else {
    el('aluno').classList.remove('hidden');
  }
}

function logout(){ location.reload(); }

// ===== NAVEGAÇÃO (CORRIGIDA) =====
function show(id){
  document.querySelectorAll('#gestor .card, #professor .card, #aluno .card')
    .forEach(c => c.classList.add('hidden'));
  el(id).classList.remove('hidden');
}

// ===== GESTOR =====
function addAluno(){
  const nome = el('alunoNome').value.trim();
  if(!nome){ alert('Informe o nome do aluno'); return; }

  const mat = Math.floor(10000000 + Math.random()*90000000);
  alunos.push({ nome, mat });

  el('listaAlunos').innerHTML = alunos
    .map(a => `• ${a.nome} — <b>${a.mat}</b>`)
    .join('<br>');

  const q = document.createElement('div');
  new QRCode(q, String(mat));
  el('listaAlunos').appendChild(document.createElement('hr'));
  el('listaAlunos').appendChild(q);

  el('alunoNome').value = '';
}

function addProfessor(){
  const nome = el('profNome').value.trim();
  const disc = el('profDisc').value.trim();
  if(!nome || !disc){ alert('Preencha todos os campos'); return; }

  professores.push({ nome, disc });

  el('listaProf').innerHTML = professores
    .map(p => `• ${p.nome} — ${p.disc}`)
    .join('<br>');

  el('hProf').innerHTML = professores
    .map((p,i)=>`<option value="${i}">${p.nome}</option>`)
    .join('');

  el('profNome').value = '';
  el('profDisc').value = '';
}

function addHorario(){
  const p = professores[el('hProf').value];
  if(!p){ alert('Cadastre um professor primeiro'); return; }

  const disc = el('hDisc').value.trim();
  const dia  = el('hDia').value.trim();
  const hora = el('hHora').value.trim();

  if(!disc || !dia || !hora){ alert('Preencha todos os campos'); return; }

  horarios.push({ prof:p.nome, disc, dia, hora });

  const html = horarios
    .map(h => `• ${h.dia} ${h.hora} — ${h.disc} (${h.prof})`)
    .join('<br>');

  el('listaHorarios').innerHTML = html;
  el('horarioAluno').innerHTML = html;

  el('hDisc').value = '';
  el('hDia').value = '';
  el('hHora').value = '';
}

// ===== DASHBOARD (INICIALIZA SOMENTE SE CHART EXISTIR) =====
function initDashboard(){
  if(typeof Chart === 'undefined') return;
  const ctx = document.getElementById('grafico');
  if(!ctx) return;
  new Chart(ctx,{
    type:'bar',
    data:{
      labels:['1º Bim','2º Bim','3º Bim','4º Bim'],
      datasets:[{ data:[80,78,85,90] }]
    }
  });
}
</script></body>
</html>