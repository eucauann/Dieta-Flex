# Documentação da Calculadora de Dieta

## Visão Geral

A Calculadora de Dieta é uma aplicação web que ajuda os usuários a calcular suas necessidades nutricionais com base em diversos parâmetros, como sexo, idade, altura, peso e nível de atividade física. A aplicação permite que os usuários ajustem a ingestão de proteínas e gorduras através de controles deslizantes e fornece resultados detalhados sobre massa magra, massa gorda e calorias necessárias.

**Nota:** Este projeto é apenas uma ferramenta para embasar suas decisões alimentares. É altamente recomendável consultar um nutricionista para obter orientação profissional personalizada.

## Estrutura do Projeto

O projeto consiste em três arquivos principais:

1. **`index.html`**: O arquivo HTML que contém a estrutura da página e os elementos do formulário.
2. **`style.css`**: O arquivo CSS que estiliza a aplicação e define a aparência dos elementos.
3. **`script.js`**: O arquivo JavaScript que contém a lógica para calcular as necessidades nutricionais e manipular a interface do usuário.

## Fórmulas Utilizadas

As fórmulas para os cálculos realizados na Calculadora de Dieta incluem:

1. **Taxa Metabólica Basal (TMB)**: A TMB é calculada utilizando a fórmula de Cunningham, que considera a massa magra do corpo:
   \[
   TMB = 500 + (22 \times \text{Massa Magra em kg})
   \]

2. **Cálculo das calorias necessárias**:
   - **Calorias em repouso** (TMB)
   - **Calorias durante o treino** (multiplicador baseado na intensidade da atividade física)
   - **Calorias para ganho ou perda de peso** (ajuste baseado no objetivo do usuário)

3. **Ingestão de macronutrientes**:
   - **Proteínas**: Calculadas com base na proteína por kg de peso total (g).
   - **Gorduras**: Calculadas com base na gordura por kg de peso total (g).
   - **Carboidratos**: Calculados a partir das calorias restantes após a subtração das calorias de proteínas e gorduras.

## Instruções de Uso

1. **Abra o arquivo `index.html` em um navegador da web.**
2. **Preencha os campos do formulário**:
   - Selecione o sexo e o biotipo.
   - Insira a idade, altura, peso e percentual de gordura.
   - Insira a medida da cintura, quadril e braço.
   - Selecione o objetivo (perder, manter ou ganhar peso).
   - Selecione a intensidade da atividade física.
   - Ajuste as quantidades de proteína e gordura desejadas usando os controles deslizantes.
3. **Clique no botão "Calcular"** para obter os resultados nutricionais.

## Descrição dos Arquivos

### `index.html`

Este arquivo contém a estrutura HTML da página. Os principais elementos incluem:

- Um cabeçalho (`<h1>`) com o título da calculadora.
- Um formulário (`<form>`) que coleta as informações do usuário.
- Elementos de entrada (`<input>`, `<select>`, `<button>`) que permitem a interação do usuário.
- Uma seção de resultados (`<div id="resultado">`) que exibe os resultados após o cálculo.

### `style.css`

Este arquivo contém estilos para a aplicação, incluindo:

- Definição de fontes e cores para a página.
- Estilo para o contêiner da calculadora, incluindo margens, bordas e sombras.
- Estilo para os grupos de formulários e botões, garantindo uma aparência limpa e organizada.

### `script.js`

Este arquivo contém a lógica para o cálculo das necessidades nutricionais e manipulação do DOM. As principais funções incluem:

- **Coleta de dados**: Captura os valores inseridos pelo usuário no formulário.
- **Cálculo**: Realiza os cálculos necessários para determinar a massa magra, massa gorda, taxa metabólica basal (TMB) e as calorias necessárias para o objetivo selecionado.
- **Exibição de resultados**: Atualiza a seção de resultados com os dados calculados, permitindo que o usuário visualize suas necessidades nutricionais.

## Considerações Finais

A Calculadora de Dieta é uma ferramenta útil para quem deseja monitorar sua dieta e ajustar suas necessidades nutricionais de acordo com seus objetivos de saúde. Para melhorias futuras, considere adicionar funcionalidades como gráficos de progresso, recomendações personalizadas e armazenamento de dados do usuário.

**Nota:** Este projeto é uma referência inicial e não deve substituir a consulta a um nutricionista. É sempre recomendável buscar orientação profissional para um plano alimentar adequado às suas necessidades.
