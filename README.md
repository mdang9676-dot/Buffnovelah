<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>TOOL-NOVELAH_by KING - Full + IB </title>
  <style>
    body {
      font-family: 'Courier New', monospace;
      background: #0d1a0d;
      color: #00ff41;
      min-height: 100vh;
      padding: 15px;
      margin: 0;
      background-image: linear-gradient(rgba(0,255,0,0.07) 1px, transparent 1px),
                        linear-gradient(90deg, rgba(0,255,0,0.07) 1px, transparent 1px);
      background-size: 40px 40px;
    }
    .container { max-width: 800px; margin: auto; }
    h1 { text-align: center; text-shadow: 0 0 15px #00ff41; font-size: 2.3rem; margin: 20px 0; letter-spacing: 3px; }
    .section {
      background: rgba(0,20,0,0.8);
      border: 2px solid #00ff41;
      border-radius: 10px;
      padding: 20px;
      margin: 20px 0;
      box-shadow: 0 0 20px rgba(0,255,0,0.4);
    }
    input, select, button {
      width: 100%;
      padding: 12px;
      margin: 10px 0;
      font-size: 1.1rem;
      border-radius: 6px;
      border: none;
    }
    input { background: #001100; color: #00ff41; border: 1px solid #00cc33; }
    select { background: #001100; color: #00ff41; border: 1px solid #00cc33; }
    button {
      background: #9b5de5;
      color: white;
      font-weight: bold;
      cursor: pointer;
      box-shadow: 0 0 12px #9b5de5;
    }
    button:disabled { background: #444; cursor: not-allowed; box-shadow: none; opacity: 0.6; }
    button:hover:not(:disabled) { background: #c77dff; transform: scale(1.03); }
    .status { text-align: center; font-size: 1.4rem; margin: 15px 0; }
    .success { color: #00ff41; text-shadow: 0 0 10px #00ff41; }
    .error { color: #ff3366; text-shadow: 0 0 10px #ff3366; }
    .buffing { color: #ffcc00; animation: blink 1s infinite; }
    @keyframes blink { 50% { opacity: 0.6; } }
    .account-item {
      background: rgba(0,40,0,0.7);
      padding: 15px;
      margin: 15px 0;
      border-left: 6px solid #00ff41;
      border-radius: 8px;
      font-size: 1.1rem;
    }
    .copy-btn {
      background: #00cc99;
      color: black;
      padding: 8px 14px;
      margin-left: 10px;
      border-radius: 5px;
      cursor: pointer;
      font-size: 0.95rem;
    }
    .copy-btn:hover { background: #00ffbb; }
    .copy-all-btn {
      background: #ffd700;
      color: #001100;
      font-weight: bold;
      margin-top: 20px;
    }
    .buff-options { display: flex; flex-wrap: wrap; gap: 12px; justify-content: center; margin: 15px 0; }
    .buff-btn {
      background: #ffd700;
      color: #001100;
      padding: 12px 20px;
      border: none;
      border-radius: 6px;
      cursor: pointer;
      box-shadow: 0 0 10px #ffd700;
    }
    .buff-btn.selected {
      background: #ff3366;
      color: white;
      box-shadow: 0 0 15px #ff3366;
    }
    .get-key-info {
      background: rgba(255,51,102,0.15);
      border: 1px dashed #ff3366;
      padding: 15px;
      margin: 15px 0;
      border-radius: 8px;
      text-align: center;
    }
    .link-btn {
      background: #ff3366;
      color: white;
      box-shadow: 0 0 15px #ff3366;
    }
    .link-btn:hover { background: #ff6699; }
    .contact-section {
      text-align: center;
      margin-top: 30px;
      padding: 20px;
      background: rgba(255,215,0,0.1);
      border: 1px dashed #ffd700;
      border-radius: 10px;
    }
    .contact-btn {
      background: #4267B2 !important; /* FB blue */
      margin: 10px 5px;
      padding: 14px 24px;
      font-size: 1.1rem;
    }
    .contact-btn.tiktok {
      background: #000 !important; /* TikTok black */
    }
    .hidden { display: none; }
    #greeting {
      position: fixed;
      inset: 0;
      background: rgba(0,26,13,0.98);
      display: flex;
      align-items: center;
      justify-content: center;
      z-index: 9999;
      transition: opacity 0.8s ease-out, transform 0.8s ease-out;
    }
    #greeting h2 {
      font-size: 7rem;
      color: #00ff41;
      text-shadow: 0 0 60px #00ff41, 0 0 100px #00ff41;
      animation: pulse 1.2s infinite alternate;
    }
    @keyframes pulse { from { transform: scale(1); } to { transform: scale(1.1); } }
    #greeting.fade-out { opacity: 0; transform: scale(0.8); }
    #main-content { opacity: 0; transition: opacity 0.6s ease-in; }
  </style>
</head>
<body>

<div id="greeting"><h2>Hello</h2></div>

<div class="container" id="main-content">
  <h1>TOOL-NOVELAH_by KING</h1>

  <!-- KEY THƯỜNG -->
  <div id="key-normal-section" class="section">
    <h2 style="text-align:center; color:#00ff99;">NHẬP KEY FREE</h2>
    <input type="text" id="key-normal" placeholder="Nhập key thường ở đây..." />
    <button onclick="checkNormalKey()">CHECK KEY ❤️</button>
    <div id="normal-status" class="status"></div>

    <div class="get-key-info">
      <p style="color:#ffcc00; margin-bottom:10px;">Chưa có key? Vượt link lấy free ngay!</p>
      <button class="link-btn" onclick="window.open('https://link4m.com/46N3uJO', '_blank')">VƯỢT LINK LẤY KEY 🔥</button>
      <p style="font-size:0.9rem; margin-top:10px;">(Làm theo hướng dẫn → copy key về dán)</p>
    </div>

    <div id="normal-content" class="hidden">
      <h3 style="text-align:center; color:#00ffcc;">TẠO TÀI KHOẢN NHANH (Thủ công)</h3>
      <label>Số lượng acc:</label>
      <select id="acc-count">
        <option value="1">1 acc</option>
        <option value="2">2 acc</option>
        <option value="3">3 acc</option>
        <option value="4">4 acc</option>
        <option value="5">5 acc</option>
        <option value="10">10 acc</option>
      </select>
      <button onclick="generateAccounts()">XÁC NHẬN ✓ TẠO ACC</button>
      <div id="acc-status" class="status hidden">Đang tạo acc...</div>
      <div id="accounts-list" class="hidden"></div>
      <button id="copy-all-acc" class="copy-all-btn hidden" onclick="copyAllAcc()">COPY TẤT CẢ ACC VÀO CLIPBOARD</button>
    </div>
  </div>

  <!-- VIP PREMIUM -->
  <div class="section">
    <h2 style="text-align:center; color:#ffd700;">MỤC VIP (Key Premium)</h2>
    <input type="text" id="key-vip" placeholder="Nhập key premium..." />
    <button onclick="checkVipKey()">CHECK KEY</button>
    <div id="vip-status" class="status"></div>

    <div id="vip-content" class="hidden">
      <h3 style="text-align:center; color:#ffd700;">BUFF ĐIỂM PREMIUM</h3>

      <label>Nhập mã mời (8 số):</label>
      <input type="text" id="invite-code" placeholder="Ví dụ: 12345678" maxlength="8" oninput="validateInviteCode()" />

      <label style="margin-top:15px;">Chọn gói điểm:</label>
      <div class="buff-options" id="buff-options">
        <button class="buff-btn" data-points="30000" disabled>30k điểm</button>
        <button class="buff-btn" data-points="60000" disabled>60k điểm</button>
        <button class="buff-btn" data-points="120000" disabled>120k điểm</button>
        <button class="buff-btn" data-points="150000" disabled>150k điểm</button>
        <button class="buff-btn" data-points="200000" disabled>200k điểm</button>
        <button class="buff-btn" data-points="500000" disabled>500k điểm</button>
      </div>

      <button id="buff-confirm-btn" disabled onclick="startBuff()">XÁC NHẬN BUFF</button>
      <div id="buff-status" class="status hidden"></div>
    </div>
  </div>

  <!-- PHẦN IB MUA KEY -->
  <div class="contact-section">
    <p style="font-size:1.3rem; color:#ffd700; margin-bottom:15px;">Chưa có key VIP? IB ngay để mua key premium</p>
    <button class="contact-btn" onclick="window.open('https://www.facebook.com/angminh.972364', '_blank')">IB Facebook</button>
    <button class="contact-btn tiktok" onclick="window.open('https://www.tiktok.com/@nhincaij026', '_blank')">IB TikTok</button>
  </div>

</div>

<script>
// Greeting tắt hẳn
window.addEventListener('load', () => {
  const greeting = document.getElementById('greeting');
  const main = document.getElementById('main-content');
  setTimeout(() => {
    greeting.classList.add('fade-out');
    setTimeout(() => {
      greeting.remove();
      main.style.opacity = '1';
    }, 800);
  }, 3000);
});

// KEY THƯỜNG
function checkNormalKey() {
  const key = document.getElementById('key-normal').value.trim();
  const status = document.getElementById('normal-status');
  const content = document.getElementById('normal-content');

  if (key === 'toolfree-2026-76') {
    status.innerHTML = '<span class="success">KEY ĐÚNG ✅ - ĐÃ KÍCH HOẠT!</span>';
    content.classList.remove('hidden');
    document.getElementById('key-normal').classList.add('hidden');
    document.querySelector('#key-normal-section button[onclick="checkNormalKey()"]').classList.add('hidden');
    document.querySelector('.get-key-info').classList.add('hidden');
  } else {
    status.innerHTML = '<span class="error">Key sai ❌</span><br><p style="color:#ffcc00;">Chưa có key? Nhấn vượt link bên trên nhé!</p>';
  }
}

// TẠO ACC
function generateAccounts() {
  const count = parseInt(document.getElementById('acc-count').value);
  const status = document.getElementById('acc-status');
  const list = document.getElementById('accounts-list');
  const copyBtn = document.getElementById('copy-all-acc');

  status.classList.remove('hidden');
  list.classList.add('hidden');
  list.innerHTML = '';
  copyBtn.classList.add('hidden');

  setTimeout(() => {
    status.classList.add('hidden');
    let allText = '';
    let html = '';

    for (let i = 1; i <= count; i++) {
      const rand = Math.floor(Math.random() * 9000 + 1000);
      const email = `Kingdeptrai${rand}@gmail.com`;
      const pass = '123456789deptrai';

      allText += `Acc ${i}:\nTên: ${email}\nMk: ${pass}\n\n`;

      html += `
        <div class="account-item">
          <strong>Acc ${i}</strong><br>
          Tên: ${email} 
          <button class="copy-btn" onclick="copy('${email}')">Copy tên</button><br>
          Mk: ${pass} 
          <button class="copy-btn" onclick="copy('${pass}')">Copy mk</button>
        </div>
      `;
    }

    list.innerHTML = html;
    list.classList.remove('hidden');
    copyBtn.dataset.text = allText;
    copyBtn.classList.remove('hidden');
  }, 1200);
}

// VIP PREMIUM
let selectedPoints = null;
let inviteCodeValid = false;
let isBuffing = false;

function validateInviteCode() {
  if (isBuffing) return;
  const code = document.getElementById('invite-code').value.trim();
  const buffBtns = document.querySelectorAll('.buff-btn');
  const buffBtn = document.getElementById('buff-confirm-btn');

  if (/^\d{8}$/.test(code)) {
    inviteCodeValid = true;
    buffBtns.forEach(btn => { if (!isBuffing) btn.disabled = false; });
  } else {
    inviteCodeValid = false;
    buffBtns.forEach(btn => btn.disabled = true);
    buffBtn.disabled = true;
    selectedPoints = null;
    document.querySelectorAll('.buff-btn').forEach(b => b.classList.remove('selected'));
  }
  checkBuffReady();
}

document.querySelectorAll('.buff-btn').forEach(btn => {
  btn.onclick = () => {
    if (btn.disabled || isBuffing) return;
    document.querySelectorAll('.buff-btn').forEach(b => b.classList.remove('selected'));
    btn.classList.add('selected');
    selectedPoints = btn.dataset.points;
    checkBuffReady();
  };
});

function checkBuffReady() {
  const buffBtn = document.getElementById('buff-confirm-btn');
  buffBtn.disabled = !(inviteCodeValid && selectedPoints !== null) || isBuffing;
}

function checkVipKey() {
  const key = document.getElementById('key-vip').value.trim();
  const status = document.getElementById('vip-status');
  if (key === 'keypremium-2026') {
    status.innerHTML = '<span class="success">Key VIP đúng ✅ - Mở khóa premium</span>';
    document.getElementById('vip-content').classList.remove('hidden');
  } else {
    status.innerHTML = '<span class="error">Key sai ❌</span>';
  }
}

function startBuff() {
  if (!inviteCodeValid || !selectedPoints) return alert('Nhập mã mời 8 số và chọn gói điểm trước nhé!');
  isBuffing = true;
  document.getElementById('invite-code').disabled = true;
  document.querySelectorAll('.buff-btn').forEach(btn => btn.disabled = true);
  document.getElementById('buff-confirm-btn').disabled = true;

  const code = document.getElementById('invite-code').value.trim();
  const status = document.getElementById('buff-status');
  status.classList.remove('hidden');
  let time = 30;
  status.innerHTML = `<span class="buffing">Đang buff ${selectedPoints/1000}k điểm 🔄<br>Mã mời: ${code}<br>Vui lòng không thoát trang</span><br>Còn ${time} giây...`;

  const timer = setInterval(() => {
    time--;
    status.innerHTML = `<span class="buffing">Đang buff ${selectedPoints/1000}k điểm 🔄<br>Mã mời: ${code}<br>Vui lòng không thoát trang</span><br>Còn ${time} giây...`;
    if (time <= 0) {
      clearInterval(timer);
      status.innerHTML = `<span class="success">BUFF THÀNH CÔNG! ✅<br>Nhận ${selectedPoints/1000}k điểm với mã mời ${code}!</span>`;
      isBuffing = false;
    }
  }, 1000);
}

function copy(text) {
  navigator.clipboard.writeText(text).then(() => alert('Đã copy: ' + text)).catch(() => alert('Copy thủ công nhé Cem!'));
}

function copyAllAcc() {
  const text = document.getElementById('copy-all-acc').dataset.text;
  navigator.clipboard.writeText(text).then(() => alert('Copy tất cả acc thành công!\nDán vào note để đăng ký dần.')).catch(() => alert('Copy thủ công nhé!'));
}
</script>
</body>
</html>    <button class="contact-btn tiktok" onclick="window.open('https://www.tiktok.com/@nhincaij026', '_blank')">IB TikTok</button>
  </div>

</div>

<script>
// Greeting tắt hẳn
window.addEventListener('load', () => {
  const greeting = document.getElementById('greeting');
  const main = document.getElementById('main-content');
  setTimeout(() => {
    greeting.classList.add('fade-out');
    setTimeout(() => {
      greeting.remove();
      main.style.opacity = '1';
    }, 800);
  }, 3000);
});

// KEY THƯỜNG
function checkNormalKey() {
  const key = document.getElementById('key-normal').value.trim();
  const status = document.getElementById('normal-status');
  const content = document.getElementById('normal-content');

  if (key === 'toolvip2026-ẩn') {
    status.innerHTML = '<span class="success">KEY ĐÚNG ✅ - ĐÃ KÍCH HOẠT!</span>';
    content.classList.remove('hidden');
    document.getElementById('key-normal').classList.add('hidden');
    document.querySelector('#key-normal-section button[onclick="checkNormalKey()"]').classList.add('hidden');
    document.querySelector('.get-key-info').classList.add('hidden');
  } else {
    status.innerHTML = '<span class="error">Key sai ❌</span><br><p style="color:#ffcc00;">Chưa có key? Nhấn vượt link bên trên nhé!</p>';
  }
}

// TẠO ACC
function generateAccounts() {
  const count = parseInt(document.getElementById('acc-count').value);
  const status = document.getElementById('acc-status');
  const list = document.getElementById('accounts-list');
  const copyBtn = document.getElementById('copy-all-acc');

  status.classList.remove('hidden');
  list.classList.add('hidden');
  list.innerHTML = '';
  copyBtn.classList.add('hidden');

  setTimeout(() => {
    status.classList.add('hidden');
    let allText = '';
    let html = '';

    for (let i = 1; i <= count; i++) {
      const rand = Math.floor(Math.random() * 9000 + 1000);
      const email = `Kingdeptrai${rand}@gmail.com`;
      const pass = '123456789deptrai';

      allText += `Acc ${i}:\nTên: ${email}\nMk: ${pass}\n\n`;

      html += `
        <div class="account-item">
          <strong>Acc ${i}</strong><br>
          Tên: ${email} 
          <button class="copy-btn" onclick="copy('${email}')">Copy tên</button><br>
          Mk: ${pass} 
          <button class="copy-btn" onclick="copy('${pass}')">Copy mk</button>
        </div>
      `;
    }

    list.innerHTML = html;
    list.classList.remove('hidden');
    copyBtn.dataset.text = allText;
    copyBtn.classList.remove('hidden');
  }, 1200);
}

// VIP PREMIUM
let selectedPoints = null;
let inviteCodeValid = false;
let isBuffing = false;

function validateInviteCode() {
  if (isBuffing) return;
  const code = document.getElementById('invite-code').value.trim();
  const buffBtns = document.querySelectorAll('.buff-btn');
  const buffBtn = document.getElementById('buff-confirm-btn');

  if (/^\d{8}$/.test(code)) {
    inviteCodeValid = true;
    buffBtns.forEach(btn => { if (!isBuffing) btn.disabled = false; });
  } else {
    inviteCodeValid = false;
    buffBtns.forEach(btn => btn.disabled = true);
    buffBtn.disabled = true;
    selectedPoints = null;
    document.querySelectorAll('.buff-btn').forEach(b => b.classList.remove('selected'));
  }
  checkBuffReady();
}

document.querySelectorAll('.buff-btn').forEach(btn => {
  btn.onclick = () => {
    if (btn.disabled || isBuffing) return;
    document.querySelectorAll('.buff-btn').forEach(b => b.classList.remove('selected'));
    btn.classList.add('selected');
    selectedPoints = btn.dataset.points;
    checkBuffReady();
  };
});

function checkBuffReady() {
  const buffBtn = document.getElementById('buff-confirm-btn');
  buffBtn.disabled = !(inviteCodeValid && selectedPoints !== null) || isBuffing;
}

function checkVipKey() {
  const key = document.getElementById('key-vip').value.trim();
  const status = document.getElementById('vip-status');
  if (key === 'keypremium2026-ẩn') {
    status.innerHTML = '<span class="success">Key VIP đúng ✅ - Mở khóa premium</span>';
    document.getElementById('vip-content').classList.remove('hidden');
  } else {
    status.innerHTML = '<span class="error">Key sai ❌</span>';
  }
}

function startBuff() {
  if (!inviteCodeValid || !selectedPoints) return alert('Nhập mã mời 8 số và chọn gói điểm trước nhé!');
  isBuffing = true;
  document.getElementById('invite-code').disabled = true;
  document.querySelectorAll('.buff-btn').forEach(btn => btn.disabled = true);
  document.getElementById('buff-confirm-btn').disabled = true;

  const code = document.getElementById('invite-code').value.trim();
  const status = document.getElementById('buff-status');
  status.classList.remove('hidden');
  let time = 30;
  status.innerHTML = `<span class="buffing">Đang buff ${selectedPoints/1000}k điểm 🔄<br>Mã mời: ${code}<br>Vui lòng không thoát trang</span><br>Còn ${time} giây...`;

  const timer = setInterval(() => {
    time--;
    status.innerHTML = `<span class="buffing">Đang buff ${selectedPoints/1000}k điểm 🔄<br>Mã mời: ${code}<br>Vui lòng không thoát trang</span><br>Còn ${time} giây...`;
    if (time <= 0) {
      clearInterval(timer);
      status.innerHTML = `<span class="success">BUFF THÀNH CÔNG! ✅<br>Nhận ${selectedPoints/1000}k điểm với mã mời ${code}!</span>`;
      isBuffing = false;
    }
  }, 1000);
}

function copy(text) {
  navigator.clipboard.writeText(text).then(() => alert('Đã copy: ' + text)).catch(() => alert('Copy thủ công nhé Cem!'));
}

function copyAllAcc() {
  const text = document.getElementById('copy-all-acc').dataset.text;
  navigator.clipboard.writeText(text).then(() => alert('Copy tất cả acc thành công!\nDán vào note để đăng ký dần.')).catch(() => alert('Copy thủ công nhé!'));
}
</script>
</body>
</html>
