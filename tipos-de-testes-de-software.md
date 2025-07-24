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

