<!doctype html>
<html lang="zh-Hant">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>SQL 教材｜SELECT 互動式教學</title>
  <style>
    :root{
      --bg:#0b1220;
      --card:#121b2f;
      --card2:#0f172a;
      --text:#e5e7eb;
      --muted:#a7b0c0;
      --accent:#60a5fa;
      --accent2:#34d399;
      --warn:#fbbf24;
      --danger:#fb7185;
      --line:rgba(255,255,255,.08);
      --shadow: 0 10px 25px rgba(0,0,0,.35);
      --radius:16px;
      --mono: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono","Courier New", monospace;
    }
    *{box-sizing:border-box}
    body{
      margin:0;
      font-family: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, "Noto Sans TC", Arial, sans-serif;
      background: radial-gradient(1200px 600px at 20% 0%, rgba(96,165,250,.15), transparent 60%),
                  radial-gradient(1000px 500px at 80% 0%, rgba(52,211,153,.12), transparent 55%),
                  var(--bg);
      color:var(--text);
    }
    header{
      max-width: 1100px;
      margin: 28px auto 10px;
      padding: 0 18px;
      display:flex;
      gap:16px;
      align-items:flex-start;
      justify-content:space-between;
      flex-wrap:wrap;
    }
    .brand{
      display:flex; gap:12px; align-items:center;
    }
    .logo{
      width:44px; height:44px; border-radius:14px;
      background: linear-gradient(135deg, rgba(96,165,250,.9), rgba(52,211,153,.85));
      box-shadow: var(--shadow);
    }
    h1{
      margin:0;
      font-size: 20px;
      line-height: 1.2;
    }
    .subtitle{
      margin:4px 0 0;
      color: var(--muted);
      font-size: 13px;
    }
    .top-actions{
      display:flex; gap:10px; align-items:center;
      flex-wrap:wrap;
    }
    button, .pill{
      border:1px solid var(--line);
      background: rgba(255,255,255,.04);
      color: var(--text);
      padding: 10px 12px;
      border-radius: 12px;
      cursor:pointer;
      font-weight: 600;
      transition: .15s ease;
    }
    button:hover{
      transform: translateY(-1px);
      background: rgba(255,255,255,.06);
    }
    button:disabled{
      opacity:.45;
      cursor:not-allowed;
      transform:none;
    }
    .pill{
      cursor: default;
      font-size: 12px;
      color: var(--muted);
      font-weight: 600;
    }
    main{
      max-width: 1100px;
      margin: 0 auto 40px;
      padding: 0 18px;
      display:grid;
      grid-template-columns: 360px 1fr;
      gap: 16px;
    }
    @media (max-width: 980px){
      main{grid-template-columns: 1fr}
    }
    .panel{
      background: rgba(18,27,47,.78);
      border: 1px solid var(--line);
      border-radius: var(--radius);
      box-shadow: var(--shadow);
      overflow:hidden;
    }
    .panel .hd{
      padding: 14px 16px;
      border-bottom: 1px solid var(--line);
      display:flex; align-items:center; justify-content:space-between;
      gap:10px;
    }
    .panel .hd strong{font-size: 14px}
    .panel .bd{padding: 14px 16px}
    .progress{
      height:10px;
      background: rgba(255,255,255,.06);
      border-radius: 999px;
      overflow:hidden;
      border:1px solid var(--line);
    }
    .bar{
      height:100%;
      width:0%;
      background: linear-gradient(90deg, rgba(96,165,250,.9), rgba(52,211,153,.85));
      transition: width .25s ease;
    }
    .list{
      display:flex;
      flex-direction:column;
      gap:10px;
    }
    .stepbtn{
      text-align:left;
      width:100%;
      display:flex;
      gap:10px;
      align-items:center;
      justify-content:space-between;
      padding: 12px 12px;
      border-radius: 14px;
    }
    .left{
      display:flex; gap:10px; align-items:flex-start;
    }
    .num{
      width:26px; height:26px; border-radius: 10px;
      display:grid; place-items:center;
      border: 1px solid var(--line);
      background: rgba(255,255,255,.04);
      font-family: var(--mono);
      font-size: 12px;
      color: var(--muted);
      flex: 0 0 auto;
    }
    .label{
      display:flex; flex-direction:column; gap:3px;
    }
    .label .title{font-weight:800; font-size: 13px}
    .label .desc{color: var(--muted); font-size: 12px}
    .badge{
      font-size: 11px;
      padding: 6px 8px;
      border-radius: 999px;
      border: 1px solid var(--line);
      color: var(--muted);
      background: rgba(255,255,255,.03);
      white-space:nowrap;
    }
    .badge.ok{color: rgba(52,211,153,.9); border-color: rgba(52,211,153,.25); background: rgba(52,211,153,.08)}
    .badge.lock{color: rgba(251,191,36,.9); border-color: rgba(251,191,36,.25); background: rgba(251,191,36,.08)}
    .badge.now{color: rgba(96,165,250,.95); border-color: rgba(96,165,250,.25); background: rgba(96,165,250,.08)}
    .content{
      min-height: 620px;
    }
    .concept{
      display:none;
      animation: fade .18s ease;
    }
    .concept.active{display:block;}
    @keyframes fade{from{opacity:.2; transform: translateY(3px)} to{opacity:1; transform:none}}
    .kicker{
      display:flex; gap:10px; align-items:center; flex-wrap:wrap;
      margin-bottom: 10px;
    }
    .kicker .tag{
      font-size: 12px;
      padding: 6px 10px;
      border-radius: 999px;
      background: rgba(96,165,250,.10);
      border: 1px solid rgba(96,165,250,.25);
      color: rgba(96,165,250,.95);
      font-weight: 800;
    }
    .kicker .tag.green{
      background: rgba(52,211,153,.10);
      border-color: rgba(52,211,153,.25);
      color: rgba(52,211,153,.95);
    }
    .concept h2{
      margin: 6px 0 6px;
      font-size: 18px;
    }
    .note{
      margin: 0 0 12px;
      color: var(--muted);
      line-height: 1.6;
      font-size: 14px;
    }
    .grid2{
      display:grid;
      grid-template-columns: 1fr 1fr;
      gap: 12px;
    }
    @media (max-width: 980px){
      .grid2{grid-template-columns: 1fr}
    }
    .box{
      background: rgba(15,23,42,.6);
      border: 1px solid var(--line);
      border-radius: 14px;
      overflow:hidden;
    }
    .box .bhd{
      padding: 10px 12px;
      border-bottom: 1px solid var(--line);
      display:flex; align-items:center; justify-content:space-between; gap:10px;
      color: var(--muted);
      font-size: 12px;
      font-weight: 700;
    }
    .box .bbd{padding: 10px 12px}
    pre{
      margin:0;
      padding: 12px;
      border-radius: 12px;
      background: rgba(0,0,0,.35);
      border: 1px solid rgba(255,255,255,.08);
      overflow:auto;
      font-family: var(--mono);
      font-size: 13px;
      line-height: 1.55;
    }
    .actions{
      display:flex; gap:10px; flex-wrap:wrap;
      margin-top: 10px;
    }
    .btn-accent{
      background: rgba(96,165,250,.14);
      border-color: rgba(96,165,250,.25);
    }
    .btn-green{
      background: rgba(52,211,153,.14);
      border-color: rgba(52,211,153,.25);
    }
    .btn-warn{
      background: rgba(251,191,36,.14);
      border-color: rgba(251,191,36,.25);
    }
    .result{
      font-family: var(--mono);
      font-size: 12.5px;
      color: #dbeafe;
      line-height: 1.55;
    }
    table{
      width:100%;
      border-collapse: collapse;
      overflow:hidden;
      border-radius: 12px;
      border: 1px solid rgba(255,255,255,.08);
      background: rgba(0,0,0,.25);
    }
    th, td{
      padding: 9px 10px;
      border-bottom: 1px solid rgba(255,255,255,.06);
      text-align:left;
      vertical-align: top;
    }
    th{
      color: var(--muted);
      font-size: 12px;
      font-weight: 800;
      background: rgba(255,255,255,.03);
    }
    tr:last-child td{border-bottom:none}
    .hint{
      padding: 10px 12px;
      border-radius: 14px;
      background: rgba(251,191,36,.10);
      border: 1px solid rgba(251,191,36,.22);
      color: #fde68a;
      font-size: 13px;
      line-height: 1.6;
      margin-top: 12px;
    }
    .okhint{
      padding: 10px 12px;
      border-radius: 14px;
      background: rgba(52,211,153,.10);
      border: 1px solid rgba(52,211,153,.22);
      color: #bbf7d0;
      font-size: 13px;
      line-height: 1.6;
      margin-top: 12px;
    }
    .editor{
      width:100%;
      min-height: 120px;
      border-radius: 12px;
      border: 1px solid rgba(255,255,255,.10);
      background: rgba(0,0,0,.30);
      color: var(--text);
      padding: 10px 12px;
      font-family: var(--mono);
      font-size: 13px;
      outline:none;
      line-height:1.6;
      resize: vertical;
    }
    footer{
      max-width: 1100px;
      margin: 0 auto 40px;
      padding: 0 18px;
      color: var(--muted);
      font-size: 12px;
      line-height: 1.6;
    }
    code{font-family: var(--mono)}
  </style>
</head>

<body>
<header>
  <div class="brand">
    <div class="logo"></div>
    <div>
      <h1>SQL 互動式教材：SELECT 從 0 到上手</h1>
      <p class="subtitle">一個概念一個概念往下學（member / product / orders / comment 模擬資料）</p>
    </div>
  </div>
  <div class="top-actions">
    <span class="pill" id="statusPill">進度：0 / 7</span>
    <button id="btnReset" class="btn-warn">重置進度</button>
    <button id="btnNext" class="btn-accent" disabled>下一個概念</button>
  </div>
</header>

<main>
  <!-- 左：步驟導覽 -->
  <section class="panel">
    <div class="hd">
      <strong>課程導覽</strong>
      <div style="min-width:120px">
        <div class="progress" aria-label="progress">
          <div class="bar" id="progressBar"></div>
        </div>
      </div>
    </div>

    <div class="bd">
      <div class="list" id="stepList"></div>
      <div class="hint" style="margin-top:14px">
        使用方式：<br/>
        1) 先點第 1 個概念 → 看說明 → 按「執行」看結果<br/>
        2) 完成後按「標記完成」→ 才能解鎖下一個概念
      </div>
    </div>
  </section>

  <!-- 右：內容區 -->
  <section class="panel content">
    <div class="hd">
      <strong id="contentTitle">請從左側第 1 個概念開始</strong>
      <span class="badge now" id="contentBadge">尚未開始</span>
    </div>
    <div class="bd" id="contentArea"></div>
  </section>
</main>

<footer>
  這份教材用「模擬資料」呈現結果，目的是讓學生在沒有連線資料庫時也能互動練習。<br/>
  你也可以把每段 SQL 直接貼到 phpMyAdmin 的 SQL 頁籤實際執行（你的 firstdb：member / product / orders / comment）。
</footer>

<script>
  // -----------------------
  // 模擬資料（對應你的表）
  // -----------------------
  const data = {
    member: [
      { mem_id: 1, cname: "小華", cemail: "hua@test.com", phone: "0911111111", birthday: "1995-01-01" },
      { mem_id: 2, cname: "小美", cemail: "mei@test.com", phone: "0922222222", birthday: "1996-02-02" },
      { mem_id: 3, cname: "小強", cemail: "qiang@test.com", phone: "0933333333", birthday: "1997-03-03" },
      { mem_id: 4, cname: "小芳", cemail: "fang@test.com", phone: "0944444444", birthday: "1998-04-04" },
      { mem_id: 5, cname: "小明", cemail: "ming@test.com", phone: "0955555555", birthday: "1999-05-05" }
    ],
    product: [
      { pro_id: 1, productName: "iPhone 15", pcategory: "electronics", sku:"APL-001", price:30000, stock:50 },
      { pro_id: 2, productName: "Nike Shoes", pcategory: "sports", sku:"NK-002", price:4500, stock:100 },
      { pro_id: 3, productName: "T-shirt", pcategory: "clothing", sku:"CL-003", price:800, stock:200 },
      { pro_id: 4, productName: "Coffee", pcategory: "food", sku:"FD-004", price:200, stock:500 }
    ],
    comment: [
      { msg_id: 1, mem_id: 1, pro_id: 1, rating: 5, comment_text: "這支手機真的很好用！", comment_date:"2024-01-10 10:30:00"},
      { msg_id: 2, mem_id: 2, pro_id: 2, rating: 4, comment_text: "鞋子很舒服，會再回購", comment_date:"2024-01-11 14:20:00"},
      { msg_id: 3, mem_id: 3, pro_id: 3, rating: 3, comment_text: "品質普通，價格還可以", comment_date:"2024-01-12 09:15:00"},
      { msg_id: 4, mem_id: 4, pro_id: 1, rating: 5, comment_text: "拍照功能很強", comment_date:"2024-01-13 18:45:00"},
      { msg_id: 5, mem_id: 5, pro_id: 4, rating: 2, comment_text: "咖啡味道偏苦，不太喜歡", comment_date:"2024-01-14 08:00:00"},
    ]
  };

  // -----------------------
  // 教學步驟（逐步解鎖）
  // -----------------------
  const steps = [
    {
      id: "s1",
      title: "SELECT *：看全部資料",
      desc: "查某張表所有欄位、所有資料",
      tag: "SELECT *",
      explain: [
        "SELECT 是「查詢資料」的指令。",
        "`*` 代表「所有欄位」。",
        "常用來：第一次查看資料表內容。"
      ],
      sqlSamples: [
        { label: "查詢所有會員", sql: "SELECT * FROM member;" , run: () => tableFrom(data.member) },
        { label: "查詢所有商品", sql: "SELECT * FROM product;" , run: () => tableFrom(data.product) }
      ],
      practice: {
        prompt: "請找出 comment 表的所有資料（用 SELECT *）。",
        answer: "SELECT * FROM comment;",
        run: () => tableFrom(data.comment)
      }
    },
    {
      id: "s2",
      title: "SELECT 欄位：只拿需要的欄位",
      desc: "避免 *，只選你要的欄位",
      tag: "欄位選取",
      explain: [
        "實務上通常不會一直用 `SELECT *`，因為欄位多會亂、也浪費傳輸。",
        "你可以指定要哪些欄位，例如：姓名 + Email。"
      ],
      sqlSamples: [
        {
          label: "只看會員姓名與 Email",
          sql: "SELECT cname, cemail FROM member;",
          run: () => tableFrom(selectCols(data.member, ["cname","cemail"]))
        },
        {
          label: "只看商品名稱與價格",
          sql: "SELECT productName, price FROM product;",
          run: () => tableFrom(selectCols(data.product, ["productName","price"]))
        }
      ],
      practice: {
        prompt: "只查 product 的 productName 和 stock 兩個欄位。",
        answer: "SELECT productName, stock FROM product;",
        run: () => tableFrom(selectCols(data.product, ["productName","stock"]))
      }
    },
    {
      id: "s3",
      title: "WHERE：加條件篩選",
      desc: "只要符合條件的資料",
      tag: "WHERE",
      explain: [
        "WHERE 就是「篩選」。",
        "語法：`SELECT ... FROM ... WHERE 條件;`",
        "注意：字串要加單引號，例如 `pcategory = 'food'`。"
      ],
      sqlSamples: [
        {
          label: "找 mem_id = 5 的會員（小明）",
          sql: "SELECT * FROM member WHERE mem_id = 5;",
          run: () => tableFrom(filter(data.member, r => r.mem_id === 5))
        },
        {
          label: "找 food 類商品",
          sql: "SELECT productName, price FROM product WHERE pcategory = 'food';",
          run: () => tableFrom(selectCols(filter(data.product, r => r.pcategory === "food"), ["productName","price"]))
        },
        {
          label: "找 rating >= 4 的評論",
          sql: "SELECT * FROM comment WHERE rating >= 4;",
          run: () => tableFrom(filter(data.comment, r => r.rating >= 4))
        }
      ],
      practice: {
        prompt: "找出 price > 1000 的商品（只顯示 productName, price）。",
        answer: "SELECT productName, price FROM product WHERE price > 1000;",
        run: () => tableFrom(selectCols(filter(data.product, r => r.price > 1000), ["productName","price"]))
      }
    },
    {
      id: "s4",
      title: "AND / OR：多條件篩選",
      desc: "條件可以組合起來",
      tag: "AND / OR",
      explain: [
        "`AND`：兩個條件都要成立。",
        "`OR`：任一條件成立即可。",
        "括號可以控制優先順序，例如：(A OR B) AND C"
      ],
      sqlSamples: [
        {
          label: "food 類且價格 < 500",
          sql: "SELECT productName, price FROM product WHERE pcategory='food' AND price < 500;",
          run: () => tableFrom(selectCols(filter(data.product, r => r.pcategory==="food" && r.price < 500), ["productName","price"]))
        },
        {
          label: "rating = 5 或 4",
          sql: "SELECT * FROM comment WHERE rating = 5 OR rating = 4;",
          run: () => tableFrom(filter(data.comment, r => r.rating===5 || r.rating===4))
        }
      ],
      practice: {
        prompt: "找出 sports 類 或 electronics 類 的商品（顯示 productName, pcategory）。",
        answer: "SELECT productName, pcategory FROM product WHERE pcategory='sports' OR pcategory='electronics';",
        run: () => tableFrom(selectCols(filter(data.product, r => r.pcategory==="sports" || r.pcategory==="electronics"), ["productName","pcategory"]))
      }
    },
    {
      id: "s5",
      title: "ORDER BY：排序資料",
      desc: "由大到小、由新到舊",
      tag: "ORDER BY",
      explain: [
        "ORDER BY 用來「排序」。",
        "ASC：由小到大（預設），DESC：由大到小。",
        "日期常用 DESC：最新在最上面。"
      ],
      sqlSamples: [
        {
          label: "商品價格由高到低",
          sql: "SELECT productName, price FROM product ORDER BY price DESC;",
          run: () => tableFrom(selectCols(sortBy([...data.product], "price", "DESC"), ["productName","price"]))
        },
        {
          label: "評論時間由新到舊",
          sql: "SELECT * FROM comment ORDER BY comment_date DESC;",
          run: () => tableFrom(sortBy([...data.comment], "comment_date", "DESC"))
        }
      ],
      practice: {
        prompt: "把 member 依照 mem_id 由大到小排序。",
        answer: "SELECT * FROM member ORDER BY mem_id DESC;",
        run: () => tableFrom(sortBy([...data.member], "mem_id", "DESC"))
      }
    },
    {
      id: "s6",
      title: "LIMIT：只顯示前幾筆",
      desc: "控制筆數，做列表/首頁很常用",
      tag: "LIMIT",
      explain: [
        "LIMIT 用來限制回傳筆數。",
        "常與 ORDER BY 搭配：例如「最新 3 筆」。"
      ],
      sqlSamples: [
        {
          label: "最新 3 筆評論",
          sql: "SELECT * FROM comment ORDER BY comment_date DESC LIMIT 3;",
          run: () => tableFrom(sortBy([...data.comment], "comment_date", "DESC").slice(0,3))
        },
        {
          label: "最便宜的 2 個商品",
          sql: "SELECT productName, price FROM product ORDER BY price ASC LIMIT 2;",
          run: () => tableFrom(selectCols(sortBy([...data.product], "price", "ASC").slice(0,2), ["productName","price"]))
        }
      ],
      practice: {
        prompt: "找出價格由高到低的商品，只顯示前 1 筆。",
        answer: "SELECT * FROM product ORDER BY price DESC LIMIT 1;",
        run: () => tableFrom(sortBy([...data.product], "price", "DESC").slice(0,1))
      }
    },
    {
      id: "s7",
      title: "綜合練習：WHERE + ORDER BY + LIMIT",
      desc: "一次把常用招式串起來",
      tag: "綜合",
      explain: [
        "最常見查詢組合：",
        "1) 先 WHERE 篩選 → 2) ORDER BY 排序 → 3) LIMIT 控制筆數",
        "這就是商品列表、最新評論、排行榜的核心。"
      ],
      sqlSamples: [
        {
          label: "food 類商品：由便宜到貴，取前 3 筆",
          sql: "SELECT productName, price FROM product WHERE pcategory='food' ORDER BY price ASC LIMIT 3;",
          run: () => {
            const rows = filter(data.product, r => r.pcategory==="food");
            const sorted = sortBy(rows, "price", "ASC").slice(0,3);
            return tableFrom(selectCols(sorted, ["productName","price"]));
          }
        },
        {
          label: "高分評論：rating >= 4，由新到舊，取前 2 筆",
          sql: "SELECT * FROM comment WHERE rating >= 4 ORDER BY comment_date DESC LIMIT 2;",
          run: () => {
            const rows = filter(data.comment, r => r.rating >= 4);
            const sorted = sortBy(rows, "comment_date", "DESC").slice(0,2);
            return tableFrom(sorted);
          }
        }
      ],
      practice: {
        prompt: "請完成：找出 price >= 800 的商品，依價格由高到低，取前 3 筆，只顯示 productName、price。",
        answer: "SELECT productName, price FROM product WHERE price >= 800 ORDER BY price DESC LIMIT 3;",
        run: () => {
          const rows = filter(data.product, r => r.price >= 800);
          const sorted = sortBy(rows, "price", "DESC").slice(0,3);
          return tableFrom(selectCols(sorted, ["productName","price"]));
        }
      }
    }
  ];

  // -----------------------
  // 狀態（解鎖/完成）
  // -----------------------
  const state = {
    unlocked: 0,   // 已解鎖到哪個 index（包含）
    active: 0,     // 目前正在看的 index
    done: new Set()
  };

  // -----------------------
  // DOM
  // -----------------------
  const stepList = document.getElementById("stepList");
  const contentArea = document.getElementById("contentArea");
  const contentTitle = document.getElementById("contentTitle");
  const contentBadge = document.getElementById("contentBadge");
  const progressBar = document.getElementById("progressBar");
  const statusPill = document.getElementById("statusPill");
  const btnNext = document.getElementById("btnNext");
  const btnReset = document.getElementById("btnReset");

  // -----------------------
  // 工具：表格渲染
  // -----------------------
  function tableFrom(rows){
    if(!rows || rows.length === 0){
      return `<div class="result">（查無資料）</div>`;
    }
    const cols = Object.keys(rows[0]);
    let thead = `<tr>${cols.map(c=>`<th>${escapeHtml(c)}</th>`).join("")}</tr>`;
    let tbody = rows.map(r => {
      return `<tr>${cols.map(c=>`<td>${escapeHtml(String(r[c]))}</td>`).join("")}</tr>`;
    }).join("");
    return `<table><thead>${thead}</thead><tbody>${tbody}</tbody></table>`;
  }
  function escapeHtml(s){
    return s.replaceAll("&","&amp;").replaceAll("<","&lt;").replaceAll(">","&gt;").replaceAll('"',"&quot;").replaceAll("'","&#039;");
  }
  function selectCols(rows, cols){
    return rows.map(r => {
      const o = {};
      cols.forEach(c => o[c] = r[c]);
      return o;
    });
  }
  function filter(rows, fn){
    return rows.filter(fn);
  }
  function sortBy(rows, key, dir="ASC"){
    const sign = dir === "DESC" ? -1 : 1;
    rows.sort((a,b)=>{
      const av = a[key], bv = b[key];
      if(av === bv) return 0;
      return (av > bv ? 1 : -1) * sign;
    });
    return rows;
  }

  // -----------------------
  // UI：渲染左側步驟
  // -----------------------
  function renderSteps(){
    stepList.innerHTML = "";
    steps.forEach((s, idx) => {
      const isUnlocked = idx <= state.unlocked;
      const isDone = state.done.has(s.id);
      const isActive = idx === state.active;

      const badge = isDone ? `<span class="badge ok">已完成</span>`
                   : isActive ? `<span class="badge now">進行中</span>`
                   : isUnlocked ? `<span class="badge">可學習</span>`
                   : `<span class="badge lock">未解鎖</span>`;

      const btn = document.createElement("button");
      btn.className = "stepbtn";
      btn.disabled = !isUnlocked;
      btn.innerHTML = `
        <div class="left">
          <div class="num">${idx+1}</div>
          <div class="label">
            <div class="title">${s.title}</div>
            <div class="desc">${s.desc}</div>
          </div>
        </div>
        ${badge}
      `;
      btn.onclick = () => {
        state.active = idx;
        renderAll();
      };
      stepList.appendChild(btn);
    });
  }

  // -----------------------
  // UI：渲染右側內容
  // -----------------------
  function renderContent(){
    const s = steps[state.active];
    const isUnlocked = state.active <= state.unlocked;
    if(!isUnlocked){
      contentTitle.textContent = "尚未解鎖";
      contentBadge.textContent = "未解鎖";
      contentBadge.className = "badge lock";
      contentArea.innerHTML = `<div class="hint">請先完成前面的概念，才能解鎖本章。</div>`;
      return;
    }

    contentTitle.textContent = s.title;
    const isDone = state.done.has(s.id);
    contentBadge.textContent = isDone ? "已完成" : "進行中";
    contentBadge.className = isDone ? "badge ok" : "badge now";

    const explainHtml = s.explain.map(x => `<li>${escapeHtml(x)}</li>`).join("");
    const sampleBoxes = s.sqlSamples.map((item, i) => sampleBoxHtml(s.id, i, item.label, item.sql)).join("");

    const practiceId = `${s.id}_practice`;
    const practiceHtml = `
      <div class="box" style="margin-top:12px">
        <div class="bhd">
          <span>練習題</span>
          <span class="badge">${escapeHtml(s.tag)}</span>
        </div>
        <div class="bbd">
          <div class="note" style="margin:0 0 10px">${escapeHtml(s.practice.prompt)}</div>
          <textarea class="editor" id="${practiceId}" spellcheck="false" placeholder="在這裡輸入你的 SQL（例如：SELECT * FROM member;）"></textarea>
          <div class="actions">
            <button class="btn-accent" onclick="runPractice('${s.id}')">執行練習</button>
            <button onclick="showAnswer('${s.id}')">顯示參考答案</button>
          </div>
          <div id="${practiceId}_out" style="margin-top:10px"></div>
          <div class="okhint" id="${practiceId}_ok" style="display:none;margin-top:10px">
            ✅ 你已完成本概念！可以按「標記完成」解鎖下一章。
          </div>
        </div>
      </div>
    `;

    contentArea.innerHTML = `
      <div class="kicker">
        <span class="tag">${escapeHtml(s.tag)}</span>
        <span class="tag green">一步一步學</span>
      </div>

      <p class="note">本章重點：</p>
      <ul class="note" style="margin-top:-6px">${explainHtml}</ul>

      <div class="grid2">
        ${sampleBoxes}
      </div>

      ${practiceHtml}

      <div class="actions" style="margin-top:12px">
        <button class="btn-green" onclick="markDone()">標記完成</button>
        <button onclick="jumpToSqlTab()">提示：如何在 phpMyAdmin 執行</button>
      </div>

      <div class="hint">
        教學小技巧：讓學生先按「執行」看結果，再問他們：<br/>
        「這句 SQL 在做什麼？」→ 訓練口頭解釋能力。
      </div>
    `;

    // 預填練習框（讓學生不空白）
    const ta = document.getElementById(practiceId);
    ta.value = "";
  }

  function sampleBoxHtml(stepId, idx, label, sql){
    const runId = `${stepId}_sample_${idx}_out`;
    return `
      <div class="box">
        <div class="bhd">
          <span>${escapeHtml(label)}</span>
          <span class="badge">範例</span>
        </div>
        <div class="bbd">
          <pre><code>${escapeHtml(sql)}</code></pre>
          <div class="actions">
            <button class="btn-accent" onclick="runSample('${stepId}', ${idx})">執行</button>
            <button onclick="copyText(\`${escapeForTemplate(sql)}\`)">複製 SQL</button>
          </div>
          <div id="${runId}" style="margin-top:10px"></div>
        </div>
      </div>
    `;
  }

  function escapeForTemplate(s){
    // For template literal backticks safety
    return s.replaceAll("\\","\\\\").replaceAll("`","\\`").replaceAll("${","\\${");
  }

  // -----------------------
  // 執行（模擬）
  // -----------------------
  function runSample(stepId, idx){
    const s = steps.find(x => x.id === stepId);
    const out = document.getElementById(`${stepId}_sample_${idx}_out`);
    out.innerHTML = s.sqlSamples[idx].run();
  }

  function showAnswer(stepId){
    const s = steps.find(x => x.id === stepId);
    const ta = document.getElementById(`${stepId}_practice`);
    ta.value = s.practice.answer;
    ta.focus();
  }

  function normalizeSql(sql){
    return sql.trim().replace(/\s+/g," ").replace(/;+\s*$/,";");
  }

  function runPractice(stepId){
    const s = steps.find(x => x.id === stepId);
    const ta = document.getElementById(`${stepId}_practice`);
    const out = document.getElementById(`${stepId}_practice_out`);
    const ok = document.getElementById(`${stepId}_practice_ok`);

    const userSql = normalizeSql(ta.value);
    const ansSql  = normalizeSql(s.practice.answer);

    // 顯示結果（不管對錯都讓學生看到）
    out.innerHTML = s.practice.run();

    // 判斷是否符合參考答案（簡化版：完全相同）
    if(userSql.toLowerCase() === ansSql.toLowerCase()){
      ok.style.display = "block";
    } else {
      ok.style.display = "none";
      out.insertAdjacentHTML("beforebegin", `
        <div class="hint">
          你輸入的是：<code>${escapeHtml(userSql || "（空白）")}</code><br/>
          小提醒：注意表名/欄位、WHERE/ORDER BY/LIMIT 的順序，字串要加單引號。
        </div>
      `);
      // 避免重複提示堆疊：簡單做法，下一次再重繪
      setTimeout(()=>renderContent(), 50);
    }
  }

  function copyText(text){
    navigator.clipboard?.writeText(text).then(()=>{
      toast("已複製到剪貼簿");
    }).catch(()=>{
      alert("複製失敗，請手動選取複製。");
    });
  }

  function toast(msg){
    const div = document.createElement("div");
    div.textContent = msg;
    div.style.position = "fixed";
    div.style.left = "50%";
    div.style.bottom = "18px";
    div.style.transform = "translateX(-50%)";
    div.style.background = "rgba(0,0,0,.65)";
    div.style.border = "1px solid rgba(255,255,255,.12)";
    div.style.padding = "10px 12px";
    div.style.borderRadius = "12px";
    div.style.color = "#e5e7eb";
    div.style.zIndex = 9999;
    div.style.boxShadow = "0 10px 25px rgba(0,0,0,.35)";
    document.body.appendChild(div);
    setTimeout(()=>div.remove(), 1200);
  }

  // -----------------------
  // 完成/解鎖/進度
  // -----------------------
  function markDone(){
    const s = steps[state.active];
    state.done.add(s.id);

    // 解鎖下一章
    if(state.unlocked < steps.length - 1){
      state.unlocked = Math.max(state.unlocked, state.active + 1);
    }

    // 讓「下一個概念」可按
    btnNext.disabled = state.active >= state.unlocked;

    renderAll();
    toast("已標記完成 ✅");
  }

  function updateProgress(){
    const doneCount = state.done.size;
    const total = steps.length;
    statusPill.textContent = `進度：${doneCount} / ${total}`;
    const pct = Math.round((doneCount / total) * 100);
    progressBar.style.width = `${pct}%`;

    // next button
    btnNext.disabled = !(state.active < state.unlocked);
  }

  function renderAll(){
    renderSteps();
    renderContent();
    updateProgress();
  }

  // -----------------------
  // 額外：按鈕行為
  // -----------------------
  btnNext.addEventListener("click", ()=>{
    if(state.active < state.unlocked){
      state.active += 1;
      renderAll();
    }
  });

  btnReset.addEventListener("click", ()=>{
    if(!confirm("確定要重置進度嗎？（會清空完成紀錄與解鎖）")) return;
    state.unlocked = 0;
    state.active = 0;
    state.done = new Set();
    renderAll();
    toast("已重置");
  });

  function jumpToSqlTab(){
    alert("提示：到 phpMyAdmin → 選擇資料庫 firstdb → 點上方【SQL】→ 貼上 SQL → 執行。");
  }

  // 初始化
  renderAll();
</script>
</body>
</html>
