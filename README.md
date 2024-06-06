[<img src="https://img.shields.io/badge/Telegram-%40Me-orange">](https://t.me/Hakimiqbal)


![img1](.github/images/demo.png)


## Functionality
| Functional                                                     | Supported |
|----------------------------------------------------------------|:---------:|
| Multithreading                                                 |     ✅     |
| Binding a proxy to a session                                   |     ✅     |
| Auto-purchase of items if you have coins (tap, energy, charge) |     ✅     |
| Random sleep time between clicks                               |     ✅     |
| Random number of clicks per request                            |     ✅     |
| Support tdata / pyrogram .session / telethon .session          |     ✅     |

## [Settings](https://github.com/JavaCrypt0/HamsterKombatBot_Python/blob/main/.env-example)
| Tuning                | Deskripsi                                                                                 |
|--------------------------|------------------------------------------------------------------------------------------|
| **API_ID / API_HASH**    | Platform data from which to launch a Telegram session _(stock - Android)_                |
| **MIN_AVAILABLE_ENERGY** | Minimum amount of available energy, upon reaching which there will be a delay _(eg 100)_ |
| **SLEEP_BY_MIN_ENERGY**  | Delay when reaching minimum energy in seconds _(eg [1800,2400])_                         |
| **AUTO_UPGRADE**         | Whether to upgrade the passive earn _(True / False)_                                     |
| **MAX_LEVEL**            | Maximum upgrade level _(eg 20)_                                                          |
| **BALANCE_TO_SAVE**      | Balance limit that the bot “won't touch” _(eg 1000000)_                                  |
| **UPGRADES_COUNT**       | The count of cards that the bot will upgrade in 1 lap _(eg 10)_                          |
| **APPLY_DAILY_ENERGY**   | Whether to use the daily free energy boost _(True / False)_                              |
| **APPLY_DAILY_TURBO**    | Whether to use the daily free turbo boost _(True / False)_                               |
| **RANDOM_CLICKS_COUNT**  | Random number of taps _(eg [50,200])_                                                    |
| **SLEEP_BETWEEN_TAP**    | Random delay between taps in seconds _(eg [10,25])_                                      |
| **USE_PROXY_FROM_FILE**  | Whether to use proxy from the `bot/config/proxies.txt` file (True / False)               |

## Quick Start 📚
1. To install libraries on Windows click on `INSTALL.bat`.
2. To start the bot use `START.bat` (or in console: `python main.py`).

## Prerequisites
Before you begin, ensure you have the following installed:
- [Python](https://www.python.org/downloads/) version 3.10 or 3.11

## Obtaining API Keys
1. Go to [my.telegram.org](https://my.telegram.org) and log in using your phone number.
2. Select **"API development tools"** and fill out the form to register a new application.
3. Note down the `API_ID` and `API_HASH` in `.env` file provided after registering your application.

## Installation
You can download [**Repository**](https://github.com/JavaCrypt0/HamsterKombatBot_Python) by cloning it to your system and installing the necessary dependencies:
```shell
~ >>> git clone https://github.com/JavaCrypt0/HamsterKombatBot_Python
~ >>> cd HamsterKombatBot

#Linux
~/HamsterKombatBot_Python >>> python3 -m venv venv
~/HamsterKombatBot_Python >>> source venv\bin\activate
~/HamsterKombatBot_Python >>> pip3 install -r requirements.txt
~/HamsterKombatBot_Python >>> cp .env-example .env
~/HamsterKombatBot_Python >>> nano .env # Here you must specify your API_ID and API_HASH , the rest is taken by default
~/HamsterKombatBot_Python >>> python3 main.py

#Windows
~/HamsterKombatBot_Python >>> python -m venv venv
~/HamsterKombatBot_Python >>> venv/Scripts/activate
~/HamsterKombatBot_Python >>> pip install -r requirements.txt
~/HamsterKombatBot_Python >>> copy .env-example .env
~/HamsterKombatBot_Python >>> # Specify your API_ID and API_HASH, the rest is taken by default
~/HamsterKombatBot_Python >>> python main.py
```

Also for quick launch you can use arguments, for example:
```shell
~/HamsterKombatBot_Python >>> python3 main.py --action (1/2)
# Or
~/HamsterKombatBot_Python >>> python3 main.py -a (1/2)

#1 - Create session
#2 - Run clicker
```
