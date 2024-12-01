# Análise de cartão de crédito

Com do python em conjunto aos serviços do Azure Document Intelligence e Azure Blob Storage, foi criado um exemplo de aplicação que recebe o upload de uma arquivo, faz uma análise e retorna se é um cartão de crédito válido ou não.

![image](https://github.com/user-attachments/assets/708f88b6-0265-4d76-9db1-de9e924b97cd)


## Funcionalidades da Aplicação
* Upload de arquivo de imagem.
* Armazenamento em blob storage.
* Análise de imagem com base em modelo.
* Retorno de resultado ao usuário.

## Como usar
* Provisionar um `Storage Account` em uma subscription do Azure.
* Provisionar um `Document Intelligence` em uma subscription do Azure.
* Executar o comando abaixo para instalação das bibliotecas necessárias:
  ```bash
      pip install -r requirements.txt
  ```
* No arquivo `.env` preencha as informações de seu ambiente.
* Execute o comando abaixo para executar o aplicativo:
  ```bash
      streamlit run .\app.py
  ```
* Acessar a URL `http://localhost:8501/`.


## Estrutura do projeto
```tree
.
├── app.py
├── README.MD
├── src
   └── analise_cartao.py
   └── storage.py
├── .env
├── requirements.txt
```
