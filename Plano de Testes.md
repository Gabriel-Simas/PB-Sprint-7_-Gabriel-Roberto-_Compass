# Plano de Testes - Sprint 2: Mergulhando em Testes de APIs

**link para download**: 

**Autor**: Gabriel Simas Roberto da Silva

**Data:** 21/09/2023

**Versão do Documento:** 2.0

## Índice
1. Introdução
   1.1 Definições
   1.2 Abreviações
2. Definição de Escopo e Objetivos
   2.1 Escopo
   2.2 Objetivos
3. Estratégias de Testes
4. Suite de Casos de Teste
5. Candidatos para Automação de Testes
6. Ferramentas
7. Prioridades

## 1. Introdução
Nesta Sprint, o objetivo é garantir a qualidade da funcionalidade de cadastro de vendedores (usuários) em um Marketplace. Este plano de testes aborda o planejamento, escopo, estratégias, casos de teste, candidatos para automação, ferramentas e prioridades relacionadas aos testes desta Sprint.

### 1.1 Definições
- **Git**: Sistema de controle de versão.
- **Gitlab**: Plataforma de gerenciamento de código.
- **API**: Interface de Programação de Aplicativos.

### 1.2 Abreviações
- **CRUD**: Create, Read, Update, Delete.

## 2. Definição de Escopo e Objetivos

### 2.1 Escopo
O escopo dos testes para a Sprint 2 está centrado na funcionalidade de cadastro de vendedores (usuários) no Marketplace. Isso inclui todas as operações CRUD (Create, Read, Update, Delete) relacionadas aos vendedores. Especificamente, o escopo abrange:

- **Criação de Vendedores (Create)**: Verificar a capacidade do sistema de criar novos registros de vendedores no Marketplace, incluindo a inserção de informações básicas, como nome, e-mail, senha e administração.

- **Leitura de Vendedores (Read)**: Validar a capacidade do sistema de recuperar informações dos vendedores já cadastrados. Isso inclui a verificação da capacidade de listar vendedores existentes e visualizar detalhes de vendedores individuais.

- **Atualização de Vendedores (Update)**: Certificar-se de que o sistema permite a atualização das informações de vendedores, incluindo nome, e-mail e status de administração. Além disso, verificar a capacidade de atualizar informações de vendedores não existentes.

- **Exclusão de Vendedores (Delete)**: Garantir que o sistema permita a exclusão de registros de vendedores de acordo com as regras definidas. Isso inclui a exclusão de vendedores existentes e a tentativa de exclusão de vendedores inexistentes.

- **Testes de Limites e Validações**: Incluir testes que verifiquem os limites de funcionamento do sistema, como senhas com o mínimo e máximo de caracteres permitidos, bem como a validação de e-mails.

### 2.2 Objetivos
Os objetivos dos testes da Sprint 2 são os seguintes:

- **Validação da Funcionalidade**: Garantir que a funcionalidade de cadastro de vendedores esteja implementada de acordo com os requisitos definidos.

- **Cumprimento dos Critérios de Aceitação**: Verificar se todos os critérios de aceitação estabelecidos para a funcionalidade de cadastro de vendedores são atendidos.

- **Garantia de Qualidade**: Assegurar que o cadastro de vendedores seja robusto, livre de erros e possa ser usado com confiança pelos usuários finais.

- **Identificação de Problemas**: Detectar eventuais bugs ou problemas na funcionalidade e documentá-los como issues para correção posterior.

- **Preparação para Automação**: Identificar casos de teste candidatos para automação, facilitando testes futuros e aumentando a eficiência do processo de teste.

- **Melhoria Contínua**: Propor sugestões de melhorias para a funcionalidade com base na análise de testes.

## 3. Estratégia de Testes

A estratégia de testes para a Sprint 2 é projetada para abordar de forma eficaz a funcionalidade de cadastro de vendedores (usuários) em um Marketplace. A estratégia inclui os seguintes elementos:

### 3.1 Testes Manuais e Exploratórios
- **Testes Manuais**: Serão realizados testes manuais detalhados para todos os casos de teste identificados. Isso envolve a execução de ações manuais no sistema e a verificação dos resultados em relação aos critérios de aceitação.
- **Exploração de Cenários Alternativos**: Além dos cenários principais, os testadores explorarão cenários alternativos para identificar possíveis falhas e áreas de melhoria na funcionalidade.

### 3.2 Automação de Testes
- **Identificação de Candidatos para Automação**: Alguns casos de teste serão identificados como candidatos para automação. Isso inclui testes que são repetitivos, de alto risco ou críticos para a funcionalidade.
- **Desenvolvimento de Scripts de Automação**: Para os candidatos à automação, serão desenvolvidos scripts de automação de teste usando ferramentas apropriadas, como o Postman.

### 3.3 Validação de Limites e Validações
- Serão realizados testes específicos para validar os limites da funcionalidade, como:
   - Senhas com o mínimo e máximo de caracteres permitidos.
   - Validação de e-mails.
   - Conformidade com padrões de entrada.

### 3.4 Análise de Dados
- Durante os testes, os dados usados para a criação, atualização e exclusão de vendedores serão analisados para garantir que estejam corretos e que correspondam aos critérios de aceitação definidos.

### 3.5 Registro de Issues e Sugestões de Melhoria
- Qualquer problema encontrado durante os testes, como bugs ou comportamento inesperado, será documentado como issues no GitLab. As issues incluirão detalhes sobre como reproduzir o problema e o comportamento esperado.
- Sugestões de melhorias também serão registradas como issues, fornecendo informações sobre as melhorias propostas na funcionalidade.

### 3.5 Priorização de Testes
- Os casos de teste foram priorizados com base na importância e impacto no sistema. Isso permite que os testes mais críticos sejam realizados primeiro.

Essa estratégia de testes visa garantir que a funcionalidade de cadastro de vendedores seja testada de forma abrangente, que problemas sejam identificados e registrados adequadamente, e que casos de teste candidatos à automação sejam identificados para melhorar a eficiência dos testes futuros. Além disso, a exploração de cenários alternativos ajudará a garantir a robustez do sistema.

## 4. Suite de Casos de Teste

A suíte de casos de teste para a Sprint 2 é projetada para cobrir as principais funcionalidades relacionadas ao cadastro de vendedores (usuários) no Marketplace. A suíte incluirá os seguintes casos de teste:

### Caso de Teste 1: Criação de Novo Vendedor
- **Descrição**: Verificar a capacidade do sistema de criar com sucesso um novo registro de vendedor com informações válidas.
- **Passos**:
   1. Acessar a tela de cadastro de vendedor.
   2. Preencher todos os campos obrigatórios com informações válidas.
   3. Enviar o formulário de cadastro.
- **Critérios de Sucesso**:
   - O sistema cria um novo registro de vendedor.
   - O vendedor é redirecionado para uma página de confirmação.

### Caso de Teste 2: Leitura de Informações de Vendedor
- **Descrição**: Verificar a capacidade do sistema de exibir as informações de um vendedor existente.
- **Passos**:
   1. Acessar a página de detalhes de um vendedor.
- **Critérios de Sucesso**:
   - O sistema exibe corretamente todas as informações do vendedor.
   - Não há erros de exibição.

### Caso de Teste 3: Atualização de Detalhes do Vendedor
- **Descrição**: Verificar a capacidade do sistema de atualizar as informações de um vendedor.
- **Passos**:
   1. Acessar a página de edição de um vendedor.
   2. Modificar as informações do vendedor.
   3. Enviar o formulário de edição.
- **Critérios de Sucesso**:
   - O sistema atualiza com sucesso as informações do vendedor.
   - O vendedor é redirecionado para uma página de confirmação.

### Caso de Teste 4: Exclusão de Vendedor
- **Descrição**: Verificar a capacidade do sistema de excluir um vendedor.
- **Passos**:
   1. Acessar a página de exclusão de um vendedor.
   2. Confirmar a exclusão.
- **Critérios de Sucesso**:
   - O sistema exclui com sucesso o registro do vendedor.
   - O vendedor não é mais listado no sistema.

### Caso de Teste 5: Teste de Senha com Mínimo e Máximo de Caracteres
- **Descrição**: Verificar se o sistema valida corretamente senhas com o número mínimo e máximo de caracteres permitidos.
- **Passos**:
   1. Tentar criar um vendedor com uma senha abaixo do limite mínimo de caracteres.
   2. Tentar criar um vendedor com uma senha acima do limite máximo de caracteres.
- **Critérios de Sucesso**:
   - O sistema impede a criação de vendedores com senhas que não atendem aos critérios de comprimento.

### Caso de Teste 6: Validação de E-mail
- **Descrição**: Verificar se o sistema valida corretamente os endereços de e-mail dos vendedores.
- **Passos**:
   1. Tentar criar um vendedor com um endereço de e-mail inválido (sem formato de e-mail válido).
   2. Tentar criar um vendedor com um endereço de e-mail de provedores específicos, como "gmail" e "hotmail".
- **Critérios de Sucesso**:
   - O sistema impede a criação de vendedores com endereços de e-mail inválidos ou de provedores específicos.

### Caso de Teste 7: Teste de Campos Obrigatórios
- **Descrição**: Verificar se o sistema valida corretamente os campos obrigatórios durante o cadastro de vendedores.
- **Passos**:
   1. Tentar criar um vendedor deixando campos obrigatórios em branco.
- **Critérios de Sucesso**:
   - O sistema impede a criação de vendedores com campos obrigatórios em branco.

## 5. Candidatos para Automação de Testes

1. **Criação de Novo Vendedor**: Este caso de teste verifica a capacidade do sistema de criar com sucesso um novo registro de vendedor com informações válidas. A automação deste caso de teste pode economizar tempo, pois a criação de vendedores é uma tarefa repetitiva.

2. **Leitura de Informações de Vendedor**: Este caso de teste verifica se o sistema pode exibir corretamente as informações de um vendedor existente. A automação deste caso pode garantir que a exibição das informações do vendedor seja consistente em todas as execuções de teste.

3. **Atualização de Detalhes do Vendedor**: Verifica se o sistema é capaz de atualizar corretamente as informações de um vendedor. A automação deste caso de teste pode acelerar o processo de teste de atualização de informações.

A automação desses casos de teste pode trazer benefícios significativos, como economia de tempo e repetição consistente dos testes. No entanto, é importante lembrar que a escolha de quais casos de teste automatizar deve levar em consideração a frequência de execução e a complexidade do teste. Casos de teste que são executados com frequência e envolvem etapas repetitivas são candidatos ideais para automação.

## 6. Ferramentas
- **Descrição**: O Postman é uma ferramenta de colaboração para testar, desenvolver e documentar APIs. Ele permite criar solicitações HTTP personalizadas, automatizar testes e validar respostas de API.
- **Uso na Sprint 2**: O Postman será usado para mapear os cenários de teste, criar solicitações para a API em questão, executar testes manuais e validar as respostas da API. Também é útil para a automação de testes de API, se aplicável.
O Postman é uma escolha popular para testes de API devido à sua facilidade de uso, capacidade de automação e recursos de documentação. Ele desempenhará um papel fundamental na validação da funcionalidade da API durante a Sprint 2.

## 7. Prioridades

As prioridades foram atribuídas com base na importância e impacto no sistema, garantindo que os testes mais críticos sejam realizados primeiro:

1. **Criação de Novo Vendedor**: A criação de novos vendedores é uma operação fundamental e crítica para o funcionamento do Marketplace. Portanto, é a prioridade máxima, pois qualquer falha nessa funcionalidade pode impactar seriamente o negócio.

2. **Leitura de Informações de Vendedor**: A capacidade de ler informações de vendedores existentes também é essencial para o funcionamento correto do sistema. Garantir que as informações possam ser lidas com precisão é uma prioridade alta.

3. **Atualização de Detalhes do Vendedor**: A atualização de informações de vendedores é uma operação importante para manter dados precisos e atualizados. Portanto, é uma prioridade significativa, mas ligeiramente inferior à criação e leitura de vendedores.

4. **Exclusão de Vendedor**: Embora a exclusão de vendedores seja importante, ela é priorizada abaixo das operações anteriores, pois erros nessa funcionalidade podem ser corrigidos mais facilmente sem afetar drasticamente o sistema.

5. **Teste de Senha com Mínimo e Máximo de Caracteres**: Testes relacionados a senhas são importantes para garantir a segurança dos dados, mas, neste caso, são priorizados após as funcionalidades principais.

6. **Validação de E-mail**: A validação de e-mail é importante, mas é classificada como uma prioridade mais baixa em comparação com as funcionalidades centrais do cadastro de vendedores.

7. **Teste de Campos Obrigatórios**: Testar campos obrigatórios é importante para evitar registros incompletos, mas é uma prioridade menor em relação às principais funcionalidades.

Essa priorização ajuda a garantir que os testes mais críticos sejam executados primeiro, permitindo que os problemas mais impactantes sejam identificados e resolvidos rapidamente. Conforme o tempo e os recursos permitirem, os testes com prioridades mais baixas também serão realizados para garantir uma cobertura completa.
