
# How to Deploy the Telegram Bot

## Prerequisites
Before proceeding, ensure you have the following:
- Python 3.x installed.
- Git installed (to clone the repository).


## For Windows Users

### 1. Install Python
- Download Python from [python.org](https://www.python.org/downloads/).
- During installation, make sure to check the box labeled "Add Python to PATH".
- After installation, verify Python is installed by running the following in Command Prompt:
  ```bash
  python --version
  ```

### 2. Install Git
- Download and install Git from [git-scm.com](https://git-scm.com/).
- During installation, select the default options.

### 3. Clone the Repository
- Open Command Prompt or Git Bash.
- Navigate to the directory where you want to store the bot code:
  ```bash
  cd C:\path\to\your\directory
  ```
- Clone the repository:
  ```bash
  git clone https://github.com/asish1346/sessionAshu.git
  ```
- Navigate into the project directory:
  ```bash
  cd sessionAshu
  ```

### 4. Install Dependencies
- Open Command Prompt or Git Bash in the sessionAshu directory.
- Install the required dependencies using pip:
  ```bash
  pip install -r requirements.txt
  ```

### 5. Run the Bot
- To run the bot on Windows:
  If you have the Python script (`bott.py`):
  ```bash
  python bott.py
  ```
  If you have the executable (`bott.exe`):
  ```bash
  bott.exe
  ```

The bot should now be running and ready to accept commands.

## For Linux Users (Ubuntu/Debian)

### 1. Update System and Install Python
Open a terminal and run the following commands to update your system and install Python:
```bash
sudo apt update
sudo apt install python3 python3-pip
```

### 2. Install Git
To install Git, run:
```bash
sudo apt install git
```

### 3. Clone the Repository
Navigate to the directory where you want to store the bot code and clone the repository:
```bash
git clone https://github.com/asish1346/sessionAshu.git
cd sessionAshu
```

### 4. Install Dependencies
Use pip to install the required dependencies:
```bash
pip3 install -r requirements.txt
```

### 5. Run the Bot
To run the bot:
```bash
python3 bott.py
```
The bot will start running in the terminal.

### 6. Keep the Bot Running in the Background
To keep the bot running after you close the terminal, use `tmux` or `screen`:

#### Using tmux:
```bash
sudo apt install tmux
tmux new -s mybot
python3 bott.py
```
Press `Ctrl+B` then `D` to detach from the session and keep it running.

#### Using screen:
```bash
sudo apt install screen
screen -S mybot
python3 bott.py
```
Press `Ctrl+A` then `D` to detach from the screen session.

You can reattach to the session with:
```bash
tmux attach -t mybot  # for tmux
screen -r mybot       # for screen
```


## Conclusion
Follow the above steps to deploy the Telegram bot on either Windows or Linux. If you face any issues, ensure that the environment variables and paths are set correctly, and check that all dependencies are installed.
