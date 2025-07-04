# Testes Automatizados com Postman - Weather API

- Mini-projeto de testes automatizados com Postman usando a API pública da OpenWeather.
- Validação de parâmetros, autenticação, segurança (XSS, redirecionamento), estrutura de dados e mensagens de erro.
- Baseado na heurística POISED e técnicas como Partição de Equivalência e Análise de Valor Limite.
- Disponível em: https://www.weatherapi.com/

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

## 🧰 Como instalar o ambiente

Abrir algum terminal e digitar:

🔁 1. Fazer o clone do repositório e redirecionar para a pasta

```bash
git clone https://github.com/Railson95/qa-test-weatherapi-postman.git
cd a-test-weatherapi-postman
```

✅ 2. Fazer download e instalar o Postman pelo seguinte link, caso esteja no Windows

```bash
https://dl.pstmn.io/download/version/11.0.7/win64
```

🛠️ 3. Fazer uma conta na Weather APi

```bash
https://www.weatherapi.com/signup.aspx
```

Precisamos dessa conta para gerar a APIKey e assim estarmos autenticados para enviarmos requsições para a API
Após feito a conta, entrar e pegar a APIKey, ela fica em Dashboard/API
Guarde ela em um arquivo de texto auxiliar, iremos precisar futuramente

📦 4. Importe as Collections e o Enviroment baixados do Git no Postman

📁 5. No Postman clique em Enviroment e na variável de ambiente validApiKey, cole a APIKey que coletamos da sua conta da Weather API

▶️ Como rodar os testes

- Clique no Runner do Postman
- Arraste e solte a Collection que você quer testar
- Selecione em data driven o arquivo csv que contém os Casos de Teste

```bash
Para a Collection Auth usar o arquivo: auth_data2
Para a Collection Endpoints usar o arquivo: weather_data
Não foi necessário a criação de arquivo csv para a Collection Security
```

https://github.com/Railson95/qa-test-weatherapi-postman/blob/master/assets/select_file.png

✍️ Autor
Railson Martins da Mata
Projeto educacional com fins de prática em automação de testes de API com Postman, explorando a heurística POISED.
