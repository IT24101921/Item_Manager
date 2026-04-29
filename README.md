# Item Manager Application

A full-stack web application for managing items with discount functionality.

## Project Structure

```
Item_Manager/
├── backend/
│   ├── controllers/
│   │   └── itemController.js
│   ├── models/
│   │   └── Item.js
│   ├── routes/
│   │   └── itemRoutes.js
│   ├── server.js
│   ├── package.json
│   ├── .env
│   └── README.md
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   │   ├── ItemForm.jsx
│   │   │   ├── ItemCard.jsx
│   │   │   └── Navbar.jsx
│   │   ├── pages/
│   │   │   ├── HomePage.jsx
│   │   │   ├── AddItemPage.jsx
│   │   │   └── EditItemPage.jsx
│   │   ├── api/
│   │   │   └── itemApi.js
│   │   ├── App.jsx
│   │   ├── main.jsx
│   │   └── styles.css
│   ├── vite.config.js
│   ├── package.json
│   ├── index.html
│   ├── README.md
│   └── .gitignore
├── .gitignore
└── README.md
```

## Features

- **Add Item**: Create new items with name, category, price, description, image URL, and discount percentage
- **View Items**: Display all items on home page with discount information
- **Edit Item**: Update item details including discount percentage
- **Delete Item**: Remove items from the system

## Tech Stack

### Backend
- Node.js + Express
- MongoDB Atlas (Cloud)
- Mongoose ODM
- Nodemon (Development)

### Frontend
- React + Vite
- React Router
- Axios (API calls)
- CSS

## Installation & Setup

### Backend Setup
```bash
cd backend
npm install
# Configure .env file with MongoDB URI
npm run dev
```

### Frontend Setup
```bash
cd frontend
npm install
npm run dev
```

## Environment Variables

### Backend (.env)
```
PORT=5000
MONGO_URI=mongodb+srv://username:password@cluster0.mongodb.net/?appName=Cluster0
```

## API Endpoints

- `GET /api/items` - Get all items
- `GET /api/items/:id` - Get item by ID
- `POST /api/items` - Create new item
- `PUT /api/items/:id` - Update item
- `DELETE /api/items/:id` - Delete item

## Author
[Your Name]

## License
MIT
