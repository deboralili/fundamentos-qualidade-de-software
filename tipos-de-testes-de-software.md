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
