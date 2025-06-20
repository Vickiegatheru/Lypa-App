<script>
  function handleDeposit() {
    alert("Deposit button clicked");
  }

  function handleWithdraw() {
    alert("Withdraw button clicked");
  }

  

 function handleLogin() {
  window.location.href = '/Login.html';
}

  function handleJoin() {
    alert("Join button clicked");
  }
</script>

<svelte:head>
  <link href="https://fonts.googleapis.com/css2?family=Barlow:wght@500&display=swap" rel="stylesheet" />
</svelte:head>

<style>
  :global(body) {
  margin: 0;
  padding: 0;
  width: 100%;
  height: auto;
  display: grid;
  grid-template-rows: auto;
  background: linear-gradient(180deg, #001C5E 0%, #084CA0 51%, #084698 100%);
}


  .title {
    display: grid;
    width: 100%;
  }

  #lower {
    display: grid;
    grid-template-columns: 1fr 1fr;
  }

  #lypa {
    grid-column-start: 1;
    font-family: sans-serif;
    font-style: italic;
    font-size: 250%;
    color: white;
    margin-top: 4%;
    margin-left: -75%;
  }

  .button {
    display: flex;
    flex-direction: row;
    align-items: start;
  }

  .btn {
    padding: 10px 20px;
    margin: 10px;
    font-size: 16px;
    cursor: pointer;
    border: none;
    margin-top: 6%;
    background-color: inherit;
    color: white;
  }

  .main {
    display: grid;
    grid-template-columns: 1fr 1fr;
    padding: 20px;
    height: 900px;
    width: 100%;
  }

  .column1 {
    display: grid;
    grid-template-rows: 1fr 1fr 1fr;
    height: 867.5px;
  }

  #sendMoney {
    grid-row-start: 2;
    background: linear-gradient(180deg, #68EB75 0%, #0D6DB8 100%);
    border-radius: 30px 90px 0px 0px;
    margin-left: 0%;
    width: 460px;
    height: 284px;
    margin-bottom: -15%;
  }

  #sendMoneyP {
    text-align: left;
    font: bold 73px/80px Paralucent, sans-serif;
    color: #FFFFFF;
    font-size: 300%;
    padding: 30px;
  }

  #paragraph0 {
    background: #FFFFFF;
    margin-left: 0%;
    margin-top: 0%;
    grid-row-start: 3;
  }

  #paragraph0a {
    padding: 3% 8%;
    text-align: left;
    font: 500 22px/35px 'Barlow', sans-serif;
    color: #142944;
    font-size: 120%;
  }

  #google {
    display: grid;
    grid-template-columns: 1fr 1fr;
    padding: 2% 8%;
  }

  #applestore img,
  #playstore img {
    width: 100%;
    max-width: 273px;
    height: auto;
  }

  .column2 {
    display: grid;
    height: 829px;
    width: 570px;
  }

  #paragraph1 {
    height: 829px;
    background: linear-gradient(180deg, #F5F8F9 0%, #D5DFE2 100%);
    box-shadow: 0px 3px 6px #0037BC34;
    padding: 20px;
    width: 572px;
  }

  #country {
    display: grid;
    place-items: center;
    height: 105px;
    background: #FFFFFF;
    box-shadow: 0px 3px 6px #0037BC34;
    border-radius: 53px;
    grid-template-columns: 1fr 4fr 1fr;
    margin-bottom: 40px;
  }
  #flag{margin-left: 5%;
    width: 70px;
    height: 40px;
  align-items: center;}

  #arab {
    font-size: 150%;
    font: 39px/41px Paralucent, sans-serif;
    color: #001C5E;
  grid-column-start: 2; }
  #triangle {
      width: 0;
      height: 0;
      border-left: 20px solid transparent;
      border-right: 20px solid transparent;
      border-top: 20px solid #FF5B87; 
      cursor: pointer;
      margin: 50px auto;
    }

  #receive {
    margin-left: -50%;
    font: 24px Paralucent, sans-serif;
    color: #001C5E;
  }

  #money3 {
    margin-left: -10%;
    font: 24px Paralucent, sans-serif;
    color: #001C5E;
  }

  #clicking {
    margin-left: 10%;
    font: 24px Paralucent, sans-serif;
    color: #142944;
  }

  #sendAmount,
  #receiveAmount {
    height: 105px;
    background: #FFFFFF;
    box-shadow: 0px 3px 6px #0037BC34;
    border-radius: 53px;
    display: grid;
    place-items: center;
    margin: 30px auto;
    grid-template-columns: 1fr 3fr;
  }
  #currencyC{
 grid-column-start: 1;
 display: grid;
 grid-template-columns: 2fr 1fr;
  }
  #currency{
    display: grid;
  font-size: 100%;
  grid-column-start: 1;
      color: #001C5E;
font-size: 200%;
  align-items: center;

  }
  #triangle2{
    grid-column-start: 2;
      width: 0;
      height: 0;
      border-left: 20px solid transparent;
      border-right: 20px solid transparent;
      border-top: 20px solid #FF5B87;
      cursor: pointer;
      margin: 50px auto;
    margin-left: 75%;
  }
  #money {
    grid-column-start: 2;
    font: 500 41px/41px Paralucent, sans-serif;
    color: #001C5E;
    text-align: left;
  margin-left: -30%; }

  #send {
  margin-left: 10%;
  width: 466px;
  height: 78px;
  background: #3DD29B;
  box-shadow: 0px 3px 6px #0037BC34;
  border-radius: 53px;

  display: flex;
  justify-content: center;   
  align-items: center;       
}

#sender {
  font: 41px Paralucent, sans-serif;
  color: #FFFFFF;

  margin: 0;
  height: auto;
}

#hands{
  margin-right: -59%;
  margin-top: -40.9%;
 
}
  .content {
    width: 100%;
    height: 940px;
    display: grid;
    grid-template-rows: 1fr 1fr 1fr 1fr;
    background: linear-gradient(180deg, #F5F8F9 0%, #E4E4E4 100%);
    box-shadow: 0px 3px 6px #0037BC34;
  }

  #payment,
  #lypaHelp {
    display: grid;
    justify-items: center;
    align-items: center;
    padding: 20px;
  }

  #paymentP {
    text-align: center;
    font: bold 86px Paralucent, sans-serif;
    color: #142944;
  }

  #lypaHelpP {
    font: 28px/45px Paralucent, sans-serif;
    text-align: center;
    color: #142944;
    margin-top: -4%;
  }

  #graphics {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    margin-top: -3%;
    padding: 0 10%;
  }

  #graphics > div {
    background: #FFFFFF;
    box-shadow: 0px 3px 6px #00000029;
    border-radius: 87px;
    display: grid;
    justify-items: center;
    width: 300px;
    height: 400px;
    margin: 0 auto;
  }

  #billPayments {
    font: 47px/41px Paralucent, sans-serif;
    color: #142944;
    text-align: center;
    font-size: 250%;
  }

  #product {
    width: 200px;
    height: 200px;
    margin-top: 50px;
  }

  .footer {
    display: grid;
    justify-items: center;
    text-align: center;
    padding: 60px 0;
  }

  #startP {
    font: bold 86px/83px Paralucent, sans-serif;
    color: #FFFFFF;
  }

  #greatP {
    font: bold 37px/36px Paralucent, sans-serif;
    color: #6AED75;
    margin-top: 40px;
    width: 80%;
    margin-left: 10%;
  }
</style>

<div class="title">
  <div id="lower">
    <p id="lypa">lypa</p>
    <div class="button">
      <button class="btn deposit" on:click={handleDeposit}>Deposit</button>
      <button class="btn withdraw" on:click={handleWithdraw}>Withdraw</button>
      <button class="btn login" on:click={handleLogin}>Login</button>
        <button class="btn join" on:click={handleJoin}>Join</button>
    </div>
  </div>
</div>

<div class="main">
  <div class="column1">
    <div id="sendMoney">
      <p id="sendMoneyP">Send Money To Your Loved Ones</p>
    </div>
    <div id="paragraph0">
      <p id="paragraph0a">
        You don’t need to download ten apps for your financial services.
        Use LYPA for everything.
        Send money from UAE to Kenya instantly and right from the LYPA
        app on your phone.
      </p>
      <div id="google">
        <div id="applestore">
          <img src="/Images/Image 94.png" alt="Apple Store" />
        </div>
        <div id="playstore">
          <img src="/Images/Image 95.png" alt="Play Store" />
        </div>
      </div>
    </div>
  </div>

  <div class="column2">
    <div id="paragraph1">
        <div id="country">       
          <img id="flag" src="/Images/flag.jpeg" alt="Bill Image" />


       <p id="arab">United Arab Emirates</p>
        <img id="triangle" src="" alt="Scroll Icon" />
      </div>

      <p id="receive">SEND AMOUNT</p>
      <div id="sendAmount">
        <div id="currencyC">
                  <p id="currency">
                   AED
                  </p>
              <img id="triangle2" src="" alt="Scroll Icon" />

           </div>


        <p id="money">10,000.00</p>
      </div>

      <p id="receive">RECEIVE AMOUNT</p>
      <div id="receiveAmount">
        <div id="currencyC">
                  <p id="currency">
                   KES
                  </p>
              <img id="triangle2" src="" alt="Scroll Icon" />

           </div> <p id="money">320,193.00</p>
      </div>

      <p id="money3">1 AED = 32.02 KES</p>

      <div id="send">
        <div id="sender">Send</div>
      </div>

      <p id="clicking">By clicking send, I agree with terms & policy</p>
    </div>
    <div id="hands">
  <img id="hands1" src="/Images/Image 83.png" alt="Hands image" width="250" height="250" />
    </div>
  </div>
</div>

<div class="content">
  <div id="payment">
    <p id="paymentP">All Your Payments In One Place</p>
  </div>

  <div id="lypaHelp">
    <p id="lypaHelpP">
      LYPA App helps with more than just sending money.
      You can easily make bill payments and even recharge mobile airtime instantly.
      All in one APP, Lypa App.
    </p>
  </div>

  <div id="graphics">
    <div id="bill">
      <img id="product" src="/Images/Image 96.png" alt="Bill Image" />
      <p id="billPayments">Bill Payments</p>
    </div>

    <div id="airtime">
      <img id="product" src="/Images/Image 97.png" alt="Airtime Image" />
      <p id="billPayments">Airtime Topup</p>
    </div>

    <div id="sendMoney2">
      <img id="product" src="/Images/Image 98.png" alt="Send Money" />
      <p id="billPayments">Send Money</p>
    </div>
  </div>

  <div id="space"></div>
</div>

<div class="footer">
  <div id="start">
    <p id="startP">Start Sending Money Stress Free</p>
  </div>
  <div id="great">
    <p id="greatP">Great Exchange Rates * Super Fast Transfers * Instant Payments</p>
  </div>
</div>
