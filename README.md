
# 🧠 Azure Credit Card Image Validation

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)
![Streamlit](https://img.shields.io/badge/Streamlit-app-red?logo=streamlit)
![Azure](https://img.shields.io/badge/Azure-Document_Intelligence-blue?logo=microsoftazure)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Em%20desenvolvimento-yellow)

Este projeto realiza a **validação de imagens de cartões de crédito** utilizando o serviço **Azure Document Intelligence** (antigo Form Recognizer). Ele extrai e analisa informações de documentos enviados via Azure Blob Storage, com foco em segurança e automação.

---

## 🚀 Funcionalidades

- Upload de imagens de cartões via Azure Blob Storage  
- Extração de dados com Azure Document Intelligence  
- Validação de campos como número, nome e data de validade  
- Interface interativa com Streamlit  
- Proteção contra fraudes com verificação automatizada

---

## 🛠️ Tecnologias

- Python 3.11  
- Azure Document Intelligence  
- Azure Blob Storage  
- Streamlit  
- dotenv

---

## 📦 Instalação

### 1. Clone o repositório

```bash
git clone https://github.com/EliasPira/new-azure-card-validation.git
cd new-azure-card-validation
pip install -r requirements.txt
```

> 💡 Se preferir usar SSH:
> `git clone git@github.com:EliasPira/new-azure-card-validation.git`

### 2. Configure suas variáveis de ambiente

Crie um arquivo `.env` na raiz do projeto com os seguintes campos:

```env
ENDPOINT=https://<seu-recurso>.cognitiveservices.azure.com
SUBSCRIPTION_KEY=<sua-chave-do-form-recognizer>
AZURE_STORAGE_CONNECTION_STRING=<sua-string-de-conexão>
CONTAINER_NAME=<nome-do-container>
```

> 🔐 **Importante:** nunca versionar o arquivo `.env`. Ele já está incluído no `.gitignore`.

---

## ▶️ Execução

```bash
streamlit run src/app.py
```

---

## 🧪 Testes

Você pode incluir testes unitários com `pytest` ou `unittest` para validar os serviços. Exemplo:

```bash
pytest tests/
```

---

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

## 🙋‍♂️ Autor

Desenvolvido por **Elias** — Piracicaba, SP 🇧🇷  
Conecte-se no [LinkedIn](https://www.linkedin.com) ou contribua com sugestões!

---

## 🤝 Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests.

1. Fork este repositório  
2. Crie sua branch: `git checkout -b minha-feature`  
3. Commit suas alterações: `git commit -m 'Minha nova feature'`  
4. Push para a branch: `git push origin minha-feature`  
5. Abra um Pull Request

---

## 📌 Roadmap (em breve)

- [ ] Validação de bandeiras de cartão  
- [ ] Integração com OCR alternativo  
- [ ] Dashboard de estatísticas de validação  