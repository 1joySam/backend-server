## Prerequisites

This starter has minimal prerequisites and most of these will usually already be installed on your computer.

- [Install Node.js](https://nodejs.org/en/download/)
- [Install git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
- [Install SQLite](https://www.sqlite.org/download.html)

## Setting up your store

- Install the Medusa CLI
  ```
  npm install -g @medusajs/medusa
  yarn global add @medusajs/medusa
  ```
- Run your project
  ```
  cd backend-server
  npm start
  ```
  npm install
  ```

Your local Medusa server is now running on port **9000**.

### Seeding your Medusa store

---

To seed your medusa store run the following command:

```
medusa seed -f ./data/seed.json
or npm seed
```

This command seeds your database with some sample datal to get you started, including a store, an administrator account, a region and a product with variants. What the data looks like precisely you can see in the `./data/seed.json` file.


Your local Medusa server is now running on port **9000**.

## Try it out

```
curl -X GET localhost:9000/store/products | python -m json.tool
```

After the seed script has run you will have the following things in you database:

- a User with the email: admin@medusa-test.com and password: supersecret
- a Region called Default Region with the countries GB, DE, DK, SE, FR, ES, IT
- a Shipping Option called Standard Shipping which costs 10 EUR
- a Product called Cool Test Product with 4 Product Variants that all cost 19.50 EUR

