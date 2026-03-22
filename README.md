# Política de Privacidade — IALI Ticket App

**Última atualização:** 21 de março de 2026

---

## 1. Identificação do Responsável

O aplicativo **IALI Ticket App** (`com.iali.ticket_app`) é desenvolvido e operado por:

**Liga Digital Serviços LTDA**
CNPJ: 34.474.358/0001-78
Nome Fantasia: Liga Digital
Contato: contato@ligadigital.online

---

## 2. Sobre Este Aplicativo

O IALI Ticket App é um aplicativo de uso **interno e restrito**, destinado exclusivamente a operadores e funcionários habilitados da IALI e de grupos BNI. Sua finalidade é o gerenciamento de eventos e a realização de check-in de participantes via QR Code ou lista manual.

O acesso ao aplicativo é controlado por credenciais individuais e não está disponível para o público geral.

---

## 3. Dados Coletados e Finalidade

### 3.1 Dados do Operador (Usuário Logado)

| Dado | Finalidade |
|------|-----------|
| E-mail | Autenticação no sistema |
| Senha | Autenticação no sistema (não armazenada no dispositivo) |
| Nome e sobrenome | Exibição no perfil dentro do app |
| Tokens de acesso (JWT) | Manutenção da sessão autenticada |

Os tokens de autenticação são armazenados localmente no dispositivo utilizando armazenamento seguro (`flutter_secure_storage`), criptografado pelo sistema operacional. São automaticamente removidos no logout.

### 3.2 Dados de Participantes de Eventos

O app acessa, exibe e atualiza os seguintes dados de participantes de eventos, armazenados na plataforma BNI/IALI:

| Dado | Finalidade |
|------|-----------|
| Nome e sobrenome | Identificação do participante |
| Número de WhatsApp | Exibição para o operador |
| Especialidade profissional | Exibição para o operador |
| Status de presença/pagamento | Controle de check-in e situação do ingresso |

Esses dados **não são coletados pelo app** — são lidos da base de dados existente da IALI/BNI e utilizados exclusivamente para a operação de check-in. Nenhuma dessas informações é armazenada permanentemente no dispositivo.

### 3.3 Dados de Eventos

| Dado | Finalidade |
|------|-----------|
| Nome do grupo BNI | Exibição ao operador |
| Endereço do evento | Exibição ao operador |
| Data, hora e valor | Exibição ao operador |

Esses dados são mantidos em cache temporário no dispositivo por até **2 minutos** para desempenho e são apagados no logout.

### 3.4 Câmera (QR Code)

O app solicita permissão de acesso à **câmera** exclusivamente para leitura de QR Codes no formato `iali:<ID>`. Nenhuma imagem ou vídeo é capturado, gravado ou transmitido. O processamento é feito localmente, em tempo real.

### 3.5 Conectividade de Rede

O app realiza verificações periódicas de conectividade com a internet (ping para um servidor externo) com o único objetivo de exibir um aviso de conexão indisponível ao operador. Nenhum dado pessoal é transmitido nessas verificações.

---

## 4. Analytics — Microsoft Clarity

O app utiliza o **Microsoft Clarity** (ID do projeto: `vzg2bpgxfc`), ferramenta de análise de experiência de uso desenvolvida pela Microsoft Corporation.

O Clarity pode coletar:
- Gravações de sessão (telas acessadas, sequência de navegação)
- Interações de toque e navegação dentro do app
- Informações sobre o dispositivo e sistema operacional

Esses dados são utilizados exclusivamente pela equipe técnica da Liga Digital para **identificação e correção de bugs** e **análise de problemas de usabilidade**. O acesso é restrito ao departamento técnico responsável.

Para mais informações sobre como a Microsoft trata esses dados, consulte a [Política de Privacidade da Microsoft](https://privacy.microsoft.com/pt-br/privacystatement).

---

## 5. Base Legal para o Tratamento (LGPD)

O tratamento de dados pessoais realizado por este aplicativo fundamenta-se nas seguintes bases legais previstas na Lei Geral de Proteção de Dados (Lei nº 13.709/2018):

- **Execução de contrato** (Art. 7º, V): dados do operador são tratados para prestação do serviço contratado entre a Liga Digital e a IALI/BNI.
- **Legítimo interesse** (Art. 7º, IX): dados de participantes são acessados para a operação de check-in de eventos, atividade-fim do sistema.
- **Cumprimento de obrigação** (Art. 7º, II): manutenção de registros de presença conforme exigências operacionais da IALI/BNI.

---

## 6. Armazenamento e Retenção de Dados

- **No dispositivo:** tokens de sessão e cache de eventos são armazenados temporariamente e removidos no logout. Nenhum dado de participante é retido no dispositivo.
- **No servidor (`crm.bnibrasil.com.br`):** os dados de eventos e participantes são armazenados e gerenciados diretamente pela IALI/BNI pelo tempo necessário às suas operações.

A Liga Digital, na qualidade de operadora, não define o prazo de retenção dos dados armazenados no servidor da IALI/BNI.

---

## 7. Compartilhamento de Dados

Os dados tratados pelo app **não são vendidos, alugados ou compartilhados comercialmente** com terceiros.

O compartilhamento ocorre apenas:

| Destinatário | Motivo |
|-------------|--------|
| IALI / BNI (via API `crm.bnibrasil.com.br`) | Operação central do sistema de eventos |
| Microsoft Clarity | Analytics técnico para correção de bugs (uso interno restrito) |

---

## 8. Segurança

Adotamos medidas técnicas para proteção dos dados tratados pelo app:

- Tokens de autenticação armazenados em cofre seguro do sistema operacional (`flutter_secure_storage`)
- Toda comunicação com a API utiliza HTTPS (TLS)
- Tokens expiram automaticamente e são renovados de forma segura
- No logout, todos os dados locais são apagados integralmente

---

## 9. Público-Alvo

Este aplicativo é destinado exclusivamente a **operadores habilitados maiores de 18 anos**. Não é direcionado a crianças ou adolescentes. Caso um acesso indevido seja identificado, entre em contato pelo e-mail abaixo.

---

## 10. Direitos do Titular

Nos termos da LGPD, o titular dos dados pode, a qualquer momento, solicitar:

- Confirmação da existência de tratamento
- Acesso aos dados
- Correção de dados incompletos, inexatos ou desatualizados
- Eliminação dos dados tratados
- Informação sobre o compartilhamento realizado
- Revogação do consentimento (quando aplicável)

Para exercer esses direitos, entre em contato pelo e-mail:
**contato@ligadigital.online**

---

## 11. Alterações nesta Política

Esta política pode ser atualizada periodicamente. A data de "Última atualização" no topo deste documento indica quando a versão vigente foi publicada. Alterações relevantes serão comunicadas aos operadores antes de entrarem em vigor.

---

## 12. Contato

**Liga Digital Serviços LTDA**
contato@ligadigital.online
CNPJ: 34.474.358/0001-78
