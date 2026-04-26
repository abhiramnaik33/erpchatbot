# Agent-ERP

Agent-ERP is a Flask-based web application that provides a 3D avatar assistant integrated into an academic ERP dashboard. It utilizes the Groq API with the `llama-3.1-8b-instant` model to generate role-specific responses and dynamic chart data based on simulated academic data.

## Features

- **Role-Based Access Control**: Simulates different academic roles including Student, Teacher, Head of Department (HOD), Dean/Director, and University Administration.
- **AI Avatar Assistant**: Interactive 3D avatar that answers queries contextually based on the authenticated user's role.
- **Dynamic Chart Generation**: The assistant can return structured chart data (Bar, Line, Pie charts) to visualize metrics like CGPA progression, attendance, and department performance.
- **Fast Inference**: Powered by Groq for near-instantaneous LLM responses.

## Prerequisites

- Python 3.8+
- Groq API Key

## Setup & Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/abhiramnaik33/erpchatbot.git
   cd erpchatbot
   ```

2. **Create a virtual environment (optional but recommended):**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install dependencies:**
   ```bash
   pip install flask flask-cors groq python-dotenv
   ```

4. **Environment Variables:**
   Create a `.env` file in the root directory and add your Groq API key:
   ```env
   GROQ_API_KEY=your_groq_api_key_here
   ```

5. **Run the Application:**
   ```bash
   python app.py
   ```
   The application will be available at `http://127.0.0.1:5000/`.

## Usage

- Navigate to the web interface.
- Send queries through the chat interface. The 3D avatar will respond with speech and potentially display charts.
- The system mocks role data. Ensure the correct role is passed to test different data scopes.
