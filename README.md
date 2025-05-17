# Guia de Instalação Python para Ubuntu (com `uv`)

Olá a todos!

Estava com alguns conflitos na instalação do Python na minha máquina Linux Ubuntu. Felizmente, um amigo, **Matheus Gabriel** (vulgo `@su3h7am` do Discord), me ajudou a entender o uso de diretórios corretos para facilitar o processo. Fica aqui meu agradecimento também ao camarada **@cfranco3133**!
    
Lembrando o projeto alura não da suporte a usuários de Linux, e pode ocorrer coisas após a tentativa de instalar os pacotes do python3, onde sugere muitas vezes códigos que poderiam botar em risco minha máquina como `pip install "pacote" --break-system-packages`.

---


É importante ressaltar que o projeto Alura não oferece suporte oficial a usuários de Linux, e você pode encontrar situações após tentar instalar pacotes Python 3 que sugerem comandos arriscados, como `pip install "pacote" --break-system-packages`.

**ATENÇÃO:** O uso de `--break-system-packages` pode comprometer a estabilidade do seu sistema operacional!

Conforme a imagem abaixo destaca:

![Captura de tela de 2025-05-16 10-06-08.png](Captura%20de%20tela%20de%2025-05-16%2010-06-08.png)

**NÃO FAÇA ISSO, A MENOS QUE VOCÊ SAIBA EXATAMENTE O QUE ESTÁ FAZENDO E ESTEJA DISPOSTO A ARRISCAR QUEBRAR SEU SISTEMA OPERACIONAL.**

A melhor prática é sempre utilizar **ambientes virtuais** para seus projetos Python, isolando as dependências e evitando conflitos com os pacotes do sistema.

---

## Solução com `uv`

Para uma abordagem mais segura e eficiente, especialmente em Linux, recomendo o uso do **`uv`**. Ele é uma **ferramenta** rápida e poderosa para gerenciamento de pacotes e ambientes virtuais Python, atuando como o **instrumento ideal** para manter suas configurações organizadas e livres de problemas.



Primeiro, você precisa **instalar o `uv`** em seu sistema, executando este comando no terminal:

## Esses comandos vão:

* **`uv init`**: **Inicializar** um novo projeto `uv` no diretório atual.
* **`uv venv`**: **Criar** um ambiente virtual isolado dentro do diretório do seu projeto (normalmente em uma pasta chamada `.venv`).
* **`source .venv/bin/activate`**: **Ativar** o ambiente virtual. A partir deste ponto, qualquer pacote que você instalar ou comando Python que executar estará dentro deste ambiente isolado, sem afetar o sistema global.
* **`uv add google-genai`**: **Instalar** o pacote `google-genai` no seu ambiente virtual ativo.
* **`uv add dotenv`**: **Instalar** o pacote `dotenv` no seu ambiente virtual ativo.
* **`uv sync`**: **Sincronizar** as dependências do projeto, garantindo que tudo esteja conforme o planejado.

##LINK DE INSTALAÇÃO

```bash
curl -LsSf [https://astral.sh/uv/install.sh](https://astral.sh/uv/install.sh) | sh


