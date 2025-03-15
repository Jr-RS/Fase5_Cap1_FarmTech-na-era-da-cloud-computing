# FIAP - Faculdade de Informática e Administração Paulista

<p align="center">
<a href= "https://www.fiap.com.br/"><img src="assets/logo-fiap.png" alt="FIAP - Faculdade de Informática e Admnistração Paulista" border="0" width=40% height=40%></a>
</p>

---

# 🌾 Projeto de Previsão de Rendimento de Safra - FarmTech Solutions

## Nome do projeto
Fase 4 - Cap 1 - Automação e Inteligência na FarmTech Solutions

## Nome do grupo
Grupo 44

## 👨‍🎓 Integrantes:
- [Ana Beatriz Duarte Domingues](https://www.linkedin.com/in/)
- [Junior Rodrigues da Silva](https://www.linkedin.com/in/jrsilva051/)
- [Carlos Emilio Castillo Estrada](https://www.linkedin.com/in/)

## 👩‍🏫 Professores:
### Tutor(a)
- [Lucas Gomes Moreira](https://www.linkedin.com/company/inova-fusca)
### Coordenador(a)
- [André Godoi Chiovato](https://www.linkedin.com/company/inova-fusca)

---

## 📝 Descrição
Este projeto foi desenvolvido como parte do curso da FIAP e tem como objetivo analisar dados de uma fazenda de médio porte para prever o rendimento de safra. Para isso, utilizamos técnicas de análise exploratória de dados (EDA), clusterização para identificação de padrões e anomalias, e modelos de regressão supervisionada para previsão de rendimento.

Os dados utilizados incluem informações sobre a cultura plantada, precipitação, umidade, temperatura e rendimento da safra em toneladas por hectare.

---

## 📚 Estrutura de Pastas

```
/
|-- assets/                                 # Imagens, logotipos e anexos
|   |-- Estimativa - SA (São Paulo).pdf     # Arquivo pdf com as estimativas de preços na AWS
|   |-- Estimativa - US (N. Virginia).pdf   # Arquivo pdf com as estimativas de preços na AWS
|   |-- logo-fiap.png                       # Logo da FIAP exibido no readme
|-- data/                                   # Base de dados utilizada no projeto
|   |-- crop_yield.csv                      # Arquivo com os dados das safras
|-- NomeCompleto_RM_pbl_fase4.ipynb         # Notebook principal do projeto
|-- README.md                               # Documentação do projeto
```

---

### 🚀 Passo a Passo
Abra o notebook no Jupyter ou Google Colab e execute as células de código na sequência.

---

## 📊 Comparação de Custos AWS

Foram realizadas duas estimativas de custos utilizando a AWS Pricing Calculator:

| Serviço | São Paulo (SA) | Virgínia do Norte (US) | Diferença |
|---------|---------------|------------------------|------------|
| **EC2 (t4g.micro)** | **US$ 7,83/mês** | **US$ 4,91/mês** | **+59,6% mais caro em SP** |
| **AWS Lambda (1000 requests)** | **US$ 0,00/mês** | **US$ 0,00/mês** | **Sem custo** |
| **S3 (50GB)** | **US$ 2,02/mês** | **US$ 1,15/mês** | **+75,7% mais caro em SP** |
| **Total Mensal** | **US$ 9,85/mês** | **US$ 6,06/mês** | **+62,5% mais caro em SP** |
| **Total Anual** | **US$ 118,20** | **US$ 72,72** | **US$ 45,48 de diferença** |

---

## 📜 Considerações sobre a LGPD e Armazenamento no Exterior

A **Lei Geral de Proteção de Dados (LGPD - Lei nº 13.709/2018)** impõe restrições ao armazenamento e processamento de dados fora do Brasil:

- **Transferência Internacional de Dados** (Art. 33 da LGPD) requer que:
  - O país de destino tenha proteção de dados equivalente ao Brasil.
  - Exista contrato garantindo conformidade com a LGPD.
  - O titular dos dados tenha dado consentimento específico.

### 🏆 Escolha da Melhor Opção para o Projeto

Embora a hospedagem nos EUA seja mais barata, devido às exigências da **LGPD** e à necessidade de acesso rápido aos clientes brasileiros, a **recomendação é hospedar os serviços na AWS São Paulo (sa-east-1)**.

**Justificativa:**

✔ **Conformidade Legal** – Evita riscos de penalização por descumprimento da LGPD.  
✔ **Latência Menor** – Hospedagem no Brasil reduz o tempo de resposta dos serviços.  
✔ **Maior Controle dos Dados** – A AWS no Brasil garante que os dados permaneçam dentro da jurisdição nacional.

💡 **Decisão Final:** Apesar do custo mais alto, a escolha pela **AWS São Paulo (sa-east-1)** é recomendada para evitar riscos regulatórios e melhorar a eficiência operacional.

---

### ⚙️ Implementação da Infraestrutura

- **Treinamento do Modelo:** Google Colab (evita custo de computação na AWS).
- **Empacotamento do Projeto:** Docker local.
- **Hospedagem da API:** AWS EC2 (São Paulo).
- **Inferências:** AWS Lambda (processamento sob demanda).
- **Armazenamento dos Dados:** AWS S3 (logs e resultados das inferências).

---

### 🎥 Vídeo Demonstrativo
O vídeo demonstrativo do projeto está disponível no YouTube:
[Assista aqui](#) *(Atualizar com o link do vídeo)*

---

## 📚 Histórico de Lançamentos

* 0.1.0 - 13/03/2025
    * Primeira versão do projeto com análise exploratória, clusterização e modelos de regressão.

---

## 📋 Licença

<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1"><p xmlns:cc="http://creativecommons.org/ns#" xmlns:dct="http://purl.org/dc/terms/"><a property="dct:title" rel="cc:attributionURL" href="https://github.com/agodoi/template">MODELO GIT FIAP</a> por <a rel="cc:attributionURL dct:creator" property="cc:attributionName" href="https://fiap.com.br">Fiap</a> está licenciado sobre <a href="http://creativecommons.org/licenses/by/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">Attribution 4.0 International</a>.</p>