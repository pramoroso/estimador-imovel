
# 🏘️ Estimador de Imóveis

Este é um app web interativo que permite estimar o valor de imóveis com base em dados de área construída, terreno e vagas de garagem. Desenvolvido por **Paulo Amoroso**, o app também consulta uma API pública e exibe uma tabela com valores reais de imóveis por localidade.

## 🔍 Funcionalidades

- Busca de imóveis por:
  - Tipo: apartamento ou casa
  - Estado, cidade e bairro
- Tabela com:
  - Área construída
  - Área do terreno
  - Número de vagas
  - Valor do imóvel
- Simulador de estimativa baseado em média ponderada dos dados reais:
  - R$ por m² de construção
  - R$ por m² de terreno (para casas)
  - Fator de ajuste por vagas de garagem

## 🧠 Como funciona

O app consulta dados de imóveis via API externa (`api-estimador-imoveis`) e utiliza os valores para estimar, de forma aproximada, quanto valeria um novo imóvel com base nos parâmetros inseridos.

### Fórmula de estimativa:

**Para apartamentos:**
```
valor_estimado = área_construída × preço_m2 × (1 + 0.05 × vagas)
```

**Para casas:**
```
valor_estimado = (área_construída × preço_m2) + (área_terreno × preço_terreno_m2) × (1 + 0.05 × vagas)
```

## 🛠️ Tecnologias

- HTML5
- TailwindCSS
- JavaScript moderno
- API externa hospedada via Render

## 📂 Acesse

- 🔗 Projeto online: [https://pramoroso.github.io/estimador-imovel/](https://pramoroso.github.io/estimador-imovel/)
- 📁 Código-fonte: [https://github.com/pramoroso/estimador-imovel](https://github.com/pramoroso/estimador-imovel)

## 👨‍💼 Autor

**Paulo Amoroso**  
Engenheiro Eletricista | Gerente de Projetos | Dev Entusiasta  
🔗 [LinkedIn](https://www.linkedin.com/in/paulo-amoroso-04782a29/)

---

> Esta ferramenta é um estimador aproximado. Não substitui avaliação técnica ou corretor de imóveis. Use como referência inicial.
