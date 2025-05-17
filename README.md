
# MiauzãoAI - Consultor de Economia Energética  

![GitHub](https://img.shields.io/badge/status-em%20desenvolvimento-yellowgreen)  
![Python](https://img.shields.io/badge/Python-3.x-blue)  
![License](https://img.shields.io/badge/license-MIT-green)

## 📌 Visão Geral  

O MiauzãoAI é um chatbot assistente que utiliza inteligência artificial (Google Gemini) para auxiliar usuários a gerenciar e reduzir o consumo de energia elétrica em suas residências. Com uma personalidade única e cheia de gírias, o bot faz análises personalizadas baseadas nos dados fornecidos pelo usuário.

## ✨ Funcionalidades Principais  

- 🏠 Análise de consumo energético residencial  
- 💡 Cálculo de custos por dispositivo eletrônico  
- 📊 Comparativo de faturas de energia  
- 🔍 Identificação de "vilões" de consumo  
- 💰 Dicas personalizadas para economia  
- 🌡️ Recomendações para otimização de aparelhos como ar-condicionado  
- ⏱️ Análise de tarifas por horário  

## 🛠️ Tecnologias Utilizadas  

- Python 3.x  
- Google Generative AI SDK (Gemini)  
- dotenv (para gerenciamento de variáveis de ambiente)  

## 🚀 Como Usar  

### Pré-requisitos  

- Conta no Google AI Studio  
- API Key do Gemini  
- Python 3.x instalado  

## 💬 Exemplo de Interação

### Veja como você pode interagir com o MiauzãoAI:

```Plaintext

Usuário: Minha conta de luz subiu muito este mês
MiauzãoAI: E aí, meu consagrado! Bora desvendar esse mistério da conta lá nas alturas... 
Primeiro, me passa aí: 
1. Qual foi o gasto em kWh nos últimos 3 meses? 
2. O valor atual do kWh que tá na sua conta!
3. Tem algum aparelho novo aí na casa?

```

---
## Configure sua API Key:
Crie um arquivo .env na raiz do projeto com:
`GOOGLE_API_KEY=` [sua_chave_aqui](https://aistudio.google.com/app/apikey)


## 📊 Estrutura do Projeto
### A organização do projeto segue a seguinte estrutura:

```bash
python main.py


miauzao-ai/
├── main.py            # Código principal do chatbot
├── README.md          # Este arquivo de documentação
├── requirements.txt   # Lista de dependências Python do projeto
└── .env               # Arquivo de configurações de ambiente (ignorada pelo Git)


```
# Guia de Instalação de pacotes Python para Ubuntu (com `uv`)

Olá a todos!

Estava com alguns conflitos na instalação do Python na minha máquina Linux Ubuntu. Felizmente, um amigo, **Matheus Gabriel** (vulgo `@su3h7am` do Discord), me ajudou a entender o uso de diretórios corretos para facilitar o processo. Fica aqui meu agradecimento também ao camarada **@cfranco3133**!
    
Lembrando o projeto alura não da suporte a usuários de Linux, e pode ocorrer coisas após a tentativa de instalar os pacotes do python3, onde sugere muitas vezes códigos que poderiam botar em risco minha máquina como `pip install "pacote" --break-system-packages`.


É importante ressaltar que o projeto Alura não oferece suporte oficial a usuários de Linux, e você pode encontrar situações após tentar instalar pacotes Python 3 que sugerem comandos arriscados, como `pip install "pacote" --break-system-packages`.

**ATENÇÃO:** O uso de `--break-system-packages` pode comprometer a estabilidade do seu sistema operacional!


**NÃO FAÇA ISSO, A MENOS QUE VOCÊ SAIBA EXATAMENTE O QUE ESTÁ FAZENDO E ESTEJA DISPOSTO A ARRISCAR QUEBRAR SEU SISTEMA OPERACIONAL.**

A melhor prática é sempre utilizar **ambientes virtuais** para seus projetos Python, isolando as dependências e evitando conflitos com os pacotes do sistema.

---

## Solução com `uv`

Para uma abordagem mais segura e eficiente, especialmente em Linux, recomendo o uso do **`uv`**. Ele é uma **ferramenta** rápida e poderosa para gerenciamento de pacotes e ambientes virtuais Python, atuando como o **instrumento ideal** para manter suas configurações organizadas e livres de problemas.



Primeiro, você precisa **instalar o `uv`** em seu sistema, executando este comando no terminal:

```bash
curl -LsSf [https://astral.sh/uv/install.sh](https://astral.sh/uv/install.sh) | sh
```

## Esses comandos vão:

* **`uv init`**: **Inicializar** um novo projeto `uv` no diretório atual.
* **`uv venv`**: **Criar** um ambiente virtual isolado dentro do diretório do seu projeto (normalmente em uma pasta chamada `.venv`).
* **`source .venv/bin/activate`**: **Ativar** o ambiente virtual. A partir deste ponto, qualquer pacote que você instalar ou comando Python que executar estará dentro deste ambiente isolado, sem afetar o sistema global.
* **`uv add google-genai`**: **Instalar** o pacote `google-genai` no seu ambiente virtual ativo.
* **`uv add dotenv`**: **Instalar** o pacote `dotenv` no seu ambiente virtual ativo.
* **`uv sync`**: **Sincronizar** as dependências do projeto, garantindo que tudo esteja conforme o planejado.


