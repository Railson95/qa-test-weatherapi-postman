# 🌦️ Testes Automatizados com Postman - Weather API

- Mini-projeto de automação de testes utilizando o Postman com a API pública da OpenWeather.
- Validação de parâmetros, autenticação, segurança (XSS e redirecionamento), estrutura de dados e mensagens de erro.
- Baseado na heurística POISED e técnicas como Partição de Equivalência e Análise de Valor Limite.
- A Api está disponível em: https://www.weatherapi.com/

---

## ⚙️ Tecnologias utilizadas

- **Postman** na versão `v11.0.7`
- **Git** na versão `2.48.1.windows.1`
- **VScode** na versão `1.101.2`
- **Weather API** na versão `1.0.2`

---

## 📚 Documentações

- [Documentação Postman](https://learning.postman.com/docs/introduction/overview/)
- [Documentação Weather API](https://app.swaggerhub.com/apis-docs/WeatherAPI.com/WeatherAPI/1.0.2#/)

---

## ⚙️ Como configurar o ambiente

Abra um terminal e siga os passos abaixo:

🔽 1. Clonar o repositório e acessar a pasta:

```bash
git clone https://github.com/Railson95/qa-test-weatherapi-postman.git
cd a-test-weatherapi-postman
```

🧰 2. Baixar e instalar o Postman (Windows):

```bash
https://dl.pstmn.io/download/version/11.0.7/win64
```

🔑 3. Criar uma conta na Weather API para obter a API Key:

```bash
https://www.weatherapi.com/signup.aspx
```

Acesse o painel ("Dashboard") após o login e copie sua API Key.
Salve em um local seguro, pois será usada nos testes.

📤 4. Importar os arquivos .postman_collection.json e .postman_environment.json no Postman.

🌍 5. No Postman, selecione o Environment e cole a API Key na variável validApiKey.

▶️ Como executar os testes

- Abra o Runner no Postman.
- Arraste a Collection desejada para o Runner.
- Em "Data", selecione o arquivo .csv correspondente à Collection.

```bash
Collection: Auth         → Arquivo: auth_data2.csv
Collection: Endpoints    → Arquivo: weather_data.csv
Collection: Security     → Não requer arquivo .csv
```

![Selecionar arquivo CSV](https://raw.githubusercontent.com/Railson95/qa-test-weatherapi-postman/master/assets/select_file.png)

# Imagem do teste realizado para o Endpoint Clima Atual

Parâmetros testados: Latitude e Longitude

![Teste do Endpoint Clima Atual](https://raw.githubusercontent.com/Railson95/qa-test-weatherapi-postman/master/assets/endpoints.png)

# Imagens mostrando o uso dos Packages e a remoção de Código Duplicado

## Chamando as funções criadas no Packeges da aba Script

### Requisição 1

![Package1](https://raw.githubusercontent.com/Railson95/qa-test-weatherapi-postman/master/assets/packages1.png)

### Requisição 2

![Package2](https://raw.githubusercontent.com/Railson95/qa-test-weatherapi-postman/master/assets/packages2.png)

## Package criado com nome de utils

![Package3](https://raw.githubusercontent.com/Railson95/qa-test-weatherapi-postman/master/assets/packages3.png)

✍️ Autor
Railson Martins da Mata
Este projeto tem fins educacionais e foi desenvolvido com foco em práticas de automação de testes para APIs, aplicando a heurística
POISED como guia de cobertura e análise.
