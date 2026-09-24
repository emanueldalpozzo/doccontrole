# DocControle

Sistema web para criação, gerenciamento e edição colaborativa de relatórios avaliativos, com foco nos relatórios exigidos pela Comissão Própria de Avaliação (CPA) do MEC.

## Motivação

A elaboração de relatórios institucionais costuma envolver diversos colaboradores e setores, cada um responsável por partes diferentes do documento. Quando esse processo é feito em arquivos separados, sem uma estrutura centralizada, surgem problemas recorrentes: falta de padronização entre as seções, conflitos de versão quando duas pessoas editam a mesma parte, perda de conteúdo e longas etapas de revisão manual para consolidar tudo num único documento final.

No caso específico dos relatórios da CPA/MEC, esse problema é ainda mais crítico: o instrumento de avaliação institucional precisa seguir rigorosamente uma estrutura pré-definida, e qualquer desalinhamento pode comprometer o processo avaliativo. O DocControle nasce para resolver esse problema, oferecendo uma plataforma única onde a estrutura do relatório é definida previamente e as contribuições de cada colaborador são organizadas, rastreadas e consolidadas automaticamente.

## Objetivo geral

Desenvolver um sistema web que apoie comissões na criação, gestão e edição colaborativa de relatórios de avaliação institucional (CPA/MEC), garantindo a padronização estrutural do documento e o controle de concorrência entre os usuários.

## Objetivos específicos

- Autenticação e controle de permissões via API, para gerenciar o acesso dos usuários às diferentes seções do relatório.
- Importação e interpretação de uma estrutura de avaliação em CSV, gerando as seções do documento conforme as diretrizes da CPA.
- Controle de concorrência e acompanhamento de edições em tempo real, com indicadores visuais (ex.: cores) e registro de atividades (logs) para organizar o trabalho colaborativo.
- Geração de relatório consolidado, exportado em PDF na formatação estrutural exigida pelo MEC.
- Validação da solução por meio de testes de software, verificando a mitigação de conflitos de versão e a padronização do documento final.

## Funcionalidades planejadas

- [ ] Autenticação e permissões por papel (ex.: administrador, colaborador, revisor)
- [ ] Importação de estrutura CSV da CPA e geração automática das seções do relatório
- [ ] Editor colaborativo de seções com indicadores visuais de quem está editando
- [ ] Log de atividades por seção/documento
- [ ] Exportação do relatório consolidado em PDF, na formatação exigida pelo MEC
- [ ] Testes automatizados cobrindo autenticação, importação, concorrência e exportação

## Arquitetura

Monorepo com front-end e back-end desacoplados:

- [`/backend`](backend) — API Laravel (PHP 8.5, SQLite), autenticação via Laravel Sanctum.
- [`/frontend`](frontend) — Next.js + React + TypeScript + Tailwind CSS, consumindo a API do back-end.
- `/docs` — artefatos de planejamento técnico do projeto (requisitos, modelagem de dados, wireframes, planejamento de sprints) — a serem adicionados em etapa futura.

## Status

Projeto em desenvolvimento como Trabalho de Conclusão de Curso / Prática de Implementação. Este repositório é evoluído ao longo do semestre até o Checkpoint Final.
