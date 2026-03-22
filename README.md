# BigBasketVoucherHub Bot 🤖

A powerful Telegram bot for selling BigBasket voucher codes with admin panel, payment verification, and order management.

## 🚀 Setup

### 1. Create a new Telegram Bot
- Message @BotFather → /newbot
- Set name: BigBasket Voucher Hub
- Set username: BigBasketVoucherHub_Bot
- Copy the bot token

### 2. Create Telegram Channels
- Main channel: @BigBasketVoucherHub
- Orders channel: @BigBasketOrders (or any name)
- Add the bot as **admin** to both channels

### 3. Install Dependencies
```bash
npm install
```

### 4. Configure `.env`
```
BOT_TOKEN=your_new_bot_token
ADMIN_ID=8004114088
DATABASE_URL=your_postgresql_url
WEBHOOK_URL=https://your-app.onrender.com
MAIN_CHANNEL_ID=-100xxxxxxxxx
ORDERS_CHANNEL_ID=-100xxxxxxxxx
```

### 5. Deploy to Render
- Push to GitHub
- Connect repo to Render
- Set all env vars
- Deploy!

## 📋 Order ID Format
BBH-XXXXXXXXXX-XXXXXX

## 💰 Price Setup
Admin Panel → Prices → Select category → Add/Update Tier
Format: `QUANTITY PRICE` e.g. `1 149`

## 🛡 Features
- Force channel membership
- Duplicate UTR detection
- Order ID tied to Telegram account
- 2-hour recovery window
- Auto temp-unblock via cron
- BharatPay optional auto-verification
