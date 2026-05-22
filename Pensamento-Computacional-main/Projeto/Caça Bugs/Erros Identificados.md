# Erros Identificados

## Projeto: Plataforma Inteligente de Disponibilidade de Medicamentos

---

# 1. Problemas de Lógica

## Erro 1 — Fluxo sem validação de login

O fluxograma apresenta o login do usuário, porém não existe uma validação para verificar se o e-mail e a senha estão corretos.

### Impacto
O sistema pode permitir acessos indevidos ou gerar falhas na autenticação.

### Correção
Adicionar uma decisão após o login:
- Se os dados estiverem corretos → continuar.
- Caso contrário → exibir mensagem de erro.

---

## Erro 2 — Ausência de tratamento para medicamento indisponível

O fluxo apenas verifica unidades com medicamentos disponíveis, mas não informa o que acontece quando nenhuma unidade possui o medicamento.

### Impacto
O usuário pode ficar sem resposta clara.

### Correção
Adicionar:
- Mensagem “Medicamento indisponível”.
- Opção de ativar notificação automática.

---

# 2. Problemas de Execução

## Erro 3 — Dependência da localização

O sistema exige acesso à localização, porém não trata o caso de permissão negada.

### Impacto
A busca por unidades próximas pode falhar.

### Correção
Permitir:
- Digitação manual da cidade/bairro.
- Continuação parcial do sistema sem GPS.

---

## Erro 4 — Atualização de estoque em tempo real

O sistema depende da atualização das UBS e Farmácias Populares.

### Impacto
Informações podem ficar desatualizadas.

### Correção
Implementar:
- Atualizações periódicas.
- Sincronização automática com banco de dados.

---

# 3. Problemas de Escalabilidade

## Erro 5 — Alto número de consultas simultâneas

Muitos usuários acessando ao mesmo tempo podem causar lentidão.

### Impacto
Queda de desempenho do sistema.

### Correção
Utilizar:
- Banco de dados otimizado.
- Cache de consultas.
- APIs escaláveis.

---

# 4. Problemas de Segurança

## Erro 6 — Risco relacionado à LGPD

O sistema trabalha com dados pessoais e localização.

### Impacto
Possível vazamento de dados sensíveis.

### Correção
Aplicar:
- Criptografia.
- Autenticação segura.
- Controle de permissões.
- Consentimento do usuário.

---
