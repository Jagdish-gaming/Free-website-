<h1>💸 Daily Earning Panel</h1>

<div class="card">
  <p><strong>Earn ₹20 per ad</strong><br>Minimum Withdrawal: ₹3000</p>
  <p>Today’s Earnings: ₹<span id="earning">0</span></p>
  <p>Ads Remaining: <span id="adsLeft">5</span></p>
  <button class="btn" onclick="watchAd()">Watch Ad</button>
</div>

<div class="card">
  <h2>Top Earning Apps</h2>
  <p><a href="https://play.google.com/store/apps/details?id=com.dream11.fantasy.cricket.app" target="_blank">Dream11</a></p>
  <p><a href="https://play.google.com/store/apps/details?id=com.phonepe.app" target="_blank">PhonePe Cashback</a></p>
  <p><a href="https://play.google.com/store/apps/details?id=com.google.android.apps.nbu.paisa.user" target="_blank">Google Pay Rewards</a></p>
  <p><a href="https://play.google.com/store/apps/details?id=com.cointiply.app" target="_blank">Cointiply - Watch Ads & Earn</a></p>
</div>

<script>
  let earnings = 0;
  let adsLeft = 5;

  function watchAd() {
    if (adsLeft > 0) {
      adsLeft--;
      let earned = Math.floor(Math.random() * (20 - 10 + 1)) + 10;
      earnings += earned;
      document.getElementById("earning").innerText = earnings;
      document.getElementById("adsLeft").innerText = adsLeft;

      alert("Ad watched! You earned ₹" + earned);
    } else {
      alert("No more ads for today. Come back tomorrow!");
    }
  }
</script># Free-website-
