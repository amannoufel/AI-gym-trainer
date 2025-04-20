AI Trainer – Your Personalized Workout Companion 🏋️‍♂️🤖
AI Trainer is an intelligent, GUI-based fitness companion built with Python’s Tkinter. It combines real-time workout tracking with AI-powered guidance to offer a smart, personalized fitness experience. Users can log workouts, ask fitness-related questions, and review their progress — all within a sleek and interactive interface.

🚀 Features
🔐 User Authentication
Secure login and sign-up with persistent user profiles.

💪 Workout Tracking
Buttons for common exercises: curls, squats, push-ups, shoulder presses, bench presses.

Integration with an external module (gym2.py) that tracks repetitions — potentially using sensors or computer vision.

Automatically logs workouts with exercise type, rep count, and date.

📊 Workout History
Displays a scrollable log of past workouts, showing exercises performed, rep count, and timestamps.

🧠 AI-Powered Fitness Q&A
Users can ask fitness and health-related questions.

Utilizes Google’s Gemini Pro model to give intelligent, personalized responses based on user data (name, age, height, weight).

Interactive conversation with an "Ask Another" feature for follow-up questions.

🖥️ Intuitive and Visual Interface
Clean, user-friendly interface with custom images and smooth hover effects.

Navigation sidebar for seamless movement between different sections.

💾 Data Persistence
Uses MongoDB for securely storing user credentials and workout data.

🧩 Modular Code Design
Separated functions and logical structure make the codebase easy to maintain and extend.

🛠️ Tech Stack
Python 3.x – Core language

Tkinter – GUI development

Pillow (PIL) – Image handling

Pymongo – MongoDB integration

Google Generative AI API – AI-powered Q&A system

MongoDB – Cloud or local database storage

gym2.py – External module for rep tracking (likely using computer vision or sensors)

⚙️ Installation & Setup
1. Prerequisites
Ensure you have the following:

Python 3.x installed

MongoDB (local or Atlas cluster)

Google Cloud project with Gemini API enabled + API Key

gym2.py file in the same directory (for workout tracking)

Image assets in an images/ folder (used by the UI)

2. Install Dependencies
bash
Copy
Edit
pip install pillow pymongo google-generativeai
Note: tkinter is typically bundled with Python, but if it's not, install it via your package manager.

3. Configuration
MongoDB: Update the connection_string variable in main.py with your connection URI. Ensure your database is named aitrainer.

Google Gemini API: Replace the placeholder API key in main.py with your own.

Assets & Modules: Confirm that gym2.py and the images/ folder are in the correct directory.

4. Run the App
bash
Copy
Edit
python main.py
🧭 Usage Guide
Login / Sign Up: New users can register, while returning users can log in using existing credentials.

Home: Main dashboard with navigation buttons.

Workout: Select an exercise to start tracking. The app (via gym2.py) monitors and records your performance.

Question: Ask fitness-related questions. Responses are tailored to your profile using the Gemini AI model.

History: Scroll through your workout logs to review your progress.

Logout: Securely log out and return to the login screen.

💡 Future Improvements
Enhanced Rep Tracking: Improve gym2.py for more accurate and real-time feedback using computer vision or IMUs.

Input Validation & Error Handling: Better handling for network failures, bad input, and session timeouts.

Progress Visualizations: Graphs and charts to visualize progress over time.

Custom Exercises: Allow users to define and add their own workout types.

Voice Interaction: Use speech recognition for hands-free question answering and workout control.

Mobile Support: Port the app to Android using Kivy or a cross-platform toolkit.

