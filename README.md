<div align="center">
    <img src="https://i.imgur.com/F60J2JS.png" alt="Discord Relay Bot" width="100" />
    <h1>UpgradedReservations</h1>
</div>

<div align="center">

[![Follow @saple1337](https://img.shields.io/badge/Follow-@saple1337-181717?style=for-the-badge&logo=github)](https://github.com/saple1337)
[![Star](https://img.shields.io/badge/Star-Repo-181717?style=for-the-badge&logo=github)](https://github.com/saple1337/UpgradedReservations)
[![Fork](https://img.shields.io/badge/Fork-Repo-181717?style=for-the-badge&logo=github)](https://github.com/saple1337/UpgradedReservations/fork)
[![Watch](https://img.shields.io/badge/Watch-Repo-181717?style=for-the-badge&logo=github)](https://github.com/saple1337/UpgradedReservations/subscription)
[![Buy Me a Coffee](https://i.imgur.com/mYcE2J8.png)](https://www.buymeacoffee.com/saple1337)

</div>

## **Table of Contents**
- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Configuration](#configuration)
- [Running the Bot](#running-the-bot)
- [Commands](#commands)
- [Contributing](#contributing)
- [Support](#support)
- [License](#license)

---

## **Introduction**

Welcome to **UpgradedReservations**—your go-to solution for efficiently managing nation reservations within Discord servers. Whether you're hosting an EU4 multiplayer session or a Hearts of Iron 4 campaign, this bot is designed to simplify the reservation process and enhance the overall experience for your community.

[**Invite the Bot to Your Server**](https://discord.com/oauth2/authorize?client_id=733588874500243486&scope=bot)  
*Click the link above to add the bot to your Discord server!*

---

## **Features**

- **Nation Reservations:** Effortlessly reserve nations across multiple supported game modes, ensuring a fair and organized process where no two users can reserve the same nation.
- **Dynamic Map Generation:** The bot automatically generates a visual map reflecting the current reservations, providing a clear and engaging way to view reservations.
- **Automated Cleanup:** To maintain an orderly server, the bot automatically removes expired reservations after 30 days, ensuring your channel remains clutter-free.
- **DM Notifications:** Enjoy personalized notifications delivered directly to your DMs, including error messages, reservation confirmations, and more.
- **Admin Privileges:** A comprehensive suite of admin commands allows you to manage reservations, view logs, and maintain the database with ease.

---

## **Installation**

Follow these simple steps to install and configure the UpgradedReservations on your local machine.

1. **Clone the Repository**

   Begin by cloning the repository to your local environment:

   ```git clone https://github.com/your-username/discord-reservation-bot.git```

2. **Install Dependencies**

   Ensure Python 3.7+ is installed, then proceed to install the required Python libraries:

   ```pip install -r requirements.txt```

3. **Create and Configure `config.json`**

   Next, create a `config.json` file in the root directory with the following structure:

   ```blank```

   Replace `YOUR_DISCORD_BOT_TOKEN` with your actual Discord bot token.

4. **Set Up the Database**

   The bot utilizes SQLite for managing reservations. The required tables will be automatically created when the bot is first run.

---

## **Configuration**

### **Data Files**

- `data/tags.json`: Maps country tags to nation names and pixel locations on the map for accurate visual representation.
- `data/country_colors.json`: Specifies nation colors for the `eu4` game mode, ensuring accurate map visuals.
- **Images:** Store your game mode-specific map images in the `images/` directory. The bot loads these images to generate the reservation map.

### **Environment Variables**

To ensure the bot operates smoothly, set the following environment variables:

- **TOKEN:** The bot token from your Discord Developer Portal.
- **DATABASE_URL:** The URL path to the SQLite database.

---

## **Running the Bot**

After setup, you can launch the bot using the following command:

```python main.py```

Once launched, the bot will connect to your Discord server and start listening for commands, ready to manage reservations.

---

## **Commands**

Below is a list of commands available in the UpgradedReservations:

- `!start [gamemode]`: Initiates the reservation process for the specified game mode. Must be executed before any reservations can be made.
- `!reserve [nation]`: Reserves a nation for yourself. This command can be used after the reservation process is initiated.
- `!reserve [nation] [user]`: Allows game managers to reserve a nation on behalf of another user.
- `!unreserve`: Cancels your current reservation. Game managers can also unreserve a nation for another user by mentioning them.
- `!delete`: Deletes all reservations and the logged game mode for the current channel. Only administrators are permitted to use this command.
- `!help`: Displays a comprehensive list of available commands and their descriptions.

---

## **Contributing**

We welcome and appreciate contributions to enhance UpgradedReservations. Here’s how you can contribute:

1. **Fork the Repository:** Use the "Fork" button at the top-right of the repository page.
2. **Clone Your Fork:** Clone the forked repository to your local machine.
3. **Create a New Branch:** Start a new branch for your specific feature or bugfix.
4. **Make Your Changes:** Implement your changes or bug fixes.
5. **Commit Your Changes:** Write a clear, descriptive commit message summarizing your changes.
6. **Push to Your Branch:** Push your changes to your forked repository.
7. **Submit a Pull Request:** Open a pull request on the original repository for review.

---

## **Support**

For assistance, feel free to join our [Discord server](https://discord.gg/zcu5aFwKGf) or open an issue on GitHub. We encourage contributions, feedback, and suggestions to continuously improve the bot.

---

## **License**

This project is licensed under the MIT License. Please refer to the LICENSE file for more details.

---
