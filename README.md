# 📈 Protótipo de Site Financeiro com React + Flask

Este projeto exibe dados de ações da B3 com indicadores fundamentalistas, gráficos e ranking, usando a [API da brapi.dev](https://brapi.dev/).

## 🚀 Tecnologias

- Frontend: React + Tailwind + Chart.js
- Backend: Flask (Python)
- API: [brapi.dev](https://brapi.dev)

---

## 📦 Como Rodar Localmente

### 1. Instale as dependências do backend Python

```bash
pip install -r requirements.txt
```

### 2. Gere o build do React

No diretório do projeto React:

```bash
npm install
npm run build
```

Copie a pasta `build/` para o mesmo diretório onde está o `app.py`.

Estrutura final:

```
/meu-projeto/
├── app.py
├── requirements.txt
└── build/
    ├── index.html
    └── static/
```

### 3. Inicie o servidor Flask

```bash
python app.py
```

Acesse em: [http://localhost:5000](http://localhost:5000)

---

## ☁️ Como Hospedar Gratuitamente

### PythonAnywhere (modo fácil)

1. Acesse [https://www.pythonanywhere.com/](https://www.pythonanywhere.com/)
2. Crie uma conta gratuita
3. Crie uma nova **Web App**
4. Configure para usar `Flask` e aponte para seu `app.py`
5. Faça upload da pasta `build/` também
6. Reinicie a aplicação

### Render (mais robusto)

1. Crie conta em [https://render.com/](https://render.com/)
2. Crie um novo **Web Service**
3. Suba seu projeto via GitHub
4. Configure o build com:

```
Build Command: pip install -r requirements.txt
Start Command: python app.py
```

5. Defina o caminho para `build/` como estático se necessário
