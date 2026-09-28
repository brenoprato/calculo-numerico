# Documentation Index

This index maps every first-party source file to its maintained documentation.

## Core Documents

- [Atividade Prática III](atividade-3.md): mapa e instruções dos entregáveis acadêmicos de métodos numéricos.
- [`../resolucao.ipynb`](../resolucao.ipynb): notebook executável da resolução, com atalho para o Google Colab.
- [`../dashboard_mathcha.md`](../dashboard_mathcha.md): dashboard pronto para copiar e colar no Mathcha.
- [Architecture](architecture.md): system boundaries, runtime topology, and cross-cutting decisions.
- [Operations](operations.md): local development, validation, delivery, and recovery procedures.
- [Modules](modules/): ownership, file maps, interfaces, dependencies, and test coverage by code area.
- [Features](features/): user-visible behavior and feature-level technical decisions.
- [API](api/): contracts exposed by this repository.

## Coverage Rules

Every first-party source file must appear by exact repository-relative path in a module, feature, API, architecture, or operations document. Run `verify-doc-coverage` before declaring work complete.
