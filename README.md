# Auric Space

A modern, elegant social media blogging platform built with Node.js, Express, and MongoDB. Create personalized profiles, share posts with images, and interact with content through likes.

## ✨ Features

- **User Authentication**
  - Secure JWT-based authentication
  - Bcrypt password hashing
  - User registration and login
  - Session management with cookies

- **Profile Management**
  - Customizable user profiles
  - Avatar upload functionality
  - User statistics dashboard
  - Profile personalization

- **Post Management**
  - Create posts with text content and images
  - Edit existing posts
  - Delete posts
  - Like/unlike functionality
  - Image upload support

- **Beautiful UI**
  - Modern, luxury-themed design
  - Responsive layout with Tailwind CSS
  - Smooth animations and transitions
  - Glass-morphism effects

## 🛠️ Tech Stack

- **Backend**: Node.js, Express.js
- **Database**: MongoDB with Mongoose
- **Authentication**: JWT, bcrypt, cookie-parser
- **File Upload**: Multer
- **View Engine**: EJS
- **Styling**: Tailwind CSS
- **Font**: Google Fonts (Poppins)

## 📋 Prerequisites

Before you begin, ensure you have the following installed:

- [Node.js](https://nodejs.org/) (v14 or higher)
- [MongoDB](https://www.mongodb.com/try/download/community) (running locally on port 27017)

## 🚀 Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd auric-space
```

2. Install dependencies:
```bash
npm install
```

3. Make sure MongoDB is running on your machine:
```bash
# Windows
net start MongoDB

# macOS/Linux
sudo systemctl start mongod
```

4. Start the server:
```bash
node app.js
```

5. Open your browser and navigate to:
```
http://localhost:3000
```

## 📁 Project Structure

```
auric-space/
├── app.js              # Main application file
├── package.json        # Dependencies and scripts
├── .gitignore          # Git ignore rules
├── models/
│   ├── user.js        # User model schema
│   └── post.js        # Post model schema
├── views/
│   ├── index.ejs      # Registration page
│   ├── login.ejs      # Login page
│   ├── profile.ejs    # User profile page
│   └── edit.ejs       # Post edit page
└── public/
    └── uploads/       # Uploaded images directory
```

## 🔑 Configuration

The application uses default configuration:

- **Server Port**: 3000
- **MongoDB**: `mongodb://localhost:27017/mydatabase`
- **JWT Secret**: `secretkey` (⚠️ Change this in production!)

### Environment Variables (Recommended for Production)

Create a `.env` file for sensitive configuration:

```env
PORT=3000
MONGODB_URI=mongodb://localhost:27017/mydatabase
JWT_SECRET=your-secret-key-here
```

## 🎯 Usage

### Registration
1. Navigate to `http://localhost:3000`
2. Fill in your details (name, username, age, email, password)
3. Click "Register"

### Login
1. Go to `http://localhost:3000/login`
2. Enter your email and password
3. Click "Login"

### Creating Posts
1. After logging in, you'll be redirected to your profile
2. Scroll to "Create a New Post"
3. Add a title, content, and optionally an image
4. Click "Publish"

### Managing Posts
- **Like**: Click the "Like" button on any post
- **Edit**: Click "Edit" to modify post content or image
- **Delete**: Click "Delete" to remove a post

### Avatar Upload
1. On your profile page, click "Choose file" under your avatar
2. Select an image file
3. Click "Upload"

## 🔒 Security Features

- Password hashing with bcrypt
- JWT token-based authentication
- Secure session management
- File upload validation
- Authorization checks for post operations

## 🚧 Future Enhancements

- [ ] Comments system
- [ ] Follow/unfollow users
- [ ] Search functionality
- [ ] Real-time notifications
- [ ] Email verification
- [ ] Reset password feature
- [ ] Social media sharing
- [ ] Admin dashboard

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📝 License

This project is licensed under the ISC License.

## 👤 Author

Created with ❤️ by Raman

---

**Note**: Remember to replace `secretkey` with a strong, random secret in production environments!
