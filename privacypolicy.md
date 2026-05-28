# Doctor Who Dex Discord Bot - Privacy Policy

The following document explains what data is collected by Doctor Who Dex.

## Glossary

* **"Application"** or **"Discord application"** refers to the Discord bot user, its associated owners, and the servers it operates on.
* **"Data"** refers to data stored by this individual instance, including personal data.
* **"Bot"** or **"instance"** refers to the copy of the code running this specific Discord application, with its own independent database.
* **"Collectible"** refers to any virtual object that is meant to be collected through the bot, such as Doctor Who character/item cards, custom cosmetics, or future digital rewards.
* **"Application owners"** refers to the owners and developers of this specific Discord application who hold access to the application's authentication methods, server host, and database logs (`CharGoon26`).
* **"Doctor Who Dex Moderation Team"** or **"moderation team"** refers to the application owners and any community staff members chosen to help moderate the bot's features and official spaces.

---

## Open Source

The code of Doctor Who Dex is a modified instance of the open-source BallsDex framework, running under the MIT license. A copy of the license can be found below.

> Permission is hereby granted, free of charge, to any person obtaining a copy
> of this software and associated documentation files (the "Software"), to deal
> in the Software without restriction, including without limitation the rights
> to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
> copies of the Software, and to permit persons to whom the Software is
> furnished to do so, subject to the following conditions:

> The above copyright notice and this permission notice shall be included in all
> copies or substantial portions of the Software.

> THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
> IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
> FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
> AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
> LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
> OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
> SOFTWARE.

You may check the underlying open-source framework's source code to see how data structures are managed in addition to reading the policy below.

---

## What Data is Collected

Doctor Who Dex collects the following minimal data from the Discord API to execute its game mechanics:

* **User IDs:** Used as a unique key to safely identify your player profile inside our database.
* **Server (or Guild) IDs:** Used to save configurations necessary to the bot's operations, such as customized spawning intervals or tracking server trade logs.
* **Channel IDs:** Used to determine which specific channels within a server are designated for card spawns or system logging.

In addition, the following gameplay-specific data is generated, processed, and stored by Doctor Who Dex:

* The list of Doctor Who collectible cards owned by a user.
* A history of trades executed between users, including logging transaction pairs for account validation and security.
* Active state data for turn-based player matches via the `/battle` system (current card health percentages, accumulated action energy states, active status conditions, and overall match counts).
* **Ko-fi Transaction Identifiers:** If a user chooses to claim a premium card decoration, we temporarily process and record the **Ko-fi Transaction ID / Order URL** to securely verify payment and prevent duplicate redemptions of digital shop assets. No credit card numbers, legal names, or banking information are ever accessed or visible to our bot or team.

*Note regarding Message Content:* The bot does not cache or log chat messages. When a player types a name to catch a card, that message text is analyzed in memory for less than one second solely to register a successful catch and is immediately discarded. It is never stored on disk or accessible by administrators.

---

## How the Data is Stored

All persistent game data is safely stored on a secure **PostgreSQL database server** hosted via cloud infrastructure.

Interaction between the bot's core systems and the database is executed locally via the **Tortoise ORM** framework, ensuring your user profile information remains protected behind robust container network policies.

---

## Access to the Data

The only individuals permitted to directly interact with or access the underlying raw databases are the **Application Owners: @melanutella and @bigfatbrimmy on discord**.

General community moderators or trial staff members on our support platforms do not possess back-end database access. Data is strictly utilized to facilitate core game features and will never be made public, sold, or shared with external third parties.

---

## Your Rights

You have the right to review what data is connected to your profile or request its permanent erasure.

To delete your player profile, card inventory, battle statistics, and transaction logs permanently from our system, please submit a formal request via a support ticket in our [Official Support Server](https://discord.gg/AtdytZ5egm) or contact the developers directly on Discord at **@bigfatbrimmy** and **@melanutella**.
