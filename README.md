🦙 Llama-On-The-BrowsTerminal Web Interativo para LLaMA 3: Converse com o modelo LLaMA 3 usando a API local do Ollama ou a API GROQ, diretamente no seu navegador. Desfrute de uma experiência completa com histórico de comandos, estilo personalizado e recursos extras!


✅ Funcionalidades PrincipaisIntegração Flexível:
🎯 Suporte para Ollama local☁️ Suporte para GROQ via APIExperiência de Terminal Aprimorada:
🔁 Histórico de comandos (navegue com as setas ↑ ↓)
🛠️ Comando /prompt <texto>: Altere o prompt do sistema dinamicamente
💾 Comando /save: Salve suas sessões de conversa no localStorage
📂 Comando /load: Carregue sessões salvas anteriormente
📝 Comando /export: Exporte seu histórico de conversa para o formato Markdown
📄 Exportação para PDF estilizado (recurso em breve)Interface Moderna e Adaptável:
🌗 Modo claro/escuro com alternância fácil
📱 Design responsivo: Funciona perfeitamente em desktops e dispositivos móveis
🚀 Primeiros Passos1. 

Obtenha o ProjetoClone o repositório ou baixe os arquivos do projeto:
git clone https://github.com/seu-usuario/terminal-llama.git
cd terminal-llama


2. Execute LocalmentePara evitar problemas de CORS, execute um servidor local simples com Python:python3 -m http.server
Em seguida, abra o terminal no seu navegador através do seguinte link:http://localhost:8000

🔌 Configuração das APIs 🦙 LLaMA 3 via Ollama (Local)


Instale o Ollama: 
Siga as instruções de instalação em https://ollama.com
Execute o OllamaBaixe o modelo LLaMA 

ollama run llama3

A interface do terminal está configurada para se conectar ao seguinte endereço:

http://127.0.0.1:11434/api/chat


🌐 GROQ APIObtenha uma chave de API: Acesse https://console.groq.com para criar sua conta e obter sua chave de API.A interface utiliza o seguinte endpoint da API GROQ:https://api.groq.com/openai/v1/chat/completions

🧠 Comandos do TerminalO terminal oferece os seguintes comandos:/help ou /?: Exibe a lista de comandos disponíveis./prompt <texto>: Define um novo prompt de sistema para o LLaMA 

3


./save: Salva a sessão de conversa atual no armazenamento local do navegador
./load: Carrega uma sessão de conversa salva anteriormente
./export: Exporta o histórico da conversa para um arquivo Markdown
./clear: Limpa todo o conteúdo exibido no terminal
./version: Exibe a versão do LLaMA 

3.📁 Estrutura do ProjetoA estrutura de arquivos do projeto é a seguinte:terminal-llama/
├── index.html
├── style/
│   ├── main.css
│   └── main.scss (opcional)
├── js/
│   └── app.js
├── assets/
│   └── (ícones, fontes, etc.)
└── README.md

💡 Dicas ÚteisEvite erros de CORS: 

Utilize sempre http://localhost:8000 para acessar o terminal e evitar problemas de segurança relacionados a CORS.

Transforme em app de desktop: Se desejar, você pode integrar o projeto com o Electron para criar uma aplicação de desktop.

Persistência do prompt: O prompt personalizado definido pelo comando /prompt é salvo junto com a sessão de conversa.

![image](https://github.com/user-attachments/assets/00cf3ff1-8546-4036-91f1-d80811c3ca72)
![image](https://github.com/user-attachments/assets/39af5bdd-e5de-4572-96dc-14b846552d4c)



