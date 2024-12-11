

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MAGAICHINAMU M-PAISA MADA</title>
    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            background-color: #f4f4f4;
            color: #333;
        }

        header {
            background: #007BFF;
            color: #fff;
            padding: 20px 0;
        }

        .container {
            width: 80%;
            margin: auto;
            overflow: hidden;
        }

        nav ul {
            list-style: none;
            padding: 0;
        }

        nav ul li {
            display: inline;
            margin-right: 20px;
        }

        nav ul li a {
            color: #fff;
            text-decoration: none;
        }

        h1, h2 {
            text-align: center;
        }

        section {
            background: #fff;
            margin: 20px 0;
            padding: 20px;
            border-radius: 5px;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
        }

        form {
            display: flex;
            flex-direction: column;
        }

        input {
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #ccc;
            border-radius: 5px;
        }

        button {
            padding: 10px;
            background: #007BFF;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }

        button:hover {
            background: #0056b3;
        }

        footer {
            text-align: center;
            padding: 20px 0;
            background: #007BFF;
            color: #fff;
            position: relative;
            bottom: 0;
            width: 100%;
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <h1>MAGAICHINAMU M-PAISA MADA</h1>
            <nav>
                <ul>
                    <li><a href="#registration">Register</a></li>
                    <li><a href="#payment-method">Payment Methods</a></li>
                    <li><a href="#dashboard">Dashboard</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <main class="container">
        <!-- User Registration Form -->
        <section id="registration">
            <h2>User Registration</h2>
            <form id="registration-form">
                <input type="text" id="name" name="name" placeholder="Full Name" required>
                <input type="email" id="email" name="email" placeholder="Email Address" required>
                <input type="tel" id="phone" name="phone" placeholder="Phone Number" required>
                <input type="text" id="address" name="address" placeholder="Address" required>
                <input type="date" id="dob" name="dob" required>
                <button type="submit">Register</button>
            </form>
        </section>

        <!-- Payment Method Setup -->
        <section id="payment-method">
            <h2>Payment Method Setup</h2>
            <form id="payment-form">
                <input type="text" id="card-number" name="card-number" placeholder="Card Number" required>
                <input type="text" id="exp-date" name="exp-date" placeholder="MM/YY" required>
                <input type="text" id="cvv" name="cvv" placeholder="CVV" required>
                <input type="text" id="bank-account" name="bank-account" placeholder="Bank Account Number">
                <button type="submit">Save Payment Method</button>
            </form>
        </section>

        <!-- User Dashboard -->
        <section id="dashboard">
            <h2>User Dashboard</h2>
            <div id="transaction-overview">
                <h3>Your Transactions</h3>
                <ul>
                    <li>Transaction 1: $100 - Completed</li>
                    <li>Transaction 2: $50 - Pending</li>
                </ul>
            </div>
            <button onclick="alert('Manage Payment Methods')">Manage Payment Methods</button>
        </section>
    </main>

    <footer>
        <p>Customer Support: contact@paymentplatform.com</p>
    </footer>

    <script>
        document.getElementById('registration-form').addEventListener('submit', function(event) {
            event.preventDefault();
            alert('Registration successful!');
        });

        document.getElementById('payment-form').addEventListener('submit', function(event) {
            event.preventDefault();
            alert('Payment method saved!');
        });
    </script>
</body>
</html>
