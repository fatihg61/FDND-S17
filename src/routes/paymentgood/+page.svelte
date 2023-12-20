<script>
</script>
  
<main>
    <div class="container">
        <div class="heading">
            <div class="tick-container">
                <i class="tick"></i>
            </div>
            <span>Your payment is successful</span>
        </div>
        <div class="text-container">
            <div>
                <p>You will be logged out of all devices except this one.</p>
            </div>
            <div>You will be redirected to the website in 5 seconds.</div>
            <div>Click the button below if you are not redirected to the website.</div>
            <a class="primary-button" href="/">Go to Website</a>
        </div>
    </div>
</main>
  
<style>
/* Your CSS styles */
*,
*::after,
*::before {
    box-sizing: border-box;
    font-family: sans-serif;
}

main{
    margin: 0;
    text-align: center;
    font-family: sans-serif;
}

.container {
    color: #fff;
    margin: auto;
    padding: 32px 16px 16px;
}

.heading {
    font-size: 1.5rem;
    display: flex;
    align-items: center;
    flex-direction: column;
    margin-bottom: 32px;
}

.tick-container {
    padding: 20px;
    border-radius: 100px;
    height: 56px;
    width: 56px;
    display: inline-flex;
    justify-content: center;
    align-items: center;
    background: #fff;
    margin-bottom: 12px;
}

.tick {
    display: inline-block;
    transform: rotate(45deg);
    height: 36px;
    width: 18px;
    border-bottom: solid 3px #2196f3;
    border-right: solid 3px #2196f3;
    margin-bottom: 8px;
}

.text-container {
    line-height: 1.8em;
}

.primary-button {
    color: #2196f3;
    background-color: #fff;
    padding: 12px 16px;
    display: inline-block;
    margin-top: 32px;
    border-radius: 6px;
    text-decoration: none;
    text-transform: uppercase;
}

</style>