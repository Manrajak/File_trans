# FileNest : File Sharing Application

A full-stack file sharing platform built with **Node.js**, **Express**, **MongoDB**, **AWS S3**, and **React**.  
Easily upload, share, and manage files securely with expiring links, password protection, and cloud storage.

---

## Features

- User authentication (JWT)
- Secure file uploads to AWS S3
- Shareable short links with expiry and password protection
- Email notifications for file sharing
- QR code generation for file links
- Download tracking
- Responsive React frontend

---

## Tech Stack

- **Frontend:** React, Tailwind CSS
- **Backend:** Node.js, Express
- **Database:** MongoDB Atlas
- **Cloud Storage:** AWS S3
- **Email Service:** Nodemailer (Gmail SMTP)
- **Deployment:** Render (backend), Vercel (frontend)
- **Authentication** JWT (JSON Web Tokens)
- **Other:** Redux Toolkit, REST API, QR Code generation

---

## Getting Started

### 1. Clone the Repository

```sh
git clone https://github.com/Manrajak/File_trans.git
cd File_trans
```

### 2. Install Dependencies

#### Backend
```sh
cd server
npm install
```

#### Frontend
```sh
cd ../client
npm install
```

---

### 3. Environment Variables

Create a `.env` file in the `server` directory with the following content:

```env
MONGODB_URL=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret

AWS_ACCESS_KEY_ID=your_aws_access_key
AWS_SECRET_ACCESS_KEY=your_aws_secret_key
AWS_REGION=your_aws_region
AWS_BUCKET_NAME=your_s3_bucket_name

PORT=5600
BASE_URL=https://your-backend-url.com

MAIL_USER=your_email@gmail.com
MAIL_PASS=your_email_app_password

CLIENT_URL=https://your-frontend-url.com
```

**Note:**  
- Never commit your `.env` file to version control.
- Use [environment variables](https://12factor.net/config) for all secrets and credentials.

---

### 4. Running Locally

#### Backend
```sh
cd server
npm start
```

#### Frontend
```sh
cd client
npm start
```

---

### 5. Deployment

- **Backend:** Deploy to [Render](https://render.com/) or similar.
- **Frontend:** Deploy to [Vercel](https://vercel.com/) or similar.
- Update `BASE_URL` and `CLIENT_URL` in your `.env` files accordingly.

---

## Usage

1. Register and log in.
2. Upload files (with optional expiry and password).
3. Share the generated short link or QR code.
4. Recipients can download files via the share link.

---

## License

This project is licensed under the MIT License.

---

## Acknowledgements

- [AWS S3](https://aws.amazon.com/s3/)
- [MongoDB Atlas](https://www.mongodb.com/cloud/atlas)
- [Vercel](https://vercel.com/)
- [Render](https://render.com/)
- [React](https://react.dev/)
- [Express](https://expressjs.com/)

---

**Feel free to contribute or open issues!**