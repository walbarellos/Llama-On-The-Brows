# Llama-On-The-Brows

✅ Verificação rápida:
A seguir, um checklist para garantir que o terminal funcione corretamente com ambas as APIs:

1. Llama 3 via Ollama (Local)
Certifique-se de que o Ollama está rodando localmente:

bash
Copiar
Editar
ollama run llama3
A URL correta (http://127.0.0.1:11434/api/chat) está configurada. ✅

O corpo da requisição está no formato esperado:

json
Copiar
Editar
{
  "model": "llama3",
  "messages": [{ "role": "user", "content": "texto aqui" }],
  "stream": false
}
2. GROQ API
O endpoint está correto: https://api.groq.com/openai/v1/chat/completions. ✅

A requisição está bem montada com headers e body corretos.

A chave de API foi embutida corretamente no header Authorization.

🔧 Sugestão: Melhorar seleção do modelo para GROQ
Se você quiser deixar ainda mais flexível, pode permitir a seleção de modelos diferentes via botão ou comando /set model llama3-8b-8192. Mas como o GROQ já roda o LLaMA3-8b-8192 por padrão (geralmente com o nome "llama3-8b-8192"), isso pode ser só um detalhe.

No trecho abaixo, o modelName está fixo como "llama3":

js
Copiar
Editar
let modelName = 'llama3';
Você pode alterar isso para:

js
Copiar
Editar
let modelName = currentApi === 'groq' ? 'llama3-8b-8192' : 'llama3';
🧪 Teste rápido
Se você abrir o terminal web e digitar:

css
Copiar
Editar
Olá, qual a capital da França?
Com a API da Ollama: Verifique se o serviço está de fato rodando localmente.

Com a GROQ: Já vai funcionar direto — contanto que a chave esteja válida e sem rate limit.

2. 🔐 CORS bloqueando requisições
Como seu HTML está sendo servido provavelmente por file:// (ou algum outro host local), o navegador bloqueia chamadas cross-origin (CORS). A API local da Ollama não tem CORS liberado por padrão.

💡 Soluções:
🧪 Teste via servidor local (ex: usando o Python para servir o HTML):

bash
Copiar
Editar
python3 -m http.server
Depois acesse: http://localhost:8000/index.html

✅ Ou você pode liberar CORS na Ollama com um proxy (se quiser, posso montar isso).


✅ O que vai ter no projeto:
🔹 Interface web:
HTML5 moderno

CSS (com possibilidade de usar Sass se quiser customizar depois)

Layout bonitinho com terminal

Light/Dark Mode (com toggle)

🔹 Funcionalidades:
 Suporte a Ollama local

 Suporte a GROQ via API

 Histórico de comandos no terminal (teclas ↑ ↓)

 Comando /prompt para trocar prompt do sistema

 Comando /save para salvar a conversa em .md

 Comando /load para carregar sessões

 Botão para exportar a conversa em PDF

 Salvamento automático no localStorage

 Interface responsiva (pra celular também)

📁 Estrutura de arquivos:
css
Copiar
Editar
terminal-llama/
├── index.html
├── style/
│   ├── main.css
│   └── main.scss (opcional)
├── js/
│   └── app.js
├── assets/
│   └── icons, fontes, etc.
└── README.md
