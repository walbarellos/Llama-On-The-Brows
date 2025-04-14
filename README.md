## 🦙 Llama-On-The-Brows

Terminal Web Interativo para LLaMA 3: Converse com o modelo LLaMA 3 usando a API local do Ollama ou a API GROQ, diretamente no seu navegador. Desfrute de uma experiência completa com histórico de comandos, estilo personalizado e recursos extras!

![image](https://github.com/user-attachments/assets/00cf3ff1-8546-4036-91f1-d80811c3ca72)
![image](https://github.com/user-attachments/assets/39af5bdd-e5de-4572-96dc-14b846552d4c)

---

### ✅ Funcionalidades Principais

* **Integração Flexível:**
    * 🎯 Suporte para Ollama local
    * ☁️ Suporte para GROQ via API
* **Experiência de Terminal Aprimorada:**
    * 🔁 Histórico de comandos (navegue com as setas ↑ ↓)
    * 🛠️ Comando `/prompt <texto>`: Altere o prompt do sistema dinamicamente
    * 💾 Comando `/save`: Salve suas sessões de conversa no localStorage
    * 📂 Comando `/load`: Carregue sessões salvas anteriormente
    * 📝 Comando `/export`: Exporte seu histórico de conversa para o formato Markdown
    * 📄 Exportação para PDF estilizado (recurso em breve)
* **Interface Moderna e Adaptável:**
    * 🌗 Modo claro/escuro com alternância fácil
    * 📱 Design responsivo: Funciona perfeitamente em desktops e dispositivos móveis

---

### 🚀 Primeiros Passos

#### 1. Obtenha o Projeto

Clone o repositório ou baixe os arquivos do projeto:

```bash
git clone [https://github.com/seu-usuario/terminal-llama.git](https://github.com/seu-usuario/terminal-llama.git)
cd terminal-llama

Execute Localmente

Para evitar problemas de CORS, execute um servidor local simples com Python:

python3 -m http.server

Em seguida, abra o terminal no seu navegador através do seguinte link:
```bash
http://localhost:8000




3.📁 Estrutura do ProjetoA estrutura de arquivos do projeto é a seguinte:terminal-llama/ 
 ├── index.html 
 ├── style/ 
 │   ├── main.css 
 │   └── main.scss (opcional) 
 ├── js/ 
 │   └── app.js 
 ├── assets/ 
 │   └── (ícones, fontes, etc.) 
 └── README.md 

💡 Dicas ÚteisEvite erros de CORS:  

 Utilize sempre http://localhost:8000 para acessar o terminal e evitar problemas de segurança relacionados a CORS. 

 Transforme em app de desktop: Se desejar, você pode integrar o projeto com o Electron para criar uma aplicação de desktop. 

 Persistência do prompt: O prompt personalizado definido pelo comando /prompt é salvo junto com a sessão de conversa.


@walbarellos
