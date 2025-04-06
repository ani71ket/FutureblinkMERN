# Email Marketing Flowchart App

A visual email marketing automation tool built with the MERN stack, React Flow, Agenda, and Nodemailer. This app allows users to design, schedule, and send email sequences using an intuitive drag-and-drop flowchart interface.

## Features

- Drag-and-drop flowchart builder using **React Flow**
  - Supports nodes for **Cold Email**, **Wait/Delay**, and **Lead Source**
- Save and manage flowchart sequences
- Email scheduling based on node timing using **Agenda**
- Email delivery via **Nodemailer**
- [POST] API endpoint to schedule emails
- Authentication (Bonus)
- Unit tests (Bonus)

## Tech Stack

- **Frontend:** React.js, React Flow
- **Backend:** Node.js, Express.js
- **Database:** MongoDB
- **Scheduler:** Agenda
- **Email:** Nodemailer

## Installation

```bash
# Clone the repo
git clone https://github.com/ani71ket/FutureblinkMERN.git
cd email-flowchart-app

# Install frontend dependencies
cd client
npm install

# Install backend dependencies
cd ../server
npm install
```

## Running the App

```bash
# Start the frontend
cd client
npm start

# Start the backend
cd ../server
npm run dev
```

## API Endpoint

`POST /api/schedule`

**Body:**
```json
{
  "email": "user@example.com",
  "subject": "Subject here",
  "body": "Email content here",
  "time": "2025-04-06T12:00:00Z"
}
```


