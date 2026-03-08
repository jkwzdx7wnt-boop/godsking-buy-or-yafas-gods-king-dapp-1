# godsking-buy-or-yafas-gods-king-dapp-1
BUY NOW DAPP
<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>THE YAFA’S GOD’S KING 🤴🏾 • BUY NOW</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.6.0/css/all.min.css">
  <script src="https://cdn.jsdelivr.net/npm/canvas-confetti@1.9.3/dist/confetti.browser.min.js"></script>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700&family=Inter:wght@400;600;700&display=swap');
    body { font-family: 'Inter', sans-serif; }
    .hero-font { font-family: 'Playfair Display', serif; }
    .gold-glow { text-shadow: 0 0 40px #facc15, 0 0 80px #facc15; }
    .crown { animation: float 3s ease-in-out infinite; }
    @keyframes float { 0%,100% { transform: translateY(0); } 50% { transform: translateY(-15px); } }
    .ticker { background: linear-gradient(90deg, #111827, #1e1b4b); }
    .live-dot { animation: pulse 1.5s infinite; }
    @keyframes pulse { 0%,100% { opacity: 1; } 50% { opacity: 0.2; } }
    iframe { border-radius: 20px; box-shadow: 0 0 40px rgba(234,179,8,0.3); }
  </style>
</head>
<body class="bg-black text-yellow-300 min-h-screen overflow-x-hidden">

  <div class="max-w-6xl mx-auto">

    <!-- NAVBAR -->
    <nav class="sticky top-0 z-50 bg-black/90 backdrop-blur-lg border-b border-yellow-600 px-8 py-6 flex items-center justify-between">
      <div class="flex items-center gap-4">
        <span class="text-5xl crown">🤴🏾</span>
        <h1 class="hero-font text-3xl tracking-widest">GOD’S KING</h1>
      </div>
      <div class="flex gap-6">
        <a href="https://t.me/CropKingzCoinOfficial" target="_blank" class="flex items-center gap-2 hover:text-yellow-200 transition">
          <i class="fa-brands fa-telegram text-2xl"></i>
        </a>
        <button onclick="shareToX()" class="flex items-center gap-2 hover:text-yellow-200 transition">
          <i class="fa-brands fa-x-twitter text-2xl"></i>
        </button>
      </div>
    </nav>

    <!-- LIVE TICKER -->
    <div id="ticker" class="ticker px-8 py-5 flex flex-wrap items-center justify-center gap-x-12 gap-y-3 text-sm font-mono border-b border-yellow-700">
      <div class="flex items-center gap-2"><span class="w-3 h-3 bg-emerald-400 rounded-full live-dot"></span><span class="text-emerald-400 font-bold">LIVE</span></div>
      <div>Price: <span id="price" class="text-white">$0.00000000</span></div>
      <div>MCap: <span id="mcap" class="text-white">$0</span></div>
      <div>Liq: <span id="liq" class="text-white">$0</span></div>
      <div>Vol 24h: <span id="vol" class="text-white">$0</span></div>
      <div>5m: <span id="change5" class="text-emerald-400">0.00%</span></div>
      <div>1h: <span id="change1" class="text-emerald-400">0.00%</span></div>
      <div>24h: <span id="change24" class="text-emerald-400">0.00%</span></div>
      <a href="https://dexscreener.com/solana/5uEFua7ccmt6urkv1wDSUWkTedVFnud2LY3MKx9ypump" target="_blank" class="text-xs underline">DexScreener</a>
    </div>

    <!-- HERO -->
    <section class="text-center py-16 bg-gradient-to-b from-black via-purple-950 to-black relative overflow-hidden">
      <div class="absolute inset-0 opacity-10 pointer-events-none">🤴🏾🤴🏾🤴🏾</div>
      <p class="text-amber-400 tracking-[8px] text-xl mb-2">NOW BRINGING LIQUIDITY TO RAYDIUM 👀</p>
      <h1 class="hero-font text-7xl md:text-[110px] leading-none gold-glow mb-6">THE YAFA’S<br>GOD’S KING</h1>
      <p class="text-5xl mb-8">🥇💨🤴🏾🎖️ THE YAFA WAY</p>
      <div onclick="copyCA()" class="cursor-pointer inline-flex items-center gap-4 bg-black border-2 border-yellow-500 hover:border-yellow-300 mx-auto max-w-md rounded-3xl px-10 py-6 font-mono text-lg transition-all">
        <span id="ca-text" class="break-all">5uEFua7ccmt6urkv1wDSUWkTedVFnud2LY3MKx9ypump</span>
        <i class="fa-solid fa-copy text-2xl"></i>
      </div>
    </section>

    <!-- LIVE CHART -->
    <section class="px-6 py-12 bg-zinc-950">
      <h2 class="text-center text-4xl font-bold mb-8 flex items-center justify-center gap-3">
        <span>LIVE KING CHART</span> <span class="text-3xl">📈</span>
      </h2>
      <iframe id="chart-frame" width="100%" height="620" src="https://dexscreener.com/solana/5uEFua7ccmt6urkv1wDSUWkTedVFnud2LY3MKx9ypump?embed=1&theme=dark" frameborder="0"></iframe>
    </section>

    <!-- BUY CALCULATOR & BUTTONS -->
    <section class="px-8 py-20 bg-black">
      <div class="max-w-2xl mx-auto">
        <h2 class="text-5xl font-bold text-center mb-10">BUY NOW 💸</h2>

        <!-- CALCULATOR -->
        <div class="bg-zinc-950 border border-yellow-600 rounded-3xl p-8 mb-12">
          <p class="text-yellow-400 text-center mb-6">How much $GODSKING do you want?</p>
          <div class="grid grid-cols-2 gap-6">
            <div>
              <label class="block text-xs tracking-widest mb-2">YOU PAY (SOL)</label>
              <input id="solInput" type="number" value="1" step="0.01" onkeyup="calculateBuy()" class="w-full bg-black border border-yellow-500 rounded-2xl px-6 py-5 text-3xl focus:outline-none focus:border-yellow-400 font-mono">
            </div>
            <div>
              <label class="block text-xs tracking-widest mb-2">YOU RECEIVE ($GODSKING)</label>
              <div id="tokensOut" class="w-full bg-black border border-yellow-500 rounded-2xl px-6 py-5 text-3xl font-mono text-emerald-400">0.000000</div>
            </div>
          </div>
          <div class="text-center mt-6 text-sm text-yellow-400" id="usdEstimate">$0.00 USD</div>
        </div>

        <!-- BUY BUTTONS -->
        <div class="grid md:grid-cols-2 gap-6">
          <a onclick="buyClick(this)" href="https://www.pump.fun/5uEFua7ccmt6urkv1wDSUWkTedVFnud2LY3MKx9ypump" target="_blank" class="group bg-gradient-to-br from-amber-500 to-yellow-600 text-black font-black py-12 rounded-3xl text-3xl flex flex-col items-center justify-center hover:scale-105 transition-all">
            <span class="text-6xl mb-3">🚀</span> PUMP.FUN
          </a>
          <a onclick="buyClick(this)" href="https://jup.ag/swap?outputMint=5uEFua7ccmt6urkv1wDSUWkTedVFn
          
