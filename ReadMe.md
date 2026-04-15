🚀 SendNow — Instant File Sharing Web App

«SendNow is a fast, self-hosted file sharing web application that lets you send files between devices instantly using a simple link or code — no login required.»

---

🌐 Try It Live

👉 https://sendnow.siddhart.qzz.io

---

✨ Features

⚡ Core Functionality

- 📂 Drag & Drop file upload
- 🔗 Instant shareable link generation
- 🔢 6-digit short code for quick access
- 📥 Clean download page with file info
- ⏳ Auto file expiry (temporary storage)

---

🔒 Security & Privacy

- Optional password protection
- Auto-delete files after expiry
- No permanent storage (ephemeral design)
- File size limits for safety

---

📊 User Experience

- Upload progress bar with speed indicator
- Mobile-friendly responsive UI
- “Copy link” button for quick sharing
- QR code generation for easy mobile access

---

🚀 Advanced (Optional Enhancements)

- 🔥 One-time download (self-destruct file)
- 📡 Real-time transfer (WebSockets / WebRTC)
- 📁 Multi-file upload support
- 📦 Auto zip multiple files
- 🧠 Smart compression (for large files)

---

🧠 How It Works

1. User uploads a file
2. Server stores it temporarily
3. A unique link + code is generated
4. Receiver opens link or enters code
5. File is downloaded
6. File is auto-deleted after expiry

---

🏗️ Tech Stack

Backend

- Node.js
- Express.js
- Multer (file upload handling)
- SQLite (metadata storage)

Frontend

- HTML
- TailwindCSS
- Vanilla JavaScript

Storage

- Local "/uploads" directory

---

📁 Project Structure

SendNow/
│
├── server.js
├── database.sqlite
├── uploads/
├── public/
│   ├── index.html
│   ├── upload.html
│   ├── download.html
│   ├── style.css
│   └── script.js
└── package.json

---

⚙️ Installation & Setup

1. Clone Repository

git clone https://github.com/yourusername/sendnow.git
cd sendnow

2. Install Dependencies

npm install

3. Run Server

node server.js

4. Open in Browser

http://localhost:3000

---

🌐 Deployment (Raspberry Pi + Tunnel)

Run on Raspberry Pi

node server.js

Expose using Cloudflare Tunnel

cloudflared tunnel --url http://localhost:3000

---

🔌 API Endpoints

Upload File

POST /upload

Download File

GET /d/:id

Delete File

DELETE /file/:id

---

⏳ Auto Deletion Logic

- Files are stored temporarily
- A background job deletes expired files
- Expiry options:
  - 10 minutes
  - 1 hour
  - 24 hours

---

📱 Use Cases

- Send files between phone & laptop
- Share large files quickly
- Temporary file hosting
- Replace USB / Bluetooth transfers
- Personal AirDrop alternative

---

⚠️ Limitations

- Not designed for permanent storage
- Large file uploads depend on server capacity
- No built-in user accounts (by design)

---

🔥 Future Roadmap

- Real-time peer-to-peer transfer (WebRTC)
- Device pairing system
- Clipboard integration (ClypSync)
- End-to-end encryption
- Progressive Web App (PWA)

---

🤝 Contributing

Pull requests are welcome. For major changes, open an issue first to discuss your ideas.

---

📄 License

MIT License

---

💡 Author Vision

SendNow is built to be:

- ⚡ Fast
- 🔒 Private
- 🧩 Simple

A tool you can deploy anywhere and use instantly — without friction.

---

⭐ Support

If you like this project:

- Star the repo ⭐
- Share it with others 🚀

---