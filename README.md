# Análise Climática Mensal - São Paulo 

Este projeto realiza a coleta, análise e visualização de dados climáticos para a cidade de São Paulo usando Python. Ele utiliza dados históricos de temperatura e precipitação do serviço **Open-Meteo**.

## Arquivos do Projeto

| Arquivo               | Descrição                     | Link |
|-----------------------|-------------------------------|------|
| app.ipynb             | Notebook da análise           | [Abrir app.ipynb](./app.ipynb) |
| dados_clima.csv       | Dataset utilizado na análise  | [Abrir dados_clima.csv](./dados_clima.csv) |



## Apresentação

Uma visão geral da análise de dados meteorológicos está disponível neste slide interativo:  
[Visualizar Slides no Gamma](https://gamma.app/docs/Analise-de-Dados-Meteorologicos-Visao-Geral-lralfeselp78y0b)


---

## Funcionalidades

1. **Coleta de dados**  
   - Obtém dados diários de temperatura máxima, mínima e precipitação total via API pública em formato CSV.
   - Período analisado: novembro de 2025.
  
---

3. **Processamento de dados**  
   - Lê o CSV e limpa a tabela, garantindo que os dados estejam prontos para análise.
   - Verifica se existem valores nulos.
   - Calcula estatísticas descritivas para:
     - Temperatura Máxima (°C)
     - Temperatura Mínima (°C)
     - Precipitação Total (mm)
    
---

3. **Visualização de dados**  
   - Cria um gráfico interativo usando **Plotly** com dois eixos Y:
     - Eixo Y primário: Temperaturas máxima e mínima
     - Eixo Y secundário: Precipitação total
   - Destaques:
     - Linha vermelha para temperatura máxima
     - Linha azul para temperatura mínima
     - Linha verde pontilhada para precipitação

---

4. **Análise de extremos**  
   - Identifica:
     - Dia com a maior temperatura
     - Dia com a menor temperatura
     - Dia com a maior precipitação
   - Exibe informações detalhadas de cada dia extremo (data, temperatura e precipitação).
  
   <img width="924" height="324" alt="image" src="https://github.com/user-attachments/assets/357c54f5-a627-41de-a3d2-0cd61e88f24d" />


---

**Visualização de Dados**: Um gráfico de linha foi gerado, mostrando efetivamente a evolução diária da temperatura máxima, temperatura mínima e precipitação total, permitindo compreender visualmente tendências e eventos extremos.

<img width="620" height="329" alt="image" src="https://github.com/user-attachments/assets/277d4e91-6bcc-460e-b382-4d9c057fe92d" />

---

6. **Exportação**  
   - Salva o DataFrame final em CSV: `dados_clima.csv`.

---

## Tecnologias Utilizadas

- Python 3.x
- Pandas
- Plotly
- API Open-Meteo (CSV)

---

## Como Executar

1. Clone este repositório.
2. Instale as dependências:

```bash
pip install pandas plotly





