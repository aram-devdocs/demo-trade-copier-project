Next.js Trade copier Binance

# Dev

npm install
npm run dev

- Deployment on server instructions

# Prep

Make copy of .env.template with proper API keys passed through.
Ensure mongoDB is live and working with proper schema

```shell
cd Binance-API-Trade-Copier
npm install // (If new package is required)
npm run build
```

# Pre-Deployment Check

```shell
pm2 ps // (Check to see if server is online )
pm2 delete 0 // (Should be instance 0, if other index sub 0)

```

# Deployment

```shell
pm2 --name Copier start npm -- start
```

Questions? Email aram.devdocs@gmail.com
