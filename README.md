
Estava tendo conflito para instalar python na minha máquina que é um linux Ubuntu, graças a um amigo Matheus Gabriel vulgo
@su3h7am do discord me ensinou usar os diretórios corretos para facilitar. Fica aqui meu agradecimento a ele e ao camarada @cfranco3133.

Lembrando o projeto alura não da suporte a usuários de Linux, e pode ocorrer coisas após a tentativa de instalar os pacotes do python3, onde sugere muitas vezes códigos que poderiam botar em risco minha máquina como "pip install "pacote" --break-system-packages".


uv init
uv venv
source .venv/bin/activate
uv add google-genai
uv add dotenv
uv sync