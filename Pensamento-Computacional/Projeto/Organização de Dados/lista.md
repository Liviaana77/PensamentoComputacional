# Guia de Modelagem: Plataforma Inteligente de Disponibilidade de Medicamentos

## 1. LISTA

A lista representa os componentes do sistema em sequência lógica, mostrando as principais funcionalidades da plataforma.

### Componentes do Sistema

1. Cadastro de Usuários
2. Consulta de Medicamentos
3. Gestão de Estoque
4. Notificações
5. Relatórios
6. Recomendações com IA
7. Integração com SUS

---

### Características Visuais

- Caixas verticais organizadas;
- Numeração sequencial;
- Ícones representando cada módulo;
- Utilização das cores:
  - Verde → UBS;
  - Azul → Farmácia Popular.

---

# 2. HIERARQUIA

A hierarquia representa a estrutura organizacional do sistema e a divisão dos módulos.

## Estrutura Hierárquica

```text
Plataforma Inteligente
│
├── Usuários
│   ├── Cadastro
│   ├── Login
│   └── Permissões
│
├── Consulta
│   ├── Medicamentos
│   ├── UBS
│   └── Farmácia Popular
│
├── Gestão
│   ├── Estoque
│   ├── Atualização
│   └── Histórico
│
├── Notificações
├── Relatórios
└── IA
