# Deployment

**teknik bağlamlar**

graphql

microservice

gpt-4

mysql

strapi

ant-design

tailwind-css

reactjs

nextjs

typescript

# CMS-Backend (Strapi)

Gereksinimler :  mysql

```bash
git clone https://github.com/fundamentai/launch-cms

cd launch-cms
npm i
```

Npm install yaptıktan sonra .env dosyası oluşturmamız gerekiyor.

```bash
HOST=0.0.0.0
PORT=1337
APP_KEYS="toBeModified1,toBeModified2"
API_TOKEN_SALT=tobemodified
ADMIN_JWT_SECRET=tobemodified
TRANSFER_TOKEN_SALT=tobemodified
JWT_SECRET=tobemodified

DATABASE_CLIENT=mysql
DATABASE_HOST=127.0.0.1
DATABASE_PORT=3306
DATABASE_NAME=fundamentai
DATABASE_USERNAME=user
DATABASE_PASSWORD=user123
DATABASE_SSL=false
JWT_SECRET=silelim-semtini-haritadan!

GPT_CONNECTOR="http://localhost"
```

Ardından

```bash
npm run develop
```

Strapi-CMS’miz çalışıyor!

```flow
Project information                                                          

┌────────────────────┬──────────────────────────────────────────────────┐
│ Time               │ Sun Feb 04 2024 11:18:35 GMT+0300 (GMT+03:00)    │
│ Launched in        │ 3251 ms                                          │
│ Environment        │ development                                      │
│ Process PID        │ 59742                                            │
│ Version            │ 4.19.1 (node v18.19.0)                           │
│ Edition            │ Community                                        │
│ Database           │ mysql                                            │
└────────────────────┴──────────────────────────────────────────────────┘

 Actions available                                                            

Welcome back!
To manage your project 🚀, go to the administration panel at:
http://localhost:1337/admin

To access the server ⚡️, go to:
http://localhost:1337
```

# Frontend - NEXTJS

```bash
git clone https://github.com/fundamentai/launch-site
npm i

touch src/config/config.ts
```

Oluşturduğumuz dosyaya config.example’daki değişkenleri uygun şekilde ekleyelim.

```tsx
export default {
    gql: 'http://localhost/wordpress/graphql',
    img_url: 'http://127.0.0.1:1337/',
    bearer: 'xxxx'
}
```

Ardından 

```bash
npm run dev
```

```objectivec
▲ Next.js 14.0.3
   - Local:        http://localhost:3000
   - Experiments (use at your own risk):
     · typedRoutes

 ✓ Ready in 2.4s
```