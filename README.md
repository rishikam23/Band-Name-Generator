# Band Name Generator
[Live Demo](https://band-name-generator-6rn5.onrender.com/)

A simple and fun web application that generates random band names using **Node.js**, **Express** and **EJS templating**.

---

## Features

- Generates random band names using adjectives and nouns  
- Built with Express for fast server-side rendering  
- Uses EJS for dynamic templating  
- Clean and minimal UI with custom CSS  
- Dynamic footer with current year  

---

## Tech Stack

- **Backend:** Node.js, Express  
- **Templating Engine:** EJS  
- **Middleware:** Body-parser  
- **Frontend:** HTML, CSS  

---

## Project Structure

```
Band Generator project
│
├── public
│   └── styles
│       └── main.css
│
├── views
│   ├── partials
│   │   ├── header.ejs
│   │   └── footer.ejs
│   │
│   └── index.ejs
│
├── index.js
├── package.json
├── package-lock.json
```

---

## Installation & Setup

1. Clone the repository:
```bash
git clone https://github.com/rishikam23/Band-Name-Generator.git
```

2. Navigate to the project folder:
```bash
cd Band-Name-Generator
```

3. Install dependencies:
```bash
npm i
```

4. Start the server:
```bash
node index.js
```

5. Open your browser and go to:
```
http://localhost:3000
```

---

## How It Works

- The user clicks the **"Generate Name"** button  
- A POST request is sent to `/submit`  
- The server generates:
  - A random adjective  
  - A random noun  
- These values are passed to the EJS template  
- The generated band name is displayed dynamically  

---

## UI Overview

- Default screen shows:  
  **"Welcome to the Band Generator 🤟"**

- After clicking the button, it displays a randomly generated band name.

---

## Key Highlights

- Uses **EJS partials** (`header.ejs`, `footer.ejs`) for reusable layout  
- Dynamic year rendering in footer:
```ejs
<%= new Date().getFullYear() %>
```
- Clean separation of:
  - Logic (Express)
  - Views (EJS)
  - Styling (CSS)

---

## Author
**Rishika Mathur**
