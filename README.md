# ladouce-cosmetique
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>LADOUCE COSMÉTIQUE</title>
    <style>
        /* Global Styles */
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #fef0f6; /* Fond rose clair */
        }
        
        header {
            background-color: #ff66b2; /* Rose principal */
            padding: 20px;
            text-align: center;
            color: white;
            border-bottom: 5px solid #ff3385; /* Une nuance plus foncée de rose */
        }

        header h1 {
            font-size: 36px;
            margin: 0;
            font-weight: bold;
            letter-spacing: 2px;
        }

        header p {
            font-size: 18px;
            font-style: italic;
        }

        /* Section produits */
        .product-section {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 20px;
            padding: 20px;
        }

        .product-card {
            background-color: white;
            border-radius: 15px;
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            text-align: center;
            padding: 20px;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            border: 1px solid #f1c6d8;
        }

        .product-card:hover {
            transform: scale(1.05);
            box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
        }

        .product-card img {
            width: 80%;
            border-radius: 10px;
            margin-bottom: 15px;
        }

        .product-card h2 {
            font-size: 20px;
            color: #ff3385; /* Couleur rose foncé */
            font-weight: bold;
            margin: 10px 0;
        }

        .product-card p {
            color: #777;
            font-size: 16px;
            margin-bottom: 10px;
        }

        .product-card .price {
            font-size: 18px;
            color: #ff66b2;
            font-weight: bold;
        }

        .product-card button {
            background-color: #ff3385;
            color: white;
            border: none;
            padding: 10px 20px;
            font-size: 16px;
            border-radius: 10px;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }

        .product-card button:hover {
            background-color: #e60073;
        }

        /* Footer */
        footer {
            background-color: #ff66b2;
            color: white;
            text-align: center;
            padding: 20px;
            position: relative;
            bottom: 0;
            width: 100%;
            font-size: 14px;
        }

        .footer-links a {
            color: white;
            text-decoration: none;
            margin: 0 15px;
            font-weight: bold;
        }

        .footer-links a:hover {
            text-decoration: underline;
        }

    </style>
</head>
<body>

    <!-- Header -->
    <header>
        <h1>LADOUCE COSMÉTIQUE</h1>
        <p>Explorez les produits cosmétiques qui vous subliment !</p>
    </header>

    <!-- Section des produits -->
    <div class="product-section">
        <!-- Product 1 -->
        <div class="product-card">
            <img src="https://via.placeholder.com/250x250" alt="Lipstick">
            <h2>Rouge à lèvres Luxe</h2>
            <p>Des teintes magnifiques pour toutes les occasions.</p>
            <div class="price">$25.99</div>
            <button onclick="addToCart('Rouge à lèvres Luxe')">Ajouter au panier</button>
        </div>

        <!-- Product 2 -->
        <div class="product-card">
            <img src="https://via.placeholder.com/250x250" alt="Crème hydratante">
            <h2>Crème Hydratante</h2>
            <p>Pour une peau douce et éclatante.</p>
            <div class="price">$19.99</div>
            <button onclick="addToCart('Crème Hydratante')">Ajouter au panier</button>
        </div>

        <!-- Product 3 -->
        <div class="product-card">
            <img src="https://via.placeholder.com/250x250" alt="Parfum">
            <h2>Parfum Sensuel</h2>
            <p>Une fragrance délicate qui vous accompagne toute la journée.</p>
            <div class="price">$35.00</div>
            <button onclick="addToCart('Parfum Sensuel')">Ajouter au panier</button>
        </div>

        <!-- Product 4 -->
        <div class="product-card">
            <img src="https://via.placeholder.com/250x250" alt="Mascara">
            <h2>Mascara Magnifique</h2>
            <p>Des cils plus longs et plus volumineux.</p>
            <div class="price">$15.50</div>
            <button onclick="addToCart('Mascara Magnifique')">Ajouter au panier</button>
        </div>

        <!-- Product 5 -->
        <div class="product-card">
            <img src="https://via.placeholder.com/250x250" alt="Fond de teint">
            <h2>Fond de Teint Parfait</h2>
            <p>Un teint naturel et uniforme.</p>
            <div class="price">$30.00</div>
            <button onclick="addToCart('Fond de Teint Parfait')">Ajouter au panier</button>
        </div>

        <!-- Product 6 -->
        <div class="product-card">
            <img src="https://via.placeholder.com/250x250" alt="Crayon à sourcils">
            <h2>Crayon à Sourcils</h2>
            <p>Redéfinissez vos sourcils avec précision.</p>
            <div class="price">$12.00</div>
            <button onclick="addToCart('Crayon à Sourcils')">Ajouter au panier</button>
        </div>

        <!-- Product 7 -->
        <div class="product-card">
            <img src="https://via.placeholder.com/250x250" alt="Huile nourrissante">
            <h2>Huile Nourrissante</h2>
            <p>Un soin intensif pour votre peau.</p>
            <div class="price">$22.50</div>
            <button onclick="addToCart('Huile Nourrissante')">Ajouter au panier</button>
        </div>

        <!-- Product 8 -->
        <div class="product-card">
            <img src="https://via.placeholder.com/250x250" alt="Blush">
            <h2>Blush Rosé</h2>
            <p>Pour un teint frais et lumineux.</p>
            <div class="price">$18.00</div>
            <button onclick="addToCart('Blush Rosé')">Ajouter au panier</button>
        </div>

        <!-- Product 9 -->
        <div class="product-card">
            <img src="https://via.placeholder.com/250x250" alt="Crème de jour">
            <h2>Crème de Jour</h2>
            <p>Pour un visage frais et protégé toute la journée.</p>
            <div class="price">$28.00</div>
            <button onclick="addToCart('Crème de Jour')">Ajouter au panier</button>
        </div>

        <!-- Product 10 -->
        <div class="product-card">
            <img src="https://via.placeholder.com/250x250" alt="Serum éclat">
            <h2>Sérum Éclat</h2>
            <p>Illuminez votre peau avec ce sérum magique.</p>
            <div class="price">$40.00</div>
            <button onclick="addToCart('Sérum Éclat')">Ajouter au panier</button>
        </div>
    </div>

    <!-- Footer -->
    <footer>
        <div class="footer-links">
            <a href="https://wa.me/237697111123" target="_blank">Contactez-nous sur WhatsApp</a> | 
            <a href="mailto:luccinbryan@gmail.com" target="_blank">Envoyez-nous un Email</a>
        </div>
        <p>&copy; 2024 LADOUCE COSMÉTIQUE</p>
    </footer>

    <!-- JavaScript -->
    <script>
        function addToCart(productName) {
            alert(productName + " a été ajouté à votre panier!");
        }
    </script>

</body>
</html>
