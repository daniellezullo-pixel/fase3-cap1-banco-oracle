# fase3-cap1-banco-oracle

PBL Fase 3 Capítulo 1 – Banco de Dados Oracle FarmTech Solutions

---

## Descrição do projeto

Este repositório contém as consultas SQL realizadas no banco de dados Oracle referentes à atividade da Fase 3 do projeto FarmTech Solutions.

O objetivo desta atividade foi realizar consultas no banco de dados para análise das informações de irrigação, umidade e tipos de cultura agrícola, utilizando comandos SQL para extração, filtragem e organização dos dados.

---

## Objetivo da atividade

Desenvolver consultas SQL no Oracle Database com a finalidade de:

- Visualizar os dados importados na base;
- Filtrar informações relevantes;
- Identificar padrões relacionados ao nível de irrigação;
- Calcular estatísticas descritivas;
- Organizar dados agrícolas para análise.

---

## Estrutura do repositório

A pasta `imprimir/` contém as capturas de tela das consultas executadas no Oracle SQL Developer.

Arquivos presentes:

- `01-inicio.png` → visualização inicial da base de dados;
- `02-irrigacao-alta.png` → consulta filtrando irrigação alta;
- `03-media-umidade.png` → cálculo da média de umidade;
- `04-total-registros.png` → contagem total de registros;
- `05-tipos-cultura.png` → listagem de culturas distintas.

---

## Consultas realizadas

### 1. Consulta inicial da base

**Objetivo:** visualizar todos os registros importados no banco.

**Consulta SQL utilizada:**

```sql
SELECT * 
FROM DADOS_IRRIGACAO;
```

**Resultado obtido:**  
Foi possível visualizar todos os registros presentes na tabela `DADOS_IRRIGACAO`, permitindo a validação dos dados inseridos e a compreensão da estrutura da base.

---

### 2. Consulta de irrigação alta

**Objetivo:** identificar culturas com nível de irrigação alto.

**Consulta SQL utilizada:**

```sql
SELECT *
FROM DADOS_IRRIGACAO
WHERE NIVEL_IRRIGACAO = 'Alto';
```

**Resultado obtido:**  
A consulta retornou apenas os registros classificados com nível de irrigação alto, permitindo identificar culturas que demandam maior quantidade de água.

---

### 3. Média de umidade

**Objetivo:** calcular a média da umidade registrada.

**Consulta SQL utilizada:**

```sql
SELECT AVG(UMIDADE) AS MEDIA_UMIDADE
FROM DADOS_IRRIGACAO;
```

**Resultado obtido:**  
Foi calculada a média geral da umidade registrada no banco, auxiliando na análise das condições climáticas associadas às culturas.

---

### 4. Total de registros

**Objetivo:** verificar a quantidade total de dados importados.

**Consulta SQL utilizada:**

```sql
SELECT COUNT(*) AS TOTAL_REGISTROS
FROM DADOS_IRRIGACAO;
```

**Resultado obtido:**  
A consulta retornou a quantidade total de registros armazenados na tabela, permitindo validar se a importação dos dados ocorreu corretamente.

---

### 5. Tipos de cultura distintos

**Objetivo:** listar os tipos de cultura sem repetição.

**Consulta SQL utilizada:**

```sql
SELECT DISTINCT TIPO_CULTURA
FROM DADOS_IRRIGACAO;
```

**Resultado obtido:**  
Foi possível identificar os diferentes tipos de culturas presentes na base de dados sem duplicidade de registros.

---

## Tecnologias utilizadas

- Oracle SQL Developer  
- Oracle Database  
- SQL  
- GitHub

---

## Vídeo de apresentação

Link do vídeo:  
[(https://youtu.be/F4QzTNTXk4Q)](https://youtu.be/F4QzTNTXk4Q)

---

## Autora

**Danielle Zullo**  
**RM: 571880**
