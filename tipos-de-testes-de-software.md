# 🧪 Tipos de Testes de Software

Este resumo apresenta os principais tipos de testes utilizados no processo de garantia de qualidade de software.
Dividem-se, principalmente, em duas abordagens: **estáticos e dinâmicos**, além de métodos de execução como **testes manuais e automatizados**.
Por fim, são explorados os **níveis e classificações de testes** mais utilizados na prática.

## ✅ Testes Estáticos
Testes estáticos analisam o código **sem executá-lo**. 
O objetivo é identificar erros, violações de boas práticas, falhas de segurança e inconsistências de lógica logo nas fases iniciais do desenvolvimento.
Podem incluir:

- Revisões manuais de código (code review);
- Análise automatizada com ferramentas como: FindBugs (Java), SonarQube, ESLint (JavaScript), Pylint (Python).

> 💡 Por não exigir a execução do sistema, os testes estáticos são considerados **testes de caixa branca**, focando na estrutura interna do código.

## ⚙️ Testes Dinâmicos
Os testes dinâmicos envolvem a **execução do sistema**.
Insere-se uma entrada, observa-se o comportamento do sistema e valida-se a saída.
<br/>
Esses testes avaliam:
- Comportamento funcional;
- Tempo de resposta e performance;
- Compatibilidade com diferentes ambientes;
- Robustez frente a dados inesperados.

> 🔎 Testes dinâmicos podem ser tanto caixa preta quanto caixa branca, dependendo da abordagem adotada.

## 🧑‍💻 Testes Manuais
Testes executados diretamente por uma pessoa, sem o auxílio de scripts automatizados.
<br/>
São úteis especialmente em:
- Casos em que a automação não é viável ou eficiente;
- Testes exploratórios;
- Verificação visual de elementos da interface.

Vantagens:
- Flexibilidade e adaptação rápida;
- Útil em estágios iniciais.

Desvantagens:
- Alto custo;
- Maior chance de erro humano;
- Dificuldade de repetição com precisão.

## 🤖 Testes Automatizados
São testes executados por scripts e ferramentas que simulam ações humanas ou testam funcionalidades diretamente no código.
<br/>
Podem variar desde testes simples de unidades (unit tests), até fluxos completos de navegação em uma interface (UI tests).

Vantagens:
- Repetibilidade;
- Velocidade;
- Detecção precoce de bugs em builds contínuos (CI/CD).

Desvantagens:
- Custo inicial para desenvolvimento dos testes;
- Manutenção dos scripts conforme o sistema evolui.

# 🔍 Classificação dos Testes de Software

## 1. 🧪 Testes de Unidade

Focados em testar partes isoladas do código, como **funções ou métodos**.

- Geralmente realizados por desenvolvedores;
- Cobrem apenas pequenas partes da aplicação;
- Executados rapidamente e com frequência.

Ferramentas comuns: Jest, JUnit, pytest.

## 2. 🔗 Testes de Integração

Avaliam se **módulos diferentes** interagem corretamente entre si.
<br/>
Exemplos:
- Comunicação entre o front-end e o banco de dados;
- Integração entre serviços REST.

> 🧠 São importantes para detectar problemas em pontos de comunicação entre partes do sistema.

## 3. ✅ Testes Funcionais

Verificam se o sistema cumpre os **requisitos funcionais** definidos, ou seja, se ele faz o que deveria fazer.
- Ignoram o funcionamento interno;
- Avaliam as entradas e as saídas de um sistema;
- São normalmente testes de caixa preta.

## 4. 🔁 Testes de Ponta a Ponta (End-to-End)

Simulam o **fluxo completo do usuário**, desde o início até o fim de um processo.
<br/>
Exemplo de cenário:
- Login → Adição de item ao carrinho → Pagamento → Confirmação.

> ⚠️ São testes mais demorados e frágeis a mudanças na interface, mas fornecem uma visão completa da experiência do usuário.

## 5. 📋 Testes de Aceitação

Validam se o software **atende às expectativas e critérios de aceitação do cliente ou usuário final**.

- Muitas vezes escritos em linguagem natural;
- Podem ser baseados em histórias de usuário;
- São essenciais antes de uma entrega.

Frameworks populares: Cucumber, Behave.

## 6. 🚀 Testes de Desempenho

Analisam como o sistema se comporta sob **cargas específicas**.
<br/>
Tipos:
- Teste de carga (load test): avalia desempenho sob demanda normal;
- Teste de estresse (stress test): simula picos de uso;
- Teste de escalabilidade: verifica capacidade de adaptação ao crescimento.

Ferramentas: JMeter, Gatling, Locust.

## 7. 💨 Testes de Fumaça (Smoke Tests)

Executados rapidamente para garantir que as **funcionalidades principais** estão funcionando após uma nova versão ser implementada.

> São como um "teste inicial" antes de rodar testes mais detalhados.
