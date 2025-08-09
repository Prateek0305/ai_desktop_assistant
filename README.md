# create_erica_project.py
# Paste & run this in a Python shell (or save and run: python create_erica_project.py)
import os
import textwrap

project_dir = "erica-assistant"
os.makedirs(project_dir, exist_ok=True)



    ## 🚀 Features
    - 🔍 **Wikipedia Search** – Get quick summaries from Wikipedia.
    - 🌐 **Open Websites** – YouTube, Google, or your custom links.
    - 🎵 **Play Music** – Launch songs from your PC.
    - ⏰ **Tell the Time** – Know the current time instantly.
    - 📧 **Send Emails** – Send emails via voice commands.
    - 💻 **Launch Applications** – Open Visual Studio Code or other apps.
    - 🛑 **Exit on Command** – Just say `"exit"` to stop Erica.

    ---

    ## 📂 Project Structure
    ```
    erica-assistant/
    │
    ├── erica.py          # Main program
    ├── requirements.txt  # Dependencies
    └── README.md         # This file
    ```

    ---

    ## 📦 Installation

    ### 1️⃣ Clone the Repository (or use the files created by this script)
    ```bash
    cd erica-assistant
    ```

    ### 2️⃣ Install Dependencies
    ```bash
    pip install -r requirements.txt
    ```

    **`requirements.txt`**
    ```
    pyttsx3
    SpeechRecognition
    wikipedia
    ```

    ---

    ## ▶️ Usage

    Run the script:
    ```bash
    python erica.py
    ```

    Then say commands like:
    - `"Wikipedia Python programming"`
    - `"Open YouTube"`
    - `"Play music"`
    - `"The time"`
    - `"Email to Prateek"`
    - `"Exit"`

    ---

    ## 📋 Voice Commands

    <table>
    <tr><th>Command</th><th>Action</th></tr>
    <tr><td><code>wikipedia &lt;query&gt;</code></td><td>Searches Wikipedia and reads a short summary</td></tr>
    <tr><td><code>open youtube</code></td><td>Opens YouTube in your browser</td></tr>
    <tr><td><code>open google</code></td><td>Opens Google in your browser</td></tr>
    <tr><td><code>campus</code></td><td>Opens a preset YouTube playlist</td></tr>
    <tr><td><code>play music</code></td><td>Plays an audio file from your PC</td></tr>
    <tr><td><code>the time</code></td><td>Tells you the current time</td></tr>
    <tr><td><code>open code</code></td><td>Opens Visual Studio Code</td></tr>
    <tr><td><code>email to prateek</code></td><td>Sends an email</td></tr>
    <tr><td><code>exit</code></td><td>Stops Erica</td></tr>
    </table>

    ---

    ## ⚙️ Configuration

    ### 🎵 Change Music Directory
    Edit this line in `erica.py`:
    ```python
    music_dir = r"D:\the world of 90s"
    ```

    ### 📧 Email Setup
    Replace the placeholders in `sendEmail()`:
    ```python
    server.login('your_email@gmail.com', 'your_password')
    server.sendmail('your_email@gmail.com', to, content)
    ```
    > **Note:** For Gmail, use an App Password (recommended) or configure SMTP access securely.

    ---

    ## 🛡️ Warnings
    - Requires **Windows** (uses `sapi5` voice engine).
    - Needs **microphone access**.
    - Email sending will fail if security settings block SMTP.

    ---

    ## 📜 License
    MIT License © 2025 Your Name
    """)

requirements_txt = textwrap.dedent("""\
    pyttsx3
    SpeechRecognition
    wikipedia
    """)

# write files
with open(os.path.join(project_dir, "erica.py"), "w", encoding="utf-8") as f:
    f.write(erica_code)

with open(os.path.join(project_dir, "README.md"), "w", encoding="utf-8") as f:
    f.write(readme_md)

with open(os.path.join(project_dir, "requirements.txt"), "w", encoding="utf-8") as f:
    f.write(requirements_txt)

print(f"Project files created in ./{project_dir}/")
print("Files:")
for fname in sorted(os.listdir(project_dir)):
    print(" -", fname)

print("""
Next steps:
1) Open the folder (cd erica-assistant).
2) Edit erica.py to set:
   - music_dir path
   - correct codePath for VS Code (if needed)
   - replace email placeholders in sendEmail() with your method of choice (use app passwords or environment variables).
3) Install dependencies:
   pip install -r requirements.txt
4) Run:
   python erica.py

If you want, I can:
- Add a config file template to store email safely (recommended).
- Convert email sending to use environment variables or a prompt at runtime (safer).
- Provide a version that logs recognized text to a file for debugging.
""")
