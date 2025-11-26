# 🗳️ Bot Urna Eletrônica (Telegram)

<div align="center">

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python&logoColor=white)
![Telegram](https://img.shields.io/badge/Telegram-Bot-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)
![SQLite](https://img.shields.io/badge/Database-SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white)

<h3>
  <a href="README.md">🇺🇸 Read in English</a>
</h3>

</div>

---

## 🇧🇷 Sobre
Bot de Telegram que simula uma **Urna Eletrônica**. O sistema permite computar votos remotamente através da API do Telegram, gerenciar candidatos e gerar relatórios de apuração em tempo real.

### ✨ Funcionalidades
* **Painel Administrativo:** Protegido por senha para gestão da eleição.
* **Validação de Eleitor:** Exige Nome e CPF (voto único por CPF).
* **Estados da Eleição:** Comandos para Abrir, Encerrar e Reabrir a votação.
* **Relatórios em Tempo Real:** Visualização instantânea da apuração.

---

## 🚀 Instalação e Configuração

1.  **Criar o Bot:** Fale com o [@BotFather](https://telegram.me/BotFather) no Telegram para criar um bot e obter seu **Token**.
2.  **Configurar:** Adicione o token na variável correspondente dentro do código.
3.  **Instalar Dependências:**
    ```bash
    pip install -r requirements.txt
    ```
4.  **Rodar:**
    ```bash
    python main.py
    ```

---

## 🛠️ Comandos de Administrador
> **Senha Padrão:** `1234`

| Comando | Descrição |
| :--- | :--- |
| `/inserir_presidente` | Adiciona um novo candidato à eleição. |
| `/lista_presidentes` | Lista todos os candidatos cadastrados. |
| `/deletar_presidente` | Remove um candidato (Ação irreversível). |
| `/encerrar` | Encerra a eleição e libera os resultados para todos. |
| `/reabrir` | Reabre a eleição para novos votos. |
| `/zerar_banco` | **Reset Total:** Apaga todos os dados do banco de dados. |

### 📸 Telas do Administrador
<details>
<summary>Clique para ver as Telas de Admin</summary>

**Adicionar Candidato & Listar:**
<img src="https://github.com/user-attachments/assets/9d8402e9-6da0-4206-bca3-c3d493d5ecb4" width="45%">
<img src="https://github.com/user-attachments/assets/01b8e4be-4b7a-443a-8698-11935cfb365c" width="45%">

**Deletar & Reabrir:**
<img src="https://github.com/user-attachments/assets/a24e09c0-7056-4581-9b5a-382ac6f8e155" width="45%">
<img src="https://github.com/user-attachments/assets/b923c036-737c-4991-b659-d2c75b67ea9c" width="45%">

</details>

---

## 👤 Fluxo do Usuário (Eleitor)
1.  O usuário inicia com `/start`.
2.  O bot solicita **Nome** e **CPF**.
3.  O sistema verifica se o CPF já votou (impede votos duplicados).
4.  O usuário escolhe o candidato e confirma.

### 📸 Telas do Eleitor
<details>
<summary>Clique para ver a Votação e Resultados</summary>

**Processo de Votação:**
<img src="https://github.com/user-attachments/assets/94069a55-e56f-425a-abf0-db0545315c83" width="45%">
<img src="https://github.com/user-attachments/assets/29c784c9-3415-492a-92f5-ae388610c707" width="45%">

**Resultados da Apuração (Após Encerrar):**
<img src="https://github.com/user-attachments/assets/5dfcd868-1b4b-4dca-9a43-76fd33887612" width="45%">
<img src="https://github.com/user-attachments/assets/46e08e72-299c-484a-b482-3a6c91c51530" width="45%">

</details>
