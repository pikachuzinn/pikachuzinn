<h1 align="center">Henan Heiiji Shirahige</h1>

<p align="center">
  <strong>Backend &amp; Automação Inteligente</strong><br>
  APIs REST, integração de sistemas e agentes de IA aplicados a processos reais de negócio.
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/henan-heiiji-shirahige-745467350/">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
  </a>
  <a href="mailto:henanshirahige@gmail.com">
    <img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email">
  </a>
  <img src="https://img.shields.io/badge/Londrina,%20PR%20—%20Brasil-2F855A?style=for-the-badge" alt="Localização">
</p>

---

### Sobre

Estudante de **Engenharia de Software** na UniFil (Londrina/PR), com formação técnica em Eletroeletrônica e passagem como estagiário de TI em telecomunicações — foi lá que comecei a construir automações para o próprio time.

Meu foco é **backend, automação inteligente e integração de sistemas**: transformar processos manuais e repetitivos em fluxos automatizados e confiáveis, usando APIs REST, webhooks, orquestração com N8N e agentes de IA.

- Construindo pipelines que unem **Python + LLMs + N8N** para automação de processos ponta a ponta
- Trabalhando com **Java 21 / Spring Boot** e modelagem de domínio orientada a objetos
- Estudando **Cloud AWS** — Lambda, ECS e Bedrock
- Aberto a oportunidades de **estágio e júnior** em backend, automação e agentes de IA

---

### Stack

**Linguagens**

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white" alt="Java">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" alt="JavaScript">
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white" alt="TypeScript">
  <img src="https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white" alt="SQL">
</p>

**Backend &amp; Automação**

<p>
  <img src="https://img.shields.io/badge/Node.js-5FA04E?style=flat-square&logo=nodedotjs&logoColor=white" alt="Node.js">
  <img src="https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white" alt="Express">
  <img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white" alt="Spring Boot">
  <img src="https://img.shields.io/badge/n8n-EA4B71?style=flat-square&logo=n8n&logoColor=white" alt="n8n">
  <img src="https://img.shields.io/badge/REST%20APIs-005571?style=flat-square&logo=fastapi&logoColor=white" alt="REST APIs">
  <img src="https://img.shields.io/badge/AI%20Agents-412991?style=flat-square&logo=openai&logoColor=white" alt="AI Agents">
</p>

**Dados &amp; Infra**

<p>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL">
  <img src="https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white" alt="MongoDB">
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" alt="Redis">
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker">
  <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" alt="Git">
  <img src="https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white" alt="AWS">
</p>

---

### Projetos em destaque

**[E-commerce Orders API](https://github.com/pikachuzinn/ecommerce-api)** — `Java 21` `Spring Boot 4` `PostgreSQL` `Flyway` `Testcontainers`

API REST de catálogo e pedidos construída em torno das regras que um e-commerce precisa acertar, e não em torno do CRUD: reserva de estoque sob concorrência com lock pessimista e `@Version`, preço congelado no momento da compra, máquina de estados do pedido sem `if` espalhado, e autorização por papel **e** por dono do recurso. O valor cobrado é sempre calculado no servidor, nunca enviado pelo cliente. Schema versionado com Flyway e `ddl-auto: validate`, testes de integração contra PostgreSQL real via Testcontainers, JWT stateless, OpenAPI e CI no GitHub Actions.

**[NotaFlow](https://github.com/pikachuzinn/notaflow)** — `Python` `LLM` `PostgreSQL` `Docker` `Google Drive`

Extração de dados de notas fiscais brasileiras com LLM, em produção de ponta a ponta: ingestão por Google Drive ou pasta local atrás de uma mesma interface, extração com *tool use*, validação Pydantic **antes** de gravar e retentativa corretiva que devolve o erro ao modelo — com teto separado para falha de leitura da chave de acesso. Documento reprovado vai para revisão manual com aviso por e-mail em vez de entrar sujo no banco. Idempotência, migrations versionadas, base sintética para medir o acerto da extração, testes e CI.

**[Radar de Provedores](https://github.com/pikachuzinn/radar-provedores)** — `Python` `Google Places API` `tkinter` `pytest`

Ferramenta de análise de viabilidade que mapeia provedores de internet numa região via Google Places API, com interface gráfica e CLI. Mede a sobreposição entre os termos de busca e recomenda, por cobertura, o menor conjunto que reproduz o mesmo resultado — calibrado em várias cidades para não generalizar a partir de uma só. Cache local, deduplicação por `place_id`, exportação CSV/Excel e filtro de log que mascara a chave de API. 231 testes, nenhum deles usando rede ou chave real.

**[Dragon Ball Z API](https://github.com/pikachuzinn/trabalho-api-full)** — `Node.js` `Express` `SQLite` `JWT` `Jest`

API REST completa com autenticação JWT, CRUD de três entidades relacionadas, filtros, paginação e ordenação. Inclui suíte de testes automatizados (Jest + Supertest), tratamento global de erros, collection Postman e configuração de deploy.

**[Desafio Brasilis](https://github.com/pikachuzinn/Brasilis)** — `Godot 4` `GDScript` `Playwright`

Quiz educativo sobre cultura, história e geografia do Brasil, desenvolvido como Projeto de Extensão da UniFil. Estado centralizado em singleton, persistência local e duas suítes de testes headless — incluindo validação de clique real no viewport e playthrough automatizado do build web.

---

### Contato

Aberto a conversas sobre **estágio, vagas júnior e projetos de automação**.

- **Email:** henanshirahige@gmail.com
- **LinkedIn:** [henan-heiiji-shirahige](https://www.linkedin.com/in/henan-heiiji-shirahige-745467350/)
