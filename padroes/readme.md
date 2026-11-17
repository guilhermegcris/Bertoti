## ⚖️ Minhas Contribuições - JurisAI

Este documento detalha as minhas contribuições pessoais para o desenvolvimento do JurisAI, assistente inteligente de conhecimento jurídico desenvolvido no repositório joaosantos13/Padroes-De-Projetos.

O meu foco no projeto foi a implementação do padrão de projeto Strategy (Strategy Pattern), definindo os critérios de classificação das dúvidas jurídicas e especializando o tratamento de consultas de acordo com a natureza da legislação aplicável (Constituição Federal, legislação específica, jurisprudência e dúvidas gerais).

## 💻 O que eu desenvolvi

Implementação do Strategy Pattern (LegalStrategy e Estratégias Concretas):
Estruturei a camada de estratégias dentro do pacote com.jurisai.pattern.strategy para permitir que o agente alterne dinamicamente o comportamento de busca e tratamento conforme o contexto jurídico da pergunta:

ConstitutionalStrategy: Especializada em questões envolvendo direitos fundamentais, garantias e princípios da Constituição Federal de 1988.

LegislationStrategy: Direcionada a leis ordinárias e códigos específicos do escopo do projeto, como o Código de Defesa do Consumidor (CDC) e a Lei Geral de Proteção de Dados (LGPD).

JurisprudenceStrategy: Focada na recuperação de entendimentos de tribunais, súmulas e precedentes judiciais relevantes.

GeneralLegalStrategy: Estratégia padrão (fallback) para dúvidas jurídicas abrangentes ou que não se enquadram estritamente nas categorias anteriores.

Critérios de Seleção e Roteamento de Estratégia (StrategyFactory):
Desenvolvi o mecanismo responsável por avaliar a dúvida jurídica submetida e selecionar em tempo de execução a instância de LegalStrategy mais adequada, desacoplando a lógica de decisão do fluxo principal do LegalAgent.

Integração com a Base de Conhecimento (RAG) e Comandos:
Adaptei os contratos de execução das estratégias para orquestrar consultas direcionadas à base de conhecimento jurídica e alinhar o retorno das fontes legais ao fluxo dos comandos de busca (Command) e geração de respostas via Spring AI.

## 📐 Estrutura de Arquivos Criados

Os arquivos foram organizados seguindo a estrutura de pacotes do repositório na branch Strategy:

src/main/java/com/jurisai/
└── pattern/
    └── strategy/
        ├── LegalStrategy.java           <- Interface base do Strategy Pattern
        ├── ConstitutionalStrategy.java  <- Estratégia para Constituição Federal
        ├── LegislationStrategy.java     <- Estratégia para Leis Específicas (CDC, LGPD)
        ├── JurisprudenceStrategy.java   <- Estratégia para Jurisprudência e Súmulas
        ├── GeneralLegalStrategy.java    <- Estratégia padrão para dúvidas gerais
        └── StrategyFactory.java         <- Seletor dinâmico de estratégias jurídicas


## 🚀 Como testar a minha contribuição

Para validar a compilação das estratégias, os critérios de seleção e a execução da branch Strategy, execute os comandos abaixo no terminal:

git clone https://github.com/joaosantos13/Padroes-De-Projetos.git
cd Padroes-De-Projetos
git checkout Strategy
./mvnw clean compile
./mvnw test
./mvnw spring-boot:run
