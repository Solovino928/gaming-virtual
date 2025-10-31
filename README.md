# Stripe Payments Web

This project is a simple web application that allows users to make payments using Stripe. It charges a fee of $10 to credit cards for verification purposes.

## Project Structure

```
stripe-payments-web
├── public
│   ├── index.html        # Payment page with Stripe integration
│   ├── success.html      # Page displayed upon successful payment
│   └── cancel.html       # Page displayed if payment is canceled
├── src
│   └── server.js         # Node.js server for handling backend operations
├── .env.example           # Template for environment variables
├── package.json           # npm configuration file
└── README.md              # Project documentation
```

## Setup Instructions

1. **Clone the repository:**
   ```bash
   git clone <repository-url>
   cd stripe-payments-web
   ```

2. **Install dependencies:**
   Make sure you have Node.js installed. Then run:
   ```bash
   npm install
   ```

3. **Configure environment variables:**
   Copy the `.env.example` file to `.env` and fill in your Stripe secret key:
   ```
   STRIPE_SECRET_KEY=your_secret_key_here
   ```

4. **Start the server:**
   Run the following command to start the Node.js server:
   ```bash
   node src/server.js
   ```

5. **Access the application:**
   Open your browser and go to `http://localhost:3000` to access the payment page.

## Usage

- Click the "Verificar ahora" button on the payment page to initiate the payment process.
- Upon successful payment, you will be redirected to the success page.
- If the payment is canceled, you will be redirected to the cancel page.

## License

This project is licensed under the MIT License.