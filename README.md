# O GUIA COMPLETO DOS CHK

**Autor:** [@pugno_dev](https://t.me/pugno_dev) | **GitHub:** [Pugn0](https://github.com/Pugn0)

---

## 📚 Sobre este Guia

Este repositório contém um **guia técnico e conceitual completo** sobre o processo de verificação automatizada de cartões de crédito através de diferentes plataformas. 

O conteúdo é apresentado em **nível técnico e conceitual**, sem instruções de uso prático, focando na compreensão de como funciona a simulação de transações em diferentes contextos para interpretar mensagens de erro dos gateways de pagamento e classificar o estado dos cartões.

> **Importante:** Este guia é puramente técnico e educativo. As técnicas descritas violam termos de uso de gateways, podem disparar sistemas antifraude e têm implicações legais e éticas significativas.

---

## 📖 Índice de Conteúdos

### 1️⃣ [E-commerce](01%20-%20ecommerce.md)

**Título:** *Verificação de Cartões via Plataformas de E-commerce*

Descreve o processo completo de simulação de checkout em lojas online para testar cartões. Aborda o fluxo de carrinho, seleção de frete, interação com gateway e interpretação de respostas para classificação de cartões.

**Conceitos-chave:** Checkout automatizado, tokenização, análise de mensagens de erro, carrinho de compras.

---

### 2️⃣ [Doação](02%20-%20doacao.md)

**Título:** *Verificação de Cartões via Plataformas de Doação*

Explica como plataformas de doação (crowdfunding, ONGs, campanhas) são utilizadas para verificação de cartões. Aborda formulários simplificados, valores mínimos menores e menos validações antifraude comparadas ao e-commerce.

**Conceitos-chave:** Formulários simplificados, valores mínimos, doação recorrente, menos validações.

---

### 3️⃣ [Assinatura](03%20-%20assinatura.md)

**Título:** *Verificação de Cartões via Plataformas de Assinatura*

Detalha o processo de verificação através de assinaturas recorrentes (streaming, SaaS, serviços digitais). Foca em pre-authorization, trials gratuitos e verificação de recorrência sem cobrança imediata.

**Conceitos-chave:** Pre-authorization, trial gratuito, verificação de recorrência, cancelamento imediato.

---

## 🔗 Conexões entre os Módulos

Todos os três métodos seguem uma **estrutura base comum**:

1. **Recebimento de dados do cartão** (número, validade, CVV)
2. **Geração de identidade falsa** (nome, email, endereço)
3. **Consulta BIN** (HiPay ou similar para extrair informações do cartão)
4. **Simulação do fluxo real** da plataforma específica
5. **Interação com gateway de pagamento**
6. **Análise e interpretação das respostas** do gateway para classificação

### Diferenças Principais:

| Característica | E-commerce | Doação | Assinatura |
|----------------|------------|--------|------------|
| **Complexidade do formulário** | Alta (múltiplas etapas) | Baixa (simplificado) | Média (planos/valores) |
| **Valor mínimo** | Variado | Geralmente menor | Variado (trial comum) |
| **Cobrança imediata** | Geralmente sim | Geralmente sim | Muitas vezes não (pre-auth) |
| **Validações antifraude** | Rigorosas | Menos rigorosas | Variadas |
| **Vantagem principal** | Fluxo completo | Simplicidade | Verificação sem cobrança |

---

## 🌐 Outras Formas de Verificação

Embora este guia cubra os **três métodos principais** (E-commerce, Doação e Assinatura), existem **várias outras plataformas e contextos** onde técnicas similares são aplicadas:

### 🎮 Jogos e Gaming
- Compras in-game
- Créditos virtuais
- Gift cards de jogos

### 🎁 Gift Cards e Prepaid
- Compra de gift cards digitais
- Validação através de plataformas de prepaid

### 💰 Criptomoedas
- Compra de criptomoedas com cartão
- Exchanges que aceitam cartão

### 💸 Transferências P2P e Remessas
- Plataformas de envio de dinheiro
- Serviços de remessa internacional

### ☁️ Hospedagem e Hosting
- Contratação de VPS
- Serviços de cloud computing
- Domínios e serviços web

### 🛒 Marketplaces
- Amazon, eBay e similares
- Plataformas de terceiros

### 🔌 Créditos de API e Serviços
- Compra de créditos para APIs
- Serviços de dados e ferramentas

### 📱 Aplicativos Mobile
- Compras in-app (iOS/Android)
- Créditos de aplicativos

### 🔒 VPN e Serviços de Segurança
- Assinaturas de VPN
- Serviços de segurança digital

### 🎓 Cursos Online e Educação
- Plataformas de ensino
- Cursos digitais e certificações

### 📺 Streaming e Entretenimento
- Plataformas de conteúdo
- Serviços de entretenimento

Cada uma dessas plataformas tem características específicas, gateways diferentes e validações próprias, mas todas seguem princípios similares de simulação de transação e interpretação de respostas do gateway.

---

## ⚠️ Aviso Legal e Ético

Do ponto de vista **legal e de segurança**, essas técnicas:

- ❌ Violam termos de uso de gateways
- ❌ Disparam sistemas antifraude
- ❌ Podem causar bloqueio de IP, domínio e conta
- ❌ Têm implicações legais significativas
- ❌ Podem gerar chargebacks e problemas financeiros

**Este conteúdo é apresentado apenas para fins educacionais e de compreensão técnica.**

---

## 👤 Créditos

**Desenvolvido por:**

- **Telegram:** [@pugno_dev](https://t.me/pugno_dev)
- **GitHub:** [Pugn0](https://github.com/Pugn0)

---

## 📝 Licença

Este guia é fornecido "como está", apenas para fins educacionais e de pesquisa técnica.

---

*Última atualização: 2025*
