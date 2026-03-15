---
date: 2026-03-15
title: Lançamento do SucupiraLAB e do pqLAB
categories:
  - lançamento
author_staff_member: ombudsmanviktor
---

**Lançamento público das versões 0.1$\beta$ do SucupiraLAB e do pqLAB**

![](images/hero.png)

O coLAB/UFF torna público o lançamento das versões 0.1$\beta$ duas ferramentas web de apoio à gestão e à organização da pesquisa acadêmica: o SucupiraLAB e o pqLAB, ambas desenvolvidas por Viktor Chagas com auxílio do Claude Code Sonnet v4.6 e disponibilizadas sob licença GPL-3.0.

O SucupiraLAB (v0.1$\beta$) é uma aplicação voltada a pesquisadores, docentes e coordenadores de programas de pós-graduação. Seu objetivo é centralizar as atividades de gestão acadêmica exigidas pela Plataforma Sucupira da CAPES, oferecendo módulos para prestação de contas, registro de discursos qualificados, cadastro de projetos financiados, acompanhamento de orientações, nucleação de egressos, catalogação da produção científica, internacionalização e monitoramento do fluxo de submissões de manuscritos em formato kanban. O sistema permite a geração de relatórios em PDF e a exportação de dados para planilhas, além de importar diretamente a produção acadêmica a partir do currículo Lattes salvo em HTML.

O pqLAB (v0.1$\beta$) é uma ferramenta destinada à organização de rotinas de pesquisa qualitativa. A aplicação reúne em uma única interface seis instrumentos de trabalho acadêmico — diário de campo, listas e memorandos, tarefas, favoritos, fichamentos e planos de trabalho —, conectados por links internos navegáveis. Um módulo de visualização em grafo *force-directed* gera automaticamente um mapa mental das conexões temáticas construídas pelo usuário ao longo do uso.

Ambas as aplicações compartilham a mesma arquitetura técnica: desenvolvidas em TypeScript com React 19, Vite 7, Tailwind CSS v4, React Router v7 e TanStack Query v5, com componentes baseados em shadcn/ui sobre primitivos Radix UI. A persistência de dados ocorre integralmente via GitHub Contents API, sem servidor ou banco de dados intermediário — os registros são armazenados em arquivos YAML em repositório GitHub privado de propriedade do próprio usuário. A autenticação pode ser realizada por Personal Access Token ou, opcionalmente, via Google OAuth com Firebase. A instalação de ambos os softwares é feita inteiramente pelo navegador, por meio de fork do repositório e ativação do GitHub Pages, sem necessidade de build local.

Os repositórios estão disponíveis publicamente em [github.com/ombudsmanviktor/sucupiralab](github.com/ombudsmanviktor/sucupiralab) e [github.com/ombudsmanviktor/pqlab](github.com/ombudsmanviktor/pqlab).
