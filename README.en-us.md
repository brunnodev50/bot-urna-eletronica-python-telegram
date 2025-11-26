# 🗳️ Electronic Voting Bot (Telegram)

<div align="center">

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python&logoColor=white)
![Telegram](https://img.shields.io/badge/Telegram-Bot-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)
![SQLite](https://img.shields.io/badge/Database-SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)

<h3>
  <a href="README.md">🇧🇷 Leia em Português</a>
</h3>

</div>

---

## 🇺🇸 About
A Telegram bot that simulates an **Electronic Voting Machine**. It allows remote voting via the Telegram API, candidate management, and real-time vote counting.

### ✨ Key Features
* **Secure Admin Panel:** Protected by password to manage the election.
* **Voter Validation:** Uses CPF (ID) validation to ensure unique votes per person.
* **Election States:** Ability to Open, Close, and Reopen elections.
* **Real-time Reports:** Instant vote counting and results visualization.

---

## 🚀 Setup & Installation

1.  **Create the Bot:** Talk to [@BotFather](https://telegram.me/BotFather) on Telegram to create a new bot and get your **Token**.
2.  **Configure:** Add your token to the `token` variable in the code.
3.  **Install Dependencies:**
    ```bash
    pip install -r requirements.txt
    ```
4.  **Run:**
    ```bash
    python main.py
    ```

---

## 🛠️ Admin Commands
> **Default Password:** `1234`

| Command | Description |
| :--- | :--- |
| `/inserir_presidente` | Adds a new candidate to the election. |
| `/lista_presidentes` | Lists all registered candidates. |
| `/deletar_presidente` | Removes a candidate (Irreversible). |
| `/encerrar` | Closes the election and publishes results. |
| `/reabrir` | Reopens the election for more votes. |
| `/zerar_banco` | **Hard Reset:** Wipes the entire database. |

### 📸 Admin Screenshots
<details>
<summary>Click to view Admin Interface</summary>

**Add Candidate & List:**
<img src="https://github.com/user-attachments/assets/9d8402e9-6da0-4206-bca3-c3d493d5ecb4" width="45%">
<img src="https://github.com/user-attachments/assets/01b8e4be-4b7a-443a-8698-11935cfb365c" width="45%">

**Delete & Reopen:**
<img src="https://github.com/user-attachments/assets/a24e09c0-7056-4581-9b5a-382ac6f8e155" width="45%">
<img src="https://github.com/user-attachments/assets/b923c036-737c-4991-b659-d2c75b67ea9c" width="45%">

</details>

---

## 👤 User (Voter) Flow
1.  User starts with `/start`.
2.  Bot asks for **Name** and **CPF**.
3.  Bot checks if the user has already voted.
4.  User selects a candidate and confirms.

### 📸 Voter Screenshots
<details>
<summary>Click to view Voter Interface & Results</summary>

**Voting Process:**
<img src="https://github.com/user-attachments/assets/94069a55-e56f-425a-abf0-db0545315c83" width="45%">
<img src="https://github.com/user-attachments/assets/29c784c9-3415-492a-92f5-ae388610c707" width="45%">

**Election Results (After Closing):**
<img src="https://github.com/user-attachments/assets/5dfcd868-1b4b-4dca-9a43-76fd33887612" width="45%">
<img src="https://github.com/user-attachments/assets/46e08e72-299c-484a-b482-3a6c91c51530" width="45%">

</details>
