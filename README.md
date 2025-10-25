# 🧠 Azure Credit Card Image Validation

Este projeto realiza a **validação de imagens de cartões de crédito** utilizando o serviço **Azure Document Intelligence** (antigo Form Recognizer). Ele extrai e analisa informações de documentos enviados via blob storage, com foco em segurança e automação.

## 🚀 Funcionalidades

- Upload de imagens de cartões via Azure Blob Storage  
- Extração de dados com Azure Document Intelligence  
- Validação de campos como número, nome e data de validade  
- Interface interativa com Streamlit

## 🛠️ Tecnologias

- Python 3.11  
- Azure Document Intelligence  
- Azure Blob Storage  
- Streamlit  
- dotenv

## 📦 Instalação

### 1. Clone o repositório

```bash
git clone https://github.com/seu-usuario/azure-card-validation.git
cd azure-card-validation
pip install -r requirements.txt
```

### 2. Crie um arquivo `.env` com as seguintes variáveis:

```env
ENDPOINT=https://<seu-recurso>.cognitiveservices.azure.com
SUBSCRIPTION_KEY=<sua-chave>
AZURE_STORAGE_CONNECTION_STRING=<sua-string-de-conexão>
CONTAINER_NAME=<nome-do-container>
```

## ▶️ Execução

```bash
streamlit run src/app.py
```

## 🧪 Testes

Você pode incluir testes unitários com `pytest` ou `unittest` para validar os serviços.

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 🙋‍♂️ Autor

Desenvolvido por **Elias** — Piracicaba, SP 🇧🇷  
Conecte-se no [LinkedIn](https://www.linkedin.com) ou contribua com sugestões!
