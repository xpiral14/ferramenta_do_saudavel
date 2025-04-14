# Meu Rastreador Pessoal: Nutrição e Medidas Corporais 📊🍎📏

Este é um projeto de aplicativo web estático simples, projetado para auxiliar no rastreamento pessoal de informações nutricionais diárias e medidas corporais, focado em objetivos de saúde e fitness, como emagrecimento e acompanhamento da composição corporal.

## 🎯 Objetivo

O objetivo principal deste rastreador é fornecer uma ferramenta prática e privada para:

1.  Registrar o consumo diário de alimentos, incluindo calorias e macronutrientes (proteínas, carboidratos, gorduras).
2.  Registrar medidas corporais (peso, cintura, quadril, etc.) em datas específicas.
3.  Visualizar resumos diários e semanais da ingestão nutricional.
4.  Acompanhar a evolução das medidas corporais através de histórico e gráficos.
5.  Comparar o desempenho nutricional e as mudanças nas medidas entre semanas.

Tudo isso **sem a necessidade de um backend ou banco de dados externo**, utilizando apenas o armazenamento local (`localStorage`) do navegador do usuário.

## ✨ Funcionalidades Principais

O rastreador é dividido em várias seções (páginas HTML separadas):

1.  **🏠 Início (`index.html`):** Página de boas-vindas com links para as outras seções.
2.  **📝 Registro Diário (`registro.html`):**
    *   Seleção de data.
    *   Adição de alimentos/refeições por tipo (Café da Manhã, Almoço, Jantar, Lanches).
    *   Entrada de descrição, calorias, proteínas, carboidratos e gorduras para cada item.
    *   Visualização da lista de alimentos registrados para o dia selecionado.
    *   Opção de remover itens registrados.
3.  **🎯 Plano Alimentar (`plano.html`):**
    *   Exibição estática de um plano alimentar de exemplo (baseado nas suas metas iniciais) para servir como referência.
4.  **📊 Resumo do Dia (`resumo.html`):**
    *   Seleção de data para visualização.
    *   Cálculo e exibição dos totais diários de calorias, proteínas, carboidratos e gorduras.
    *   Gráfico de rosca mostrando a distribuição de calorias por tipo de refeição.
    *   Gráfico de pizza mostrando a distribuição de macronutrientes (em gramas) no dia.
5.  **📏 Medidas (`medidas.html`):**
    *   Seleção de data para registrar as medidas.
    *   Campos para inserir diversas medidas corporais (Peso, Cintura, Quadril, Peito, Braços, Coxas, Panturrilhas).
    *   Botão para salvar as medidas do dia.
    *   Filtros para selecionar um período de datas (início e fim).
    *   Botão "Aplicar Filtro" para carregar/atualizar o histórico e os gráficos.
    *   Tabela exibindo o histórico de medidas registradas dentro do período filtrado.
    *   Gráficos de linha mostrando a evolução das principais medidas (Peso, Cintura, Quadril, Peito) ao longo do tempo (período filtrado).
    *   Opção de remover um registro de medidas de uma data específica.
6.  **📅 Resumo Semanal (`resumo_semanal.html`):**
    *   Seletores para escolher duas semanas distintas (semana atual e semana de comparação).
    *   Botão "Comparar Semanas" para processar os dados.
    *   Tabela comparativa exibindo:
        *   Médias diárias de calorias e macronutrientes para cada semana.
        *   Últimos valores de medidas corporais registrados dentro de cada semana.
        *   Variação percentual (%) entre as duas semanas para cada métrica, com indicadores visuais (cor/seta) de aumento ou diminuição.

## 💻 Tecnologias Utilizadas

*   **HTML5:** Estrutura das páginas.
*   **CSS3 (com Tailwind CSS):** Estilização e layout responsivo.
*   **JavaScript (Vanilla JS / ES6+):** Lógica de manipulação do DOM, cálculos, interações e gerenciamento de dados.
*   **Chart.js:** Biblioteca para criação dos gráficos de resumo e evolução.
*   **chartjs-adapter-date-fns:** Adaptador para Chart.js lidar corretamente com eixos de data/tempo.
*   **LocalStorage do Navegador:** Armazenamento persistente dos dados diretamente no navegador do usuário.

## 🚀 Como Usar

Como este é um projeto puramente front-end (estático):

1.  **Clone ou Baixe o Repositório:**
    ```bash
    git clone https://github.com/SEU_USUARIO/NOME_DO_REPOSITORIO.git
    cd NOME_DO_REPOSITORIO
    ```
    Ou baixe o arquivo ZIP e extraia-o.
2.  **Abra o `index.html`:** Navegue até a pasta do projeto e abra o arquivo `index.html` diretamente no seu navegador web preferido (Chrome, Firefox, Edge, etc.).
3.  **Comece a Usar:** Navegue pelas seções usando os links no topo e comece a registrar seus dados!

**Nenhuma instalação adicional ou servidor web é necessário.**

## ⚠️ Importante: Armazenamento Local

*   **Privacidade:** Seus dados de alimentação e medidas ficam armazenados **exclusivamente no navegador que você está usando**, através do `localStorage`. Eles não são enviados para nenhum servidor externo.
*   **Sem Backup na Nuvem:** Isso também significa que **não há backup automático**. Se você limpar os dados do seu navegador (cache, cookies, dados de sites) ou usar um navegador diferente ou o modo anônimo, os dados registrados serão perdidos. Considere exportar/anotar dados importantes periodicamente se precisar de um backup.
*   **Dependência do Navegador:** A funcionalidade depende da disponibilidade e permissão do `localStorage` no seu navegador.

## 📈 Possíveis Melhorias Futuras

*   Funcionalidade de **editar** registros existentes (alimentação e medidas).
*   Opção de **exportar/importar** dados (CSV, JSON) para backup ou análise externa.
*   Definição de **metas** nutricionais e de medidas, com visualização do progresso.
*   Melhorias na interface do usuário (UI) e experiência do usuário (UX).
*   Adição de mais opções de gráficos ou personalização.
*   Implementação como um Progressive Web App (PWA) para melhor experiência mobile e offline.
*   Validação mais robusta dos dados de entrada.

## 🙏 Agradecimentos

Este projeto foi desenvolvido com a assistência de uma Inteligência Artificial (modelo de linguagem da Google), que ajudou na geração de código, depuração e estruturação das funcionalidades.