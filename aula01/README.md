# Aula 01 - LLM APIs

Esta pasta contém a primeira versão do projeto da monitoria: uma aplicação Python que envia uma requisição para uma LLM e observa a resposta.

## Preparação do ambiente

Abra um terminal nesta pasta e crie um ambiente virtual:

```bash
python -m venv .venv
```

Ative o ambiente virtual de acordo com o seu sistema operacional.

No Windows PowerShell:

```powershell
.\.venv\Scripts\Activate.ps1
```

No Prompt de Comando do Windows:

```bat
.venv\Scripts\activate.bat
```

No macOS ou Linux:

```bash
source .venv/bin/activate
```

Com o ambiente ativo, instale as dependências:

```bash
python -m pip install -r requirements.txt
```

## Configuração da API da Groq

1. Acesse o [GroqCloud Console](https://console.groq.com/) e crie uma conta ou faça login.
2. Abra a página [API Keys](https://console.groq.com/keys), selecione **Create API Key** e copie a chave gerada.
3. Crie o arquivo `.env` a partir do exemplo fornecido.

No Windows PowerShell ou no Prompt de Comando:

```powershell
copy env.example .env
```

No macOS ou Linux:

```bash
cp env.example .env
```

4. Abra o arquivo `.env` e substitua o valor de `GROQ_API_KEY` pela sua chave:

```dotenv
GROQ_API_KEY=sua_chave_da_groq_aqui
```

Mantenha as demais variáveis do arquivo como estão. O `.gitignore` já impede o versionamento do `.env`; nunca compartilhe nem faça commit da sua chave.

## Execução

Abra `aula1_llm_apis_template.ipynb` no VS Code ou no Jupyter e execute as células em ordem.

## Arquivos

- `Aula 1 - LLM APIs.pptx`: apresentação da aula;
- `aula1_llm_apis_template.ipynb`: notebook da aula;
- `env.example`: variáveis de ambiente esperadas;
- `requirements.txt`: dependências Python;
- `README.md`: este documento de configuração do ambiente.
