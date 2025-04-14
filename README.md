# 🦙 Llama-On-The-Brows

Interface de terminal web para conversar com o modelo **LLaMA 3**, usando tanto a **API local do Ollama** quanto a **GROQ API** — tudo no navegador, com estilo, histórico e recursos extras!
![image](https://github.com/user-attachments/assets/00cf3ff1-8546-4036-91f1-d80811c3ca72)


![image](https://github.com/user-attachments/assets/39af5bdd-e5de-4572-96dc-14b846552d4c)

---

## ✅ Funcionalidades

- 🎯 Suporte a **Ollama local**
- ☁️ Suporte a **GROQ via API**
- 🔁 Histórico de comandos (setas ↑ ↓)
- 🛠️ Comando `/prompt` para alterar o prompt do sistema
- 💾 Comando `/save` para salvar sessões (em localStorage)
- 📂 Comando `/load` para carregar sessões salvas
- 📝 Exportação de sessões em **Markdown**
- 📄 Exportação em **PDF estilizado** (em breve)
- 🌗 Modo escuro/claro com toggle
- 📱 Responsivo (funciona no celular)

---

## 🚀 Como usar

### 1. Clonar ou baixar o projeto

```bash
git clone https://github.com/seu-usuario/terminal-llama.git
cd terminal-llama

### 2. Rodar localmente com Python (para evitar problemas de CORS)

python3 -m http.server
Acesse no navegador: http://localhost:8000

🔌 Integrações com APIs

🦙 Llama 3 via Ollama (Local)

Instale e rode o Ollama: https://ollama.com

Baixe o modelo LLaMA 3:

ollama run llama3


 A interface está configurada para se conectar a:

🧠 Comandos disponíveis
/help ou /? → Mostra todos os comandos

/prompt <texto> → Altera o prompt do sistema

/save → Salva a sessão atual

/load → Carrega uma sessão salva

/export → Exporta a conversa em Markdown

/clear → Limpa o terminal

📁 Estrutura do Projeto

terminal-llama/
├── index.html
├── style/
│   ├── main.css
│   └── main.scss (opcional)
├── js/
│   └── app.js
├── assets/
│   └── (ícones, fontes, etc.)
└── README.md

💡 Dicas
Sempre use http://localhost:8000 para evitar erro Failed to fetch por CORS.

Se quiser transformar isso num app de desktop, dá pra integrar com Electron!

O prompt personalizado é salvo junto com a sessão —










http://127.0.0.1:11434/api/chat
🌐 GROQ API
Obtenha uma chave de API em: https://console.groq.com

A interface usa o endpoint:

bash
Copiar
Editar
https://api.groq.com/openai/v1/chat/completions
