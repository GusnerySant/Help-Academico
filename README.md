# Help Acadêmico

## Integrantes do Grupo
* **Edivaldo de Souza Santos**
* **Gustavo Nery dos Santos**
* **João Victor Menezes Santos**
* **Wilgner da Silva Gomes**

---

O projeto se trata de uma atividade avaliativa desenvolvida em caráter interdisciplinar, atendendo às
disciplinas de **Engenharia de Software** e **Gerência de Projetos**, ambas ministradas no Instituto Federal
de Sergipe – Campus Lagarto. A proposta consiste em um software voltado ao **bem-estar psicológico do
estudante universitário**, motivado por um cenário nacional preocupante de ansiedade, depressão e sobrecarga
acadêmica entre os discentes brasileiros, evidenciado por levantamentos como os da OMS, FONAPRACE, Datafolha
e IBGE.

De caráter **multiplataforma** (web e mobile) e **híbrido** (online/offline), o Help Acadêmico integra alunos,
professores e equipes psicopedagógicas de uma instituição de ensino em um único ambiente, oferecendo desde
conteúdos de autoajuda e organização de estudos até agendamento de consultas psicológicas e teleconsultas.

Por reunir as duas disciplinas num único artefato, este documento está organizado em dois grandes blocos:
um **módulo de Engenharia de Software** — elicitação e especificação de requisitos, modelagem UML, protótipos
— e um **módulo de Gerência de Projetos** — escopo formal, EAP, cronograma e matriz de riscos. Cada seção abaixo
indica a qual dos dois módulos pertence.

---

## Stakeholders do Projeto
*(Gerência de Projetos)*

O levantamento de partes interessadas segue uma estrutura em camadas, prática comum tanto na etapa de
**elicitação de requisitos** quanto no **planejamento de stakeholders** em Gerência de Projetos, garantindo que
a especificação e o plano do projeto capturem as necessidades de todos os públicos envolvidos:

| Camada | Exemplos |
|---|---|
| Equipe do projeto | Orientadores e desenvolvedores (planejamento, desenvolvimento, teste e manutenção) |
| Instituição cliente | Direção-Geral, Reitoria (IFS), COAE, PROGEP, CTI |
| Usuários finais | Alunos, professores, equipe pedagógica/psicopedagógica |
| Governo e regulamentação | MEC, Ministério da Saúde, CFP, ANPD (LGPD) |
| Partes indiretamente afetadas | Famílias dos alunos, comunidade acadêmica e científica, sociedade |

---

## Escopo e Não-Escopo do Projeto
*(Gerência de Projetos)*

### Escopo
O Help Acadêmico cobre quatro grandes frentes de atuação:

1. **Funcionamento Geral** — cadastro e autenticação por perfil, comunicação segura entre usuários (chat
individual e em grupo), personalização de interface e acessibilidade, uso offline com sincronização automática
e gamificação do engajamento.
2. **Cuidado Psicológico Básico** — conteúdo educativo sobre saúde mental, exercícios de bem-estar (respiração,
mindfulness), diário emocional, terapia em grupo online e fóruns de comunidade moderados.
3. **Consultas e Teleconsultas** — agendamento de atendimento presencial no campus e teleconsulta com
psicólogos/psiquiatras licenciados, prontuário digital confidencial, lembretes automáticos e lista de espera.
4. **Organização de Estudos** — materiais e técnicas de estudo ativo validadas, oficinas conduzidas por
professores voluntários, cronogramas de estudo adaptativos e relatórios acadêmico-comportamentais.
5. **Governo e Regulamentação** — painéis institucionais anonimizados, exportação de relatórios ao MEC,
auditoria contínua de acessos, validação de credenciais profissionais e conformidade com LGPD e ECA.

### Não-Escopo (Fronteiras e Exclusões)
Delimitar explicitamente o que o sistema **não** fará é parte central do planejamento de escopo em Gerência de
Projetos — evita ambiguidade de expectativa entre equipe, orientadores e instituição adotante:

| Fronteira | O que fica de fora |
|---|---|
| Inteligência Preditiva e Diagnósticos Clínicos | Não há IA de inferência clínica, análise estatística avançada ou emissão de laudo médico — apenas triagem e notificação por regras/palavras-chave |
| Integração de Videoconferência Nativa | Não há motor próprio de streaming; a chamada de vídeo depende de redirecionamento a serviços de terceiros |
| Atuação frente ao ERP Acadêmico | Não substitui o sistema núcleo da reitoria (matrícula, diário de classe, emissão de histórico/diploma) |
| Geração Autônoma de Conteúdo | Cronogramas, flashcards e simulados dependem de curadoria manual do corpo docente, não de geração automática |
| Integração com Hardwares Biométricos | Não há captura de dados biométricos reais (frequência cardíaca, pressão arterial); a leitura de tendências é só por interação no app |

---

## EAP (Estrutura Analítica do Projeto) e Cronograma
*(Gerência de Projetos)*

O planejamento temporal segue a lógica clássica de decomposição da **EAP**, traduzida em um **Gráfico de
Gantt** com marcos por fase (concepção, elicitação de requisitos, modelagem, prototipação, matriz de riscos e
monitoramento/controle), mantido em planilha externa por recomendação da orientação da disciplina:

📎 [Cronograma completo (Google Sheets)](https://docs.google.com/spreadsheets/d/1bFW-JVixpJjC0y7ZB1UveXrAE9wBstQTG19gFmWm2JE/edit?usp=sharing)

A mesma planilha detalha a distribuição de responsabilidade dos **89 requisitos funcionais** entre os quatro
integrantes, de forma equilibrada (~22 requisitos por pessoa), reduzindo o risco de concentração de
conhecimento em um único responsável.

---

## Matriz de Riscos do Projeto
*(Gerência de Projetos)*

O projeto adota uma matriz de riscos qualitativa-quantitativa inspirada na prática de mercado/setor público
(referência: orientação do TCU sobre matriz de riscos em contratações, art. 103 da Lei 14.133/2021), adaptada
para um contexto acadêmico sem contraparte contratual. A alocação de cada risco é feita **por papel/frente**
responsável (Equipe Dev, Orientador, Instituição/IFS, Colaborador externo ou Compartilhado), em vez de por
pessoa nomeada — preservando o princípio de que o risco deve ser atribuído a quem tem melhor capacidade de
geri-lo.

**Metodologia:** cada risco recebe uma nota de Probabilidade (1–3) e Impacto (1–3); o produto define o Nível:

| Probabilidade × Impacto | Nível | Interpretação |
|---|---|---|
| 1 a 2 | Baixo | Pode ser acompanhado sem prioridade imediata |
| 3 a 4 | Médio | Deve ser monitorado e tratado no planejamento |
| 6 | Alto | Exige ação de mitigação definida |
| 9 | **Crítico** | Exige decisão imediata, priorização ou redução de escopo |

> O nível **Crítico** é reservado a eventos cuja materialização acarrete ameaça direta à vida ou integridade
> dos usuários, severas sanções civis/criminais de conformidade jurídica para a instituição, ou que
> inviabilizem de forma irreversível a continuidade do projeto.

**40 riscos identificados**, distribuídos em 6 categorias:

1. Riscos de Domínio (saúde mental)
2. Riscos Regulatórios e de Conformidade (LGPD, ECA, CFP)
3. Riscos Técnicos e de Arquitetura
4. Riscos de Planejamento e Gestão do Projeto
5. Riscos Operacionais / Equipe
6. Riscos de Segurança da Informação e Privacidade

Após revisão criteriosa item a item, seis riscos foram classificados como **Crítico**, todos ligados direta ou
indiretamente à possibilidade de falha na identificação/atendimento de um caso real de risco à vida, a
vazamento de dados clínicos sensíveis em massa, ou à inviabilização irreversível de um módulo central do
sistema — entre eles, a falha de detecção de crise no diário mental (incluindo variação por gírias/regionalismos),
a não conformidade com a LGPD, a condicionante jurídica não detalhada de legalização do módulo de
teleconsulta, a contradição arquitetural entre criptografia ponta a ponta e triagem automática de risco, e o
roubo de credenciais por engenharia social.

A matriz completa — com implicação, mitigação, alocação e justificativa de nível para cada um dos 40 riscos —
está disponível no documento principal do projeto.

---

## Engenharia de Requisitos
*(Engenharia de Software)*

### Requisitos Funcionais
São **89 requisitos** (REQ-001 a REQ-089), organizados por domínio temático: Funcionamento Geral, Cuidado
Psicológico Básico, Consultas e Teleconsultas, Organização de Estudos e Governo/Regulamentação. Cada requisito
possui código, título e descrição, cobrindo funcionalidades como cadastro por perfil, chat interno, diário
emocional, agendamento de consultas, cronograma de estudos e relatórios integrados acadêmico-emocionais.

### Requisitos Não Funcionais
Do REQ-078 ao REQ-089, tratam de qualidades transversais do sistema:
* **Desempenho** — leveza em dispositivos e redes de baixa capacidade;
* **Segurança** — criptografia ponta a ponta, proteção contra SQL Injection, XSS e força bruta;
* **Escalabilidade** — suporte a crescimento progressivo de usuários e expansão para outros campi;
* **Interoperabilidade** — integração via APIs com sistemas acadêmicos e de saúde já existentes;
* **Portabilidade** — funcionamento uniforme em web, Android e iOS;
* **Usabilidade e Acessibilidade** — design responsivo, compatibilidade com leitores de tela;
* **Retenção de Dados** — regras claras de retenção de dados acadêmicos e clínicos.

### Histórias de Usuário
Cada requisito funcional é acompanhado de uma **História de Usuário**, no formato ágil
_"Como [papel], quero [ação], para [objetivo]"_, junto de critérios de aceitação verificáveis — prática que
conecta o levantamento de requisitos a metodologias ágeis (Scrum/XP), tornando a especificação testável.

---

## Casos de Uso (UML)
*(Engenharia de Software)*

O documento detalha **81 Casos de Uso**, seguindo o padrão clássico de modelagem UML/RUP, cada um com:

* Ator principal e atores secundários;
* Pré-condições;
* Fluxo principal numerado;
* Fluxos alternativos (`A1`, `A2`...) e fluxos de exceção (`FA01`, `FA02`...);
* Pós-condições.

Os casos de uso cobrem desde autenticação e cadastro de usuários até funcionalidades específicas do domínio,
como backup automático criptografado, sincronização de calendário acadêmico, gamificação de aprendizado,
acesso offline com sincronização e canais de comunicação interna (chat individual e em grupo).

---

## Protótipos de Tela
*(Engenharia de Software)*

Wireframes/mockups de interface são vinculados diretamente aos requisitos que representam (ex: `REQ-001` e
`REQ-005` — cadastro e login; `REQ-008` — relatórios integrados), aproximando a especificação textual da
experiência visual do usuário final antes da implementação.

---

## Conceitos de Engenharia de Software Presentes

* **Engenharia de Requisitos**: elicitação, especificação e classificação de requisitos funcionais e não funcionais;
* **Modelagem UML**: casos de uso com fluxos principais, alternativos e de exceção;
* **Metodologias Ágeis**: histórias de usuário e critérios de aceitação;
* **Prototipação**: protótipos de tela ligados a requisitos específicos;
* **Atributos de Qualidade de Software**: desempenho, segurança, escalabilidade, interoperabilidade, portabilidade e usabilidade;
* **Gestão de Stakeholders**: identificação de partes interessadas como insumo para o levantamento de requisitos.

## Conceitos de Gerência de Projetos Presentes

* **Definição de Escopo**: delimitação formal de escopo e não-escopo (fronteiras e exclusões), evitando
scope creep e desalinhamento de expectativa com a instituição adotante;
* **EAP e Cronograma**: decomposição do trabalho em fases e sua tradução em Gráfico de Gantt;
* **Gestão de Stakeholders**: mapeamento em camadas (equipe, instituição, usuários finais, governo/regulação,
partes indiretamente afetadas);
* **Matriz de Riscos**: identificação, análise qualitativa-quantitativa (Probabilidade × Impacto) e alocação de
40 riscos por papel/frente responsável, com plano de mitigação individualizado;
* **Alocação de Risco por Capacidade de Gestão**: adaptação do princípio normativo do art. 103 da Lei
14.133/2021 e das orientações do TCU sobre matriz de riscos, reinterpretado para um contexto de equipe sem
contraparte contratual;
* **Gestão de Equipe**: distribuição equilibrada de responsabilidade entre os quatro integrantes e mitigação de
riscos operacionais (concentração de conhecimento, dependência de colaboradores externos e voluntários).

---

## Licença
Este projeto está licenciado sob a Licença MIT. Veja o arquivo LICENSE para detalhes.
