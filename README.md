# FUSION Restaurant - Full Stack E-commerce

Complete restaurant ordering system with menu management, order processing, and multiple payment gateways.

## 🚀 Features

✅ Beautiful responsive website (100% HTML/CSS)
✅ Full backend with Node.js + Express
✅ MongoDB database for menu, orders, reservations
✅ Payment integration (Click, PayMe, Stripe)
✅ Order tracking system
✅ Reservation management
✅ Multi-language support (UZ, RU)
✅ Mobile-friendly design

## 📁 Project Structure

```
FUSION-Restaurant/
├── fusion-restaurant.html    # Frontend
├── backend/
│   ├── server.js            # Main server
│   ├── package.json
│   ├── .env.example
│   ├── models/              # Database schemas
│   │   ├── MenuItem.js
│   │   ├── Order.js
│   │   └── Reservation.js
│   └── routes/              # API endpoints
│       ├── menu.js
│       ├── orders.js
│       ├── payments.js
│       └── reservations.js
└── docker-compose.yml       # Docker setup
```

## 🛠 Installation & Setup

### 1. Clone & Install
```bash
git clone https://github.com/yigitaliyevnodir47-sudo/FUSION-Resturant.git
cd FUSION-Resturant
cd backend
npm install
```

### 2. Environment Setup
```bash
cp .env.example .env
# Edit .env with your credentials
```

### 3. Start MongoDB
```bash
# Using Docker
docker-compose up -d

# Or local MongoDB
mongod
```

### 4. Run Server
```bash
npm run dev
```

Server runs on `http://localhost:5000`

## 📡 API Endpoints

### Menu
- `GET /api/menu` - All items
- `GET /api/menu/:id` - Item details

### Orders
- `POST /api/orders` - Create order
- `GET /api/orders/:orderId` - Get order
- `PATCH /api/orders/:orderId/status` - Update status

### Payments
- `POST /api/payments/click` - Click payment
- `POST /api/payments/payme` - PayMe payment
- `GET /api/payments/:orderId/status` - Check status

### Reservations
- `POST /api/reservations` - Book table
- `GET /api/reservations/phone/:phone` - Get reservations

## 💳 Payment Integration

### Click (Uzbekistan)
Popular for UZS payments
- Get merchant ID from Click
- Add to .env: CLICK_MERCHANT_ID, CLICK_SECRET_KEY

### PayMe (Uzbekistan)
Mobile wallet integration
- Register at payme.uz
- Add credentials to .env

### Stripe
International credit cards
- Get keys from stripe.com
- Add to .env: STRIPE_SECRET_KEY, STRIPE_PUBLIC_KEY

## 📱 Instagram Integration

1. Add link in Instagram bio → http://your-domain.com
2. Or create Instagram Stories with link stickers
3. Users can order directly from your restaurant page

## 🔗 Deployment

### Railway, Heroku, Render
```bash
git push heroku backend-development:main
```

### Self-hosted (VPS)
```bash
# Install Node.js & MongoDB
# Clone repository
# npm install & npm start
```

## 📞 Support

- **Phone**: +998 33 783 28 28
- **Instagram**: @restaurant__fusion
- **Location**: Nurafshon, Uzbekistan

## 📄 License

MIT - © 2025 FUSION Restaurant

---

**Ready to launch your e-commerce restaurant? Start with** `npm install && npm run dev`
