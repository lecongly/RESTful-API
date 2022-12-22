# RESTful API

This is a RESTful API built with Express and TypeScript, featuring authentication, product, category, payment and image routes.

## Getting Started

To get started, clone the repository and install the dependencies:

```
git clone https://github.com/lecongly/RESTful-API.git
cd RESTful-API
npm install # yarn
```

Add `.env` include variables as in the file `.env.example`

```
PORT=5000

NODE_ENV=development
BASE_DOMAIN=localhost
CLIENT_URL=http://localhost:3000

MONGODB_PATH=
MONGODB_USER=
MONGODB_PASSWORD=

ACTIVATION_TOKEN_SECRET=
ACCESS_TOKEN_SECRET=
REFRESH_TOKEN_SECRET=

MAILING_SERVICE_CLIENT_ID =
MAILING_SERVICE_CLIENT_SECRET =
MAILING_SERVICE_REFRESH_TOKEN =
SENDER_EMAIL_ADDRESS =

CLOUD_NAME =
CLOUD_API_KEY =
CLOUD_API_SECRET =
```

To start the API, run:

```
npm run build # yarn run build
npm start # yarn start
```

The API will be running on [http://localhost:5000](http://localhost:5000/).

## Endpoints

The API has the following endpoints:

### Authentication

- `POST /api/user/register`: Registers a new user.

- `POST /api/user/activation`: Activation account.

- `POST /api/user/login`: Logs in a user.

- `POST /api/user/refresh`: Refresh token for user.

- `POST /api/user/logout`: Logout a user.

- `POST /api/user/logout-all`: Logout a user all devices.

- `POST /api/user/forgot`: Forgot password for user.

### User
- `GET /api/user/me` : Returns user infor.

- `PATCH /api/user/update`: Updates a user.

- `PATCH /api/user/add_cart`:  Add products to cart user.

- `PATCH /api/user/wish_list`:  Add products to wishlist user.

### Admin
- `GET /api/user` : Returns a list of all users.

- `GET /api/user/:id`: Returns a user.

- `DELETE /api/user/delete`: Deletes a user.



### Categories

- `GET /api/categories`: Returns a list of all categories.
- `POST /api/categories`: Creates a new category.
- `GET /api/categories/:id`: Returns a single category.
- `PUT /api/categories/:id`: Updates a category.
- `DELETE /api/categories/:id`: Deletes a category.


### Products

- `GET /api/products`: Returns a list of all products.
- `POST /api/products`: Creates a new product.
- `GET /api/products/:id`: Returns a single product.
- `PUT /api/products/:id`: Updates a product.
- `DELETE /api/products/:id`: Deletes a product.

### Payments

- `GET /api/payments`: Returns a list af all payments for admin.

- `POST /api/payments`: Creates a payment.

### Image

- `POST /api/image/upload`: Upload image to cloud.

- `POST /api/image/remove`: Remove image from cloud .

## Built With

- [Express](https://expressjs.com/) - The web framework used
- [TypeScript](https://www.typescriptlang.org/) - A typed superset of JavaScript
- [MongoDB](https://www.mongodb.com/) - A NoSQL database 
- [Cloudinary](https://cloudinary.com/) - Store images

## Authors

- [Le Cong Ly](https://github.com/lecongly) - Software Engineer.

