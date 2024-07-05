
# Releases

Esta página contém informações sobre as diferentes versões lançadas do Projeto Mercasyst, incluindo notas de lançamento, alterações e links para downloads.

# Versão Atual: Mercasyst 1.0 r40

- ### **Data de Lançamento:** 20 de abril de 2024
- ### **Notas de Lançamento - Mercasyst 1.0 r40**

1. **[Mostrar Código de Barras](#tarefa-mostrar-código-de-barras)**
   - Implementada a exibição do código de barras na verificação de preço e no lançamento da compra.

2. **[Tela de Vendas](#tarefa-tela-de-vendas)**
   - Corrigido o problema que ocorria ao pressionar "ESC", impedindo a visualização das opções de alterar e pesquisar.

3. **[Impressão de Documento](#tarefa-impressão-de-documento)**
   - Corrigido o problema de impressão de duas vias do documento de venda em promissória, agora imprime apenas uma via.

4. **[Geração de Crédito SPED Cont Sisal Gomes](#tarefa-geração-de-crédito-sped-cont-sisal-gomes)**
   - Corrigido o problema na geração de crédito para PIS e COFINS na entrada fiscal de "Energia" no SPED Contribuições da Sisal Gomes.

5. **[Devolução de Cliente](#tarefa-devolução-de-cliente)**
   - Corrigido o erro que gerava saldo de vale compras em todas as filiais ao realizar uma devolução de cliente.

6. **[Impressão de Relatório](#tarefa-impressão-de-relatório)**
   - Corrigido o problema na impressão do relatório de compras, agora gera corretamente para períodos maiores que 5 dias e exibe mensagens de erro apropriadas.

7. **[Natureza de Operação](#tarefa-natureza-de-operação)**
   - Corrigido o problema em que a natureza marcada para gerar título "não" estava sendo gravada como devolução em vez de outros.

8. **[Tela de Devolução de Cliente](#tarefa-tela-de-devolução-de-cliente)**
   - Foram realizadas melhorias e correções na tela de devolução de cliente, incluindo a criação de um campo checkbox para devolução seletiva e a correção de erros de SQL.

9. **[Cadastro de Fornecedores](#tarefa-cadastro-de-fornecedores)**
   - Ajustado o padrão de filtro na pesquisa de fornecedores para evitar erros ao tentar pesquisar.



# Versão Anterior

### Mercasyst 1.0 r38

- **Data de Lançamento:** 5 de abril de 2024
- **Notas de Lançamento:**


## Tarefas Concluídas

#### Tarefa: Mostrar Código de Barras

- **Data de Registro:** 26/02/2024
- **Tipo de Tarefa:** Melhoria
- **Prioridade:** Média
- **Descrição:** Foi implementada a exibição do código de barras na verificação de preço e no lançamento da compra. Um novo layout foi criado para compor os dados, adicionando os campos "cod.Barras" e "Margem". Além disso, um painel foi adicionado ao layout para exibir os dados adicionais de cada produto.
- **Status:** Concluída

| Tabela de Informações |
|-----------------------|
| **Caminho:** Entradas - Gerenciamento de compras - Novo |
| **Tipo de Tarefa:** Melhoria |
| **Localização:** ALR Tecnologia |
| **Responsável:** Andreina Oliveira |
| **Base:** Mercasyst |

---

### Tarefa: Tela de Vendas

- **Data de Registro:** 15/03/2024
- **Tipo de Tarefa:** Erro
- **Prioridade:** Alta
- **Descrição:** Quando o usuário clica em "ESC", as opções de alterar e pesquisar não estão mais aparecendo. A tela é fechada completamente.
- **Status:** Concluída

| Tabela de Informações |
|-----------------------|
| **Caminho:** Na tela de vendas, clicar em "ESC" |
| **Tipo de Tarefa:** Erro |
| **Localização:** ALR Tecnologia |
| **Base:** Mercasyst |
| **Responsável:** Andreina Oliveira |
| **Observação:** Testar replicar tarefa para Mercasyst e Ultracash |

---


### Tarefa: Impressão de Documento

- **Data de Registro:** 25/03/2024
- **Tipo de Tarefa:** Melhoria
- **Prioridade:** Urgente
- **Descrição:** Após realizar uma venda de promissória para o cliente, o sistema estava imprimindo duas vias do documento para o cliente assinar, sendo necessário apenas uma.
- **Status:** Concluída

| Tabela de Informações |
|-----------------------|
| **Caminho:** Fazer uma venda em promissória e finalizar. O sistema perguntará se deseja imprimir o documento da venda. Se sim, serão impressas duas vias. |
| **Tipo de Tarefa:** Melhoria |
| **Localização:** Ricardo Supermercado - Queimadas |
| **Base:** Mercasyst |
| **Responsável:** Andreina Oliveira |


---

### Tarefa: Geração de Crédito SPED Cont Sisal Gomes

- **Data de Registro:** 18/03/2024
- **Tipo de Tarefa:** Erro
- **Prioridade:** Urgente
- **Descrição:** A entrada fiscal de "Energia" no SPED Contribuições da Sisal Gomes não estava gerando crédito conforme esperado. Após investigação, foi identificado que a geração de crédito para PIS e COFINS não estava sendo realizada corretamente para essa categoria de entrada. A solução foi implementar a geração de crédito adequada para PIS e COFINS, conforme informado pela contabilidade da empresa.
- **Status:** Concluída

| Tabela de Informações |
|-----------------------|
| **Caminho:** Entrada fiscal de "Energia" no SPED Contribuições da Sisal Gomes |
| **Tipo de Tarefa:** Erro |
| **Localização:** 9TEC |
| **Base:** Ultracash |
| **Responsável:** Eric |
| **Observação:** Testar nas duas bases |

---


### Tarefa: Devolução de Cliente

- **Data de Registro:** 25/03/2024
- **Tipo de Tarefa:** Erro
- **Prioridade:** Urgente
- **Descrição:** Ao realizar uma devolução de cliente, o sistema estava gerando um saldo de vale compras para o cliente em todas as filiais, quando deveria gerar somente na filial onde foi feita a devolução.
- **Status:** Concluída

| Tabela de Informações |
|-----------------------|
| **Caminho:** Saídas, outros procedimentos, devolução de cliente. Realizar uma devolução para algum cliente e, em seguida, acessar o cadastro do cliente. Clicar com o botão direito do mouse em "Vale Compras" e selecionar "Consulta Saldo do Cliente". |
| **Tipo de Tarefa:** Erro |
| **Localização:** Elias Contorno Material de Construção - Coité |
| **Base:** Mercasyst |
| **Responsável:** Gabriel Matos da Silva |
| **Observação:** Testar nas duas bases |

---


### Tarefa: Impressão de Relatório

- **Data de Registro:** 25/03/2024
- **Tipo de Tarefa:** Erro
- **Prioridade:** Urgente
- **Descrição:** Ao tentar imprimir o relatório de compras, o sistema não estava gerando o relatório em tela quando o período selecionado era maior que 5 dias. Não foram exibidas mensagens de erro para indicar o motivo da falha na geração do relatório. A falha foi corrigida e agora o sistema gera corretamente o relatório mesmo para períodos maiores que 5 dias, e mensagens de erro apropriadas foram implementadas para orientar o usuário em caso de problemas.
- **Status:** Concluída

| Tabela de Informações |
|-----------------------|
| **Caminho:** Relatórios - Entradas - Resumo das compras |
| **Tipo de Tarefa:** Erro |
| **Localização:** Ricardo Supermercado - Queimadas |
| **Base:** Mercasyst |
| **Responsável:** Andreina Oliveira |

---

### Tarefa: Natureza de Operação

- **Data de Registro:** 27/03/2024
- **Tipo de Tarefa:** Erro
- **Prioridade:** Urgente
- **Descrição:** Nas operações em que a natureza estava marcada para gerar título "não", estava sendo gravada como devolução em vez de outros. O problema foi identificado e corrigido, agora as operações são gravadas corretamente conforme a configuração da natureza.
- **Status:** Concluída

| Tabela de Informações |
|-----------------------|
| **Caminho:** Não especificado |
| **Tipo de Tarefa:** Erro |
| **Localização:** Supermercado Popular - Cansanção |
| **Base:** Mercasyst |
| **Responsável:** Andreina Oliveira |


---

### Tela de Devolução de Cliente

1. **Criar Campo Checkbox para Devolução Seletiva:**
   - Um campo de checkbox foi adicionado, permitindo ao cliente selecionar todos ou itens específicos para devolução.

2. **Corrigir Erro de SQL ao Gravar Devolução:**
   - O erro de SQL que ocorria ao tentar gravar a devolução foi resolvido.

3. **Permitir Digitação na Coluna Quantidade:**
   - Agora é possível digitar diretamente na coluna de quantidade, sem a necessidade de clicar previamente.

----

### Cadastro de Fornecedores

1. **Ajustar Padrão de Filtro na Pesquisa:**
   - Na tela de pesquisa de fornecedores, foi alterado o padrão de filtro para que a opção "Exclusivo por Código" não esteja mais selecionada por padrão. Isso evita erro ao tentar pesquisar.
