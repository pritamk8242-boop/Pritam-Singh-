<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Fantasy Sports Game</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: Arial, sans-serif;
    }

    body {
      background: #0f172a;
      color: white;
      min-height: 100vh;
    }

    header {
      background: linear-gradient(90deg, #4f46e5, #7c3aed);
      padding: 20px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    header h1 {
      font-size: 28px;
    }

    .wallet {
      background: rgba(255,255,255,0.15);
      padding: 10px 18px;
      border-radius: 12px;
      font-weight: bold;
    }

    .hero {
      padding: 40px 20px;
      text-align: center;
    }

    .hero h2 {
      font-size: 42px;
      margin-bottom: 15px;
    }

    .hero p {
      color: #cbd5e1;
      max-width: 700px;
      margin: auto;
      line-height: 1.6;
    }

    .btn {
      display: inline-block;
      margin-top: 25px;
      background: #22c55e;
      padding: 14px 28px;
      border-radius: 12px;
      text-decoration: none;
      color: white;
      font-weight: bold;
      transition: 0.3s;
    }

    .btn:hover {
      transform: scale(1.05);
      background: #16a34a;
    }

    .matches {
      padding: 40px 20px;
    }

    .matches h3 {
      text-align: center;
      margin-bottom: 30px;
      font-size: 34px;
    }

    .match-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 20px;
      max-width: 1200px;
      margin: auto;
    }

    .match-card {
      background: #1e293b;
      border-radius: 20px;
      padding: 20px;
      box-shadow: 0 10px 20px rgba(0,0,0,0.3);
      transition: 0.3s;
    }

    .match-card:hover {
      transform: translateY(-8px);
    }

    .teams {
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin: 20px 0;
    }

    .team {
      text-align: center;
    }

    .team img {
      width: 70px;
      height: 70px;
      border-radius: 50%;
      object-fit: cover;
      margin-bottom: 10px;
    }

    .vs {
      font-size: 22px;
      font-weight: bold;
      color: #facc15;
    }

    .contest {
      background: rgba(255,255,255,0.08);
      padding: 12px;
      border-radius: 12px;
      margin-top: 15px;
    }

    .contest p {
      margin: 8px 0;
      color: #e2e8f0;
    }

    .join-btn {
      width: 100%;
      margin-top: 15px;
      border: none;
      background: #7c3aed;
      color: white;
      padding: 12px;
      border-radius: 10px;
      font-size: 16px;
      cursor: pointer;
      transition: 0.3s;
    }

    .join-btn:hover {
      background: #6d28d9;
    }

    .bottom-nav {
      position: fixed;
      bottom: 0;
      width: 100%;
      background: #111827;
      display: flex;
      justify-content: space-around;
      padding: 14px 0;
      border-top: 1px solid rgba(255,255,255,0.1);
    }

    .bottom-nav a {
      color: white;
      text-decoration: none;
      font-size: 14px;
      text-align: center;
    }

    footer {
      text-align: center;
      padding: 30px;
      margin-top: 30px;
      color: #94a3b8;
    }

    @media (max-width: 768px) {
      .hero h2 {
        font-size: 30px;
      }

      header {
        flex-direction: column;
        gap: 15px;
      }
    }
  </style>
</head>
<body>

<header>
  <h1>FantasyPro</h1>
  <div class="wallet">Wallet: ₹500</div>
</header>

<section class="hero">
  <h2>Play Fantasy Matches & Win Rewards</h2>
  <p>
    Join contests, create your dream team, earn rewards, and compete with players worldwide.
  </p>
  <a href="#matches" class="btn">Join Match</a>
</section>

<section class="matches" id="matches">
  <h3>Live Matches</h3>

  <div class="match-grid">

    <div class="match-card">
      <div class="teams">
        <div class="team">
          <img src="https://images.unsplash.com/photo-1546519638-68e109498ffc?q=80&w=500&auto=format&fit=crop" alt="Team A">
          <h4>IND</h4>
        </div>

        <div class="vs">VS</div>

        <div class="team">
          <img src="https://images.unsplash.com/photo-1517649763962-0c623066013b?q=80&w=500&auto=format&fit=crop" alt="Team B">
          <h4>AUS</h4>
        </div>
      </div>

      <div class="contest">
        <p>Prize Pool: ₹10,000</p>
        <p>Entry Fee: ₹49</p>
        <p>Spots Left: 128</p>
      </div>

      <button class="join-btn">Join Contest</button>
    </div>

    <div class="match-card">
      <div class="teams">
        <div class="team">
          <img src="https://images.unsplash.com/photo-1517466787929-bc90951d0974?q=80&w=500&auto=format&fit=crop" alt="Team C">
          <h4>ENG</h4>
        </div>

        <div class="vs">VS</div>

        <div class="team">
          <img src="https://images.unsplash.com/photo-1508098682722-e99c643e7f0b?q=80&w=500&auto=format&fit=crop" alt="Team D">
          <h4>PAK</h4>
        </div>
      </div>

      <div class="contest">
        <p>Prize Pool: ₹25,000</p>
        <p>Entry Fee: ₹99</p>
        <p>Spots Left: 56</p>
      </div>

      <button class="join-btn">Join Contest</button>
    </div>

  </div>
</section>

<footer>
  © 2026 FantasyPro Sports Platform
</footer>

<div class="bottom-nav">
  <a href="#">🏠<br>Home</a>
  <a href="#">🏆<br>Contest</a>
  <a href="#">💰<br>Wallet</a>
  <a href="#">👤<br>Account</a>
</div>

</body>
</html>
