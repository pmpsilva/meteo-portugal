# 🌦️ Meteo Portugal

**Versão 26.1** 
[Road Map](https://trello.com/b/hKr4ImJM/meteo-portugal-tempo-e-mar-roadmap)

 Meteo Portugal desenvolvido por pmpsilva powered by IPMA e Open-Meteo.

Aplicação Android de meteorologia para Portugal, utilizando dados abertos do [IPMA](https://www.ipma.pt/) (Instituto Português do Mar e da Atmosfera) e do [Open-Meteo](https://open-meteo.com/).

## ✨ Funcionalidades

- **Condições atuais** — Temperatura, humidade, vento, pressão e precipitação a partir da estação meteorológica mais próxima
- **Ciclo Solar** — Horas precisas de nascer e pôr do sol
- **Previsão horária** — Detalhe hora a hora para as próximas 72 horas (temperatura, chuva, vento)
- **Previsão a 10 dias** — Temperaturas mínimas e máximas, tipo de tempo, probabilidade de precipitação e intensidade do vento
- **Avisos meteorológicos** — Alertas amarelo, laranja e vermelho do IPMA, filtrados por área
- **Índice UV** — Nível de radiação ultravioleta com descrição do risco
- **Seleção de localidade** — Todas as cidades e distritos de Portugal continental, Madeira e Açores
- **Favoritos** — Guarde as suas cidades preferidas com acesso e seleção rápida a partir do ecrã inicial
- **Deteção automática por GPS** — Na primeira utilização, seleciona a cidade mais próxima com base na localização GPS
- **Cache offline (Room)** — Os dados meteorológicos são guardados localmente para acesso instantâneo e sem internet
- **Definições** — Intervalo de poupança de dados configurável (5 min a 24h, visibilidade de secções)
- **Interface adaptável** — Fundo dinâmico que se adapta às condições meteorológicas e à hora do dia

## 🌐 API do IPMA

A aplicação consome os seguintes endpoints da [API aberta do IPMA](https://api.ipma.pt/):

| Endpoint | Descrição |
| --- | --- |
| `/public-data/forecast/aggregate/{id}.json` | Previsão agregada (horária 72h + diária 10 dias) |
| `/open-data/forecast/meteorology/cities/daily/{id}.json` | Previsão diária por localidade (legado) |
| `/open-data/forecast/meteorology/cities/daily/hp-daily-forecast-day0.json` | Previsão do dia atual (todas as cidades) |
| `/open-data/observation/meteorology/stations/obs-surface.geojson` | Observações das estações meteorológicas |
| `/open-data/forecast/warnings/warnings_www.json` | Avisos meteorológicos |
| `/open-data/forecast/meteorology/uv/uv.json` | Previsão do índice UV |
| `/public-data/forecast/locations.json` | Lista completa de localidades (todas as cidades) |
| `/open-data/weather-type-classe.json` | Tipos de tempo (descrições) |
| `/open-data/wind-speed-daily-classe.json` | Classes de velocidade do vento |
| `/open-data/precipitation-classe.json` | Classes de precipitação |

## 📄 Licença

Este projeto utiliza dados abertos do IPMA, disponíveis sob os [termos de utilização do IPMA](https://www.ipma.pt/pt/siteinfo/index.html).

---

## ☕ Apoiar o Projeto

Se gosta da app, considere pagar-me um café!

[![Buy me a coffee](https://img.shields.io/badge/Buy%20me%20a%20coffee-PayPal-blue?style=for-the-badge&logo=paypal)](https://paypal.me/PedroSilva971)


*Desenvolvido por pmpsilva com ☀️ em Portugal — powered by IPMA & Open-Meteo*
