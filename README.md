# fase3-cap1-banco-oracle

PBL Fase 3 Capítulo 1 - Banco de Dados Oracle FarmTech Solutions

## Descrição
Este repositório contém os prints das consultas SQL realizadas no banco de dados Oracle da atividade da Fase 3.

## Estrutura dos arquivos

Pasta: imprimir/

- 01-inicio.png
- 02-irrigacao-alta.png
- 03-media-umidade.png
- 04-total-registros.png
- 05-tipos-cultura.png

Consultas realizadas

1. Consulta inicial da base
SELECT * FROM DADOS_IRRIGACAO;

Objetivo: visualizar todos os registros importados no banco.

2. Consulta de irrigação alta
SELECT *
FROM DADOS_IRRIGACAO
WHERE NIVEL_IRRIGACAO = 'Alto';

Objetivo: identificar culturas com irrigação alta.

3. Média de umidade
SELECT AVG(UMIDADE) AS MEDIA_UMIDADE
FROM DADOS_IRRIGACAO;

Objetivo: calcular a média da umidade registrada.

4. Total de registros
SELECT COUNT(*) AS TOTAL_REGISTROS
FROM DADOS_IRRIGACAO;

Objetivo: verificar a quantidade total de dados importados.

5. Tipos de cultura distintos
SELECT DISTINCT TIPO_CULTURA
FROM DADOS_IRRIGACAO;

Objetivo: listar os tipos de cultura sem repetição.

## Tecnologias utilizadas
- Oracle SQL Developer
- SQL
- GitHub
## Vídeo de apresentação

Link do vídeo: https://youtu.be/F4QzTNTXk4Q
