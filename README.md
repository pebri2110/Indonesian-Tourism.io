<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Indonesian Tourism</title>
    <style>
        body {
            background: grey;
            color: white;
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }

        header {
            background-image: url('background.jpg');
            background-size: cover;
            background-size: 100%;
            background-position: center;
            background-repeat: no-repeat;
            color: white;
            text-align: center;
            padding: 10px 0;
        }

        nav ul {
            list-style-type: none;
            padding: 0;
        }

        nav ul li {
            display: inline;
            margin-right: 20px;
        }

        nav a {
            color: white;
            text-decoration: none;
        }

        section {
            padding: 20px;
        }

        footer {
            background-image: url('background.jpg');
            background-size: cover;
            color: white;
            text-align: center;
            padding: 10px 0;
        }

        button {
            background-color: #4CAF50;
            color: white;
            padding: 10px 20px;
            border: none;
            cursor: pointer;
            margin-top: 20px;
        }

        #hotels {
            text-align: center;
        }

        #hotels h2 {
            font-size: 24px;
            margin-bottom: 20px;
        }

        #hotels p {
            margin-bottom: 20px;
        }

        #hotels .hotel {
            display: flex;
            justify-content: center;
            margin-bottom: 20px;
        }

        #hotels .hotel img {
            width: 200px;
            margin-right: 20px;
            border-radius: 8px;
        }

        #hotels .hotel strong {
            font-size: 18px;
        }

        #hotels .hotel div {
            flex: 1;
        }

        ul {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-around;
            list-style-type: none;
            padding: 0;
        }

        li {
            flex: 0 0 30%;
            margin: 10px;
            padding: 10px;
            border: 1px solid white;
        }

        img {
            width: 100%;
            height: auto;
        }

        .slideshow-container {
        position: relative;
        max-width: 800px;
        margin: auto;
        }

        .slides {
        display: block;
        width: 100%;
        height: auto;
        overflow: hidden;
        position: block;
        margin: 0 auto;
        }


        .prev, .next {
        position: absolute;
        top: 50%;
        transform: translateY(-50%);
        font-size: 20px;
        cursor: pointer;
        color: white;
        background-color: black;
        border: none;
        }

        .prev {
        left: 10px;
        }

        .next {
            right: 10px;
        }

        .clock {
            font-size: 15px;
            position: fixed;
            top: 10px;
            right: 10px;
            color: white;
        }
    </style>
</head>
<body>
    <header>
        <p><span class="clock"></span></p>
        <script>
            function updateClock() {
                const now = new Date();
                const days = ['Sunday', 'Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday'];
                const day = days[now.getDay()];
                const date = now.getDate();
                const month = now.getMonth() + 1;
                const year = now.getFullYear();
                const hours = now.getHours();
                const minutes = now.getMinutes();
                const seconds = now.getSeconds();
                
                const clock = document.querySelector('.clock');
                clock.textContent = `${day}, ${date}/${month}/${year} ${hours}:${minutes}:${seconds}`;
            }
            
            updateClock();
            setInterval(updateClock, 1000);
        </script>
        <h1>Indonesian Tourism</h1>
        <nav>
            <ul>
                <li><a href="#culture">Indonesian cultures</a></li>
                <li><a href="#tourism">Best Tourist Attractions</a></li>
                <li><a href="#hotels">Favorite Hotel List</a></li>
            </ul>
        </nav>
    </header>

    <section id="culture">
        <h2>Indonesian cultures</h2>
        <p>Indonesia is a country rich in diverse ethnic cultures. Every tribe in Indonesia has unique and interesting dances, ceremonies and traditions. Examples of traditional Indonesian dances include the Pendet Dance, Saman Dance, and Reog Dance. Traditional ceremonies such as the Tedak Siten Ceremony and the Balinese Omed-omedan Tradition are also part of the richness of Indonesian culture.</p>
    </section>

    <section id="tourism">
        <h2>Best Tourist Attractions</h2>
        <p>Indonesia has many of the best tourist attractions, from beautiful beaches such as Kuta Beach in Bali, to historical sites such as Borobudur Temple in Central Java. Apart from that, Indonesia also has amazing natural destinations such as Komodo National Park and Lake Toba. Each tourist spot offers different uniqueness and beauty.</p>
    </section>

    <section id="hotels">
        <h2>Favorite Hotel List</h2>
        <p>The following is a list of favorite hotels in Indonesia along with complete facilities, prices, addresses and other important information:</p>
        <ul>
            <li><strong>Ayana Villas Bali</strong><br>
                <div class="slideshow-container">
                    <div class="slides">
                        <img src="ayana.jpg">
                        <button class="prev" onclick="plusSlides(-1)">&#10094;</button>
                        <button class="next" onclick="plusSlides(1)">&#10095;</button>
                    </div>
                    <div class="slides">
                        <img src="ayana1.jpg">
                        <button class="prev" onclick="plusSlides(-1)">&#10094;</button>
                        <button class="next" onclick="plusSlides(1)">&#10095;</button>
                    </div>
                </div>
                Facilities: Swimming pool, restaurant, Poolside bar, fitness center, Dry cleaning service, 24-hour security guard<br>
                Price: Starting from IDR 18,000,000 per night<br>
                Address: Jl. Karang Mas Sejahtera, Jimbaran 83634 Indonesia<br></li>

            <li><strong>Padma Resort Ubud</strong><br>
                <div class="slideshow-container">
                    <div class="slides">
                        <img src="padma.jpg">
                        <button class="prev" onclick="plusSlides(-1)">❮ Prev</button>
                        <button class="next" onclick="plusSlides(1)">Next ❯</button>
                    </div>
                    <div class="mySlides">
                        <img src="padma1.jpg">
                        <button class="prev" onclick="plusSlides(-1)">&#10094;</button>
                        <button class="next" onclick="plusSlides(1)">&#10095;</button>
                    </div>
                </div>
                Facilities: Spa, meeting rooms, 24-hour room service, 24-hour security guard, Bar/lounge<br>
                Price: Starting from IDR 5,000,000 per night<br>
                Address: Banjar Carik, Puhu, Payangan 80572 Indonesia<br></li>

            <li><strong>Adiwana Bisma</strong><br>
                <div class="slideshow-container">
                    <div class="slides">
                        <img src="adiwana.jpg">
                        <button class="prev" onclick="plusSlides(-1)">❮ Prev</button>
                        <button class="next" onclick="plusSlides(1)">Next ❯</button>
                    </div>
                    <div class="mySlides">
                        <img src="adiwana1.jpg">
                        <button class="prev" onclick="plusSlides(-1)">&#10094;</button>
                        <button class="next" onclick="plusSlides(1)">Next ❯</button>
                    </div>
                </div>
                Facilities: Business center, airport shuttle, free breakfast, 24-hour security, Bar/lounge<br>
                Price: Starting from IDR 3,000,000 per night<br>
                Address: Jl. Bisma, Ubud 80571 Indonesia<br></li>
        </ul>
    </section>

    <script>
        var slideIndex = 1;
        showSlides(slideIndex);
    
        function plusSlides(n) {
            showSlides(slideIndex += n);
        }
    
        function showSlides(n) {
            var i;
            var slides = document.getElementsByClassName("slides");
            if (n > slides.length) { 
                slideIndex = 1;
            }
            if (n < 1) { 
                slideIndex = slides.length;
            }
            for (i = 0; i < slides.length; i++) {
                slides[i].style.display = "none";
            }
            slides[slideIndex - 1].style.display = "block";
        }
    </script>
    <form id="transactionForm" class="left-align" onsubmit="processTransaction(event)">
        <!-- Isi form transaksi -->
    </form>
    
    <footer>
        <h3>Transaction</h3>
        <p>Please fill out the form below to proceed with the transaction:</p>
        <form id="transactionForm" onsubmit="processTransaction(event)">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required><br><br>
            
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required><br><br>
            
            <label for="paymentMethod">Payment Method:</label>
            <select id="paymentMethod" name="paymentMethod" required>
                <option value="creditCard">Credit Card</option>
                <option value="bankTransfer">Bank Transfer</option>
                <option value="eWallet">E-Wallet</option>
            </select><br><br>
            
            <label for="amount">Transaction Amount:</label>
            <input type="number" id="amount" name="amount" required><br><br>
            
            <button type="submit">Make Transaction</button>
        </form>
    </footer>
    
    <script>
        function processTransaction(event) {
            event.preventDefault();
            
            const formData = new FormData(document.getElementById("transactionForm"));
            const name = formData.get("name");
            const email = formData.get("email");
            const paymentMethod = formData.get("paymentMethod");
            const amount = formData.get("amount");
            
            // Add your transaction process logic here, for example:
            alert(`Transaction process initiated for ${name}. Details sent to ${email}. Amount: ${amount}. Payment Method: ${paymentMethod}`);
        }
    </script>
    
</body>
</html>
