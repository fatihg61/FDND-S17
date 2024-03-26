<script>
  function handleFastPayButtonClick() {
    window.location.href = "/paymentgood";
  }

  function handleCVVInput(event) {
    if (event.target.value.length > 3) {
      event.target.value = event.target.value.slice(0, 3);
    }
}
</script>

<body>
  <main>
    <div class="formfield">
      <form class="form">
        <div class="payment_other">
          <p>Fast Payment</p>
          <br />
          <button
            name="apple-pay"
            on:click={handleFastPayButtonClick}
            type="button"
            style="cursor: pointer;"
          >
            <svg
              xml:space="preserve"
              viewBox="0 0 512 210.2"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M93.6 27.1C87.6 34.2 78 39.8 68.4 39c-1.2-9.6 3.5-19.8 9-26.1 6-7.3 16.5-12.5 25-12.9 1 10-2.9 19.8-8.8 27.1m8.7 13.8c-13.9-.8-25.8 7.9-32.4 7.9-6.7 0-16.8-7.5-27.8-7.3-14.3.2-27.6 8.3-34.9 21.2-15 25.8-3.9 64 10.6 85 7.1 10.4 15.6 21.8 26.8 21.4 10.6-.4 14.8-6.9 27.6-6.9 12.9 0 16.6 6.9 27.8 6.7 11.6-.2 18.9-10.4 26-20.8 8.1-11.8 11.4-23.3 11.6-23.9-.2-.2-22.4-8.7-22.6-34.3-.2-21.4 17.5-31.6 18.3-32.2-10-14.8-25.6-16.4-31-16.8m80.3-29v155.9h24.2v-53.3h33.5c30.6 0 52.1-21 52.1-51.4s-21.1-51.2-51.3-51.2zm24.2 20.4h27.9c21 0 33 11.2 33 30.9s-12 31-33.1 31h-27.8zM336.6 169c15.2 0 29.3-7.7 35.7-19.9h.5v18.7h22.4V90.2c0-22.5-18-37-45.7-37-25.7 0-44.7 14.7-45.4 34.9h21.8c1.8-9.6 10.7-15.9 22.9-15.9 14.8 0 23.1 6.9 23.1 19.6v8.6l-30.2 1.8c-28.1 1.7-43.3 13.2-43.3 33.2 0 20.2 15.7 33.6 38.2 33.6m6.5-18.5c-12.9 0-21.1-6.2-21.1-15.7 0-9.8 7.9-15.5 23-16.4l26.9-1.7v8.8c0 14.6-12.4 25-28.8 25m82 59.7c23.6 0 34.7-9 44.4-36.3L512 54.7h-24.6l-28.5 92.1h-.5l-28.5-92.1h-25.3l41 113.5-2.2 6.9c-3.7 11.7-9.7 16.2-20.4 16.2-1.9 0-5.6-.2-7.1-.4v18.7c1.4.4 7.4.6 9.2.6"
              />
            </svg>
          </button>
          <button
            name="google-pay"
            on:click={handleFastPayButtonClick}
            type="button"
            style="cursor: pointer;"
          >
            <svg
              fill="none"
              viewBox="0 0 80 39"
              height="39"
              width="80"
              xmlns="http://www.w3.org/2000/svg"
            >
              <g clip-path="url(#a)">
                <path
                  fill="#5F6368"
                  d="M37.8 19.7V29h-3V6h7.8c1.9 0 3.7.7 5.1 2 1.4 1.2 2.1 3 2.1 4.9s-.7 3.6-2.1 4.9-3.1 2-5.1 2zm0-10.9v8h5c1.1 0 2.2-.4 2.9-1.2 1.6-1.5 1.6-4 .1-5.5l-.1-.1c-.8-.8-1.8-1.3-2.9-1.2zm18.9 4c2.2 0 3.9.6 5.2 1.8s1.9 2.8 1.9 4.8V29H61v-2.2h-.1c-1.2 1.8-2.9 2.7-4.9 2.7-1.7 0-3.2-.5-4.4-1.5-1.1-1-1.8-2.4-1.8-3.9q0-2.4 1.8-3.9c1.2-1 2.9-1.4 4.9-1.4 1.8 0 3.2.3 4.3 1v-.7c0-1-.4-2-1.2-2.6-.8-.7-1.8-1.1-2.9-1.1q-2.55 0-3.9 2.1l-2.6-1.6c1.6-2.1 3.7-3.1 6.5-3.1m-3.8 11.4c0 .8.4 1.5 1 1.9.7.5 1.5.8 2.3.8 1.2 0 2.4-.5 3.3-1.4 1-.9 1.5-2 1.5-3.2-.9-.7-2.2-1.1-3.9-1.1q-1.8 0-3 .9-1.2.75-1.2 2.1M80 13.3 70.1 36h-3l3.7-7.9-6.5-14.7h3.2l4.7 11.3h.1l4.6-11.3H80z"
                />
                <path
                  fill="#4285F4"
                  d="M25.9 17.7c0-.9-.1-1.8-.2-2.7H13.2v5.1h7.1c-.3 1.6-1.2 3.1-2.6 4v3.3H22c2.5-2.3 3.9-5.7 3.9-9.7"
                />
                <path
                  fill="#34A853"
                  d="M13.2 30.6c3.6 0 6.6-1.2 8.8-3.2l-4.3-3.3c-1.2.8-2.7 1.3-4.5 1.3-3.4 0-6.4-2.3-7.4-5.5H1.4v3.4c2.3 4.5 6.8 7.3 11.8 7.3"
                />
                <path
                  fill="#FBBC04"
                  d="M5.8 19.9c-.6-1.6-.6-3.4 0-5.1v-3.4H1.4c-1.9 3.7-1.9 8.1 0 11.9z"
                />
                <path
                  fill="#EA4335"
                  d="M13.2 9.4c1.9 0 3.7.7 5.1 2l3.8-3.8c-2.4-2.2-5.6-3.5-8.8-3.4-5 0-9.6 2.8-11.8 7.3l4.4 3.4c.9-3.2 3.9-5.5 7.3-5.5"
                />
              </g>
              <defs>
                <clipPath id="a">
                  <path fill="#fff" d="M0 0h80v38.1H0z" />
                </clipPath>
              </defs>
            </svg>
          </button>
        </div>
        <div class="separator">
          <hr class="line" />
          <p>OR</p>
          <hr class="line" />
        </div>
            <div class="card-info"> 
              <div class="input_container">
              <label class="input_label" for="cardHolderName">Cardholder Name</label>
              <input
                id="cardHolderName"
                class="input_field"
                type="text"
                name="cardHolderName"
                placeholder="Enter your full name"
                maxlength="50"
                required
                autocomplete="name"
              />
              <div class="input_container">
                <label class="input_label" for="cardNumber">Card Number</label>
                <input
                  id="cardNumber"
                  class="input_field"
                  type="text"
                  name="cardNumber"
                  placeholder="0000 0000 0000 0000"
                  pattern="[0-9]{16}"
                  maxlength="16"
                  required
                  autocomplete="cc-number"
                />
              </div>
              <div class="input_container">
                <label class="input_label" for="expiryDate">Expiry Date</label>
                <div class="split"></div>
                <input
                  id="expiryDate"
                  class="input_field"
                  type="month"
                  name="expiryDate"
                  placeholder="MM/YYYY"
                  min="2023-03"
                  max="2034-12"
                  style="width: 250px;"
                  required
                  autocomplete="cc-exp"
                />
              </div>
              <div class="input_container">
                <label class="input_label" for="cvv">CVV</label>
                <input
                  id="cvv"
                  class="input_field"
                  type="password"
                  name="cvv"
                  placeholder="CVV"
                  maxlength="3"
                  autocomplete="cc-csc"
                  on:input={handleCVVInput}
                />
              </div>
              <div class="input_container">
                <label class="input_label" for="donationType">Donation Type</label>
                <div class="split">
                  <select
                    id="donationType"
                    class="input_field"
                    style="width: 250px;"
                    autocomplete="donation-type"
                  >
                    <option value="">Select donation type</option>
                    <option value="material">Material</option>
                    <option value="financial">Financial</option>
                    <option value="clothing">Clothing</option>
                  </select>
                </div>
              </div>
              <div class="input_container">
                <label class="input_label" for="donationAmount">Donation Amount</label>
                <input
                  id="donationAmount"
                  class="input_field"
                  type="number"
                  name="donationAmount"
                  placeholder="$"
                  min="1"
                  required
                />
              </div>
              <a href="/paymentgood" class="checkout" style="cursor: pointer;">
                <span>Checkout</span>
              </a>
            </div>
        </form>
    </div>
  </main>
</body>

<style>
  @import url("https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,200;0,300;0,400;0,500;0,600;0,700;0,800;1,200;1,300&display=swap");
  main {
    height: 80vh;
    overflow: hidden;
    background: #5f5d5d;
    display: flex;
    align-items: center;
    justify-content: center;
    font-family: "Poppins";
  }

  body {
    background: #5f5d5d;
  }

  p {
    font-size: 12px;
    color: #575760;
    font-weight: 600;
  }

  .formfield {
    background: #ffffff;
    box-shadow:
      0px 187px 75px rgba(0, 0, 0, 0.01),
      0px 105px 63px rgba(0, 0, 0, 0.05),
      0px 47px 47px rgba(0, 0, 0, 0.09),
      0px 12px 26px rgba(0, 0, 0, 0.1),
      0px 0px 0px rgba(0, 0, 0, 0.1);
    border-radius: 16px;
    max-width: 450px;
  }
  .form {
    display: flex;
    flex-direction: column;
    gap: 15px;
    padding: 20px;
  }
  .payment_other {
    display: grid;
    grid-template-columns: 50% 50%;
    gap: 5px;
    padding: 10px;
    justify-content: center;
  }
  .payment_other button {
    height: 55px;
    background: #f2f2f2;
    border-radius: 11px;
    padding: 0;
    border: 0;
    outline: none;
  }
  .payment_other button svg {
    height: 18px;
  }
  .payment_other button:last-child svg {
    height: 22px;
  }

  .payment_other button:hover::before {
    transform: translate3d(100%, 0, 0);
  }
  .payment_other button:active {
    transform: scale(0.95);
  }

  .separator {
    width: calc(100% - 20px);
    display: grid;
    grid-template-columns: 2fr 1fr 2fr;
    gap: 10px;
    color: #575760;
    margin: 0 10px;
  }
  .separator p {
    display: block;
    text-align: center;
    font-weight: 600;
    font-size: 12px;
    margin: auto;
  }
  .separator .line {
    display: inline-block;
    width: 100%;
    height: 1px;
    border: 0;
    background-color: #e8e8e8;
  }
  .card-info {
    display: flex;
    flex-direction: column;
    gap: 10px;
  }
  .input_container {
    width: 100%;
    height: fit-content;
    display: flex;
    flex-direction: column;
    gap: 10px;
  }
  .split {
    display: grid;
    grid-template-columns: 4fr 2fr;
    gap: 10px;
  }

  .input_label {
    font-size: 12px;
    color: #575760;
    font-weight: 600;
  }
  .input_field {
    width: auto;
    height: 40px;
    padding: 0 0 0 16px;
    border-radius: 9px;
    outline: none;
    background-color: #f2f2f2;
    border: 1px solid #e5e5e500;
    transition: all 0.3s cubic-bezier(0.15, 0.83, 0.66, 1);
  }
  .input_field:focus {
    border: 1px solid transparent;
    box-shadow: 0px 0px 0px 2px #242424;
    background-color: transparent;
  }
  /* Reset input number styles */
  .input_field::-webkit-outer-spin-button,
  .input_field::-webkit-inner-spin-button {
    -webkit-appearance: none;
    margin: 0;
  }
  .checkout {
    position: relative;
    font-family: inherit;
    font-weight: 500;
    font-size: 18px;
    letter-spacing: 0.05em;
    border-radius: 0.8em;
    border: none;
    background: #302b63;
    color: ghostwhite;
    overflow: hidden;
  }
  .checkout span {
    position: relative;
    transition: color 0.6s;
    display: inline-flex;
    align-items: center;
    padding: 0.8em 1.2em 0.8em 1.05em;
    margin-left: 30%;
  }
  .checkout::before,
  .checkout::after {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
  }
  .checkout::before {
    content: "";
    background: #000;
    width: 120%;
    left: -10%;
    transform: skew(30deg);
    transition: transform 0.5s cubic-bezier(0.3, 1, 0.8, 1);
  }
  .checkout:hover::before {
    transform: translate3d(100%, 0, 0);
  }
  .checkout:active {
    transform: scale(0.95);
  }
</style>
