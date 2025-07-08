# 🛡️ SafeEPI - Plataforma Inteligente de Gestão de EPIs

<div align="center">

![SafeEPI Logo](https://img.shields.io/badge/SafeEPI-Sistema%20Inteligente-blue?style=for-the-badge&logo=shield&logoColor=white)

**Desenvolvido pela Barcelos Engenharia de Segurança**

*Revolucionando a gestão de Equipamentos de Proteção Individual com tecnologia biométrica e inteligência de dados*

[![Node.js](https://img.shields.io/badge/Node.js-18+-green?style=flat-square)](https://nodejs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.8+-blue?style=flat-square)](https://www.typescriptlang.org/)
[![Prisma](https://img.shields.io/badge/Prisma-6.7+-purple?style=flat-square)](https://www.prisma.io/)
[![Docker](https://img.shields.io/badge/Docker-Ready-blue?style=flat-square)](https://www.docker.com/)
[![NBIS](https://img.shields.io/badge/NBIS-Biometric%20Engine-red?style=flat-square)](https://www.nist.gov/services-resources/software/nist-biometric-image-software-nbis)

</div>

---

## 🎯 **Visão Geral**

O **SafeEPI** é uma plataforma de gestão inteligente que combina **autenticação biométrica de alta precisão** com **análise avançada de dados** para revolucionar o controle e distribuição de Equipamentos de Proteção Individual (EPIs) em ambientes corporativos.

### 🔥 **Diferenciais Tecnológicos**

- **🔐 Autenticação Biométrica NBIS**: Utiliza os algoritmos do NIST (National Institute of Standards and Technology) para matching de impressões digitais com precisão militar
- **📊 Business Intelligence Integrado**: Dashboards em tempo real com insights financeiros e operacionais
- **🏗️ Arquitetura Enterprise**: API REST robusta com TypeScript, Prisma ORM e containerização Docker
- **⚡ Performance Otimizada**: Processamento biométrico otimizado para alta concorrência
- **🛡️ Segurança Corporativa**: Rate limiting, autenticação por API Key e logs auditáveis

---

## 🏢 **Módulos da Plataforma**

### 1. **👥 Gestão Multi-Tenant**
- **Empresas**: Cadastro e gerenciamento de múltiplas organizações
- **Colaboradores**: Controle completo do quadro de funcionários
- **Usuários & Permissões**: Sistema de roles e autorizações granulares

### 2. **🦺 Controle de EPIs**
- **Catálogo Inteligente**: Gestão de EPIs com CA, validades e especificações técnicas
- **Estoque Dinâmico**: Controle de quantidades, alertas de reposição e vida útil
- **Rastreabilidade Total**: Histórico completo de movimentações e custos

### 3. **🔄 Processos de Entrega**
- **Agendamento Inteligente**: Sistema de agendamento com notificações
- **Confirmação Biométrica**: Entrega confirmada via matching de impressões digitais
- **Gestão de Devoluções**: Controle de EPIs devolvidos e substituições

### 4. **🧬 Sistema Biométrico Avançado**
- **Cadastro Multi-Dedo**: Suporte para polegar e indicador com fallback inteligente
- **Algoritmos NBIS**: mindtct, bozorth3 e cwsq para máxima precisão
- **WSQ Processing**: Processamento nativo de arquivos WSQ com validação robusta
- **Matching Inteligente**: Sistema de scores com threshold adaptivo

### 5. **📈 Business Intelligence**
- **Dashboards Executivos**: Métricas de entregas, custos e performance
- **Relatórios Financeiros**: Análise de custos por período, EPI e colaborador
- **Indicadores de Segurança**: Estatísticas de compliance e uso de EPIs
- **Alertas Inteligentes**: Notificações sobre validades, estoques e custos

---

## 🛠️ **Stack Tecnológica**

### **Backend (API Core)**
```typescript
// Tecnologias Principais
- Node.js 18+ com TypeScript 5.8+
- Express.js com middlewares avançados
- Prisma ORM com MySQL
- Zod para validação de dados
- JWT + API Key para autenticação
- Pino para logging estruturado
- Rate Limiting com rate-limiter-flexible
```

### **Processamento Biométrico**
```bash
# NBIS Tools (Linux Binaries)
- mindtct: Extração de minutiae de imagens WSQ
- bozorth3: Matching entre templates biométricos  
- cwsq: Compressão/descompressão WSQ

# Formatos Suportados
- WSQ (Wavelet Scalar Quantization)
- XYT (Minutiae Templates)
```

### **Infraestrutura**
```yaml
# Container & Deploy
- Docker com multi-stage builds
- MySQL 8.0 com otimizações
- CORS configurado para multi-origin
- Swagger/OpenAPI para documentação
- Hot reload para desenvolvimento
```

---

## 🚀 **Recursos Avançados**

### **🔍 Sistema de Diagnóstico**
- Monitoramento de saúde das ferramentas NBIS
- Análise de qualidade de impressões digitais
- Métricas de performance do sistema biométrico
- Logs detalhados para troubleshooting

### **📊 Analytics Financeiros**
- Custos anuais por EPI e categoria
- Análise de ROI em segurança
- Previsões de gastos e reposições
- Comparativos históricos

### **🔐 Segurança Enterprise**
- Autenticação multi-camada (API Key + JWT)
- Rate limiting por IP e usuário
- Logs auditáveis de todas as operações
- Sanitização e validação de dados

### **⚡ Performance**
- Conexão pool otimizada do Prisma
- Cache de templates biométricos
- Processamento assíncrono de arquivos WSQ
- Cleanup automático de arquivos temporários

---

## 📋 **Fluxos Operacionais**

### **1. Cadastro de Colaborador**
```mermaid
graph LR
    A[Cadastro Básico] --> B[Upload Biometria]
    B --> C[Processamento WSQ]
    C --> D[Extração Minutiae]
    D --> E[Validação NBIS]
    E --> F[Armazenamento Seguro]
```

### **2. Processo de Entrega**
```mermaid
graph LR
    A[Agendamento] --> B[Preparação EPIs]
    B --> C[Verificação Biométrica]
    C --> D[Confirmação Entrega]
    D --> E[Movimentação Financeira]
    E --> F[Relatórios]
```

---

## 📈 **Casos de Uso Reais**

### **🏗️ Construtoras**
- Controle de EPIs por obra e função
- Compliance com NRs (Normas Regulamentadoras)
- Redução de perdas e extravios

### **🏭 Indústrias**
- Gestão de EPIs específicos por setor
- Rastreabilidade para auditorias
- Otimização de custos operacionais

### **🚧 Empresas de Segurança**
- Distribuição controlada de equipamentos
- Histórico completo para seguradoras
- Relatórios para certificações ISO

---

## 💡 **Potencial de Expansão**

### **Integrações Futuras**
- **ERP/SAP**: Sincronização com sistemas corporativos
- **IoT Sensors**: Monitoramento do uso real dos EPIs
- **Mobile App**: Aplicativo para colaboradores
- **BI Tools**: Integração com Power BI, Tableau
- **Blockchain**: Imutabilidade de registros

### **Funcionalidades Avançadas**
- **IA Preditiva**: Previsão de necessidades de EPIs
- **Computer Vision**: Detecção automática de uso
- **APIs Terceiros**: Integração com fornecedores
- **Multi-Biometria**: Facial, íris, voz
- **Geolocalização**: Controle por localização

---

## 🏆 **Benefícios Mensuráveis**

### **💰 Financeiros**
- **Redução de 30-50%** nos custos com EPIs
- **Eliminação de perdas** por extravio
- **Otimização de estoques** com dados precisos

### **🛡️ Segurança & Compliance**
- **100% de rastreabilidade** nas entregas
- **Conformidade total** com NRs e auditorias
- **Redução de acidentes** por uso inadequado

### **📊 Operacionais**
- **Automatização** de processos manuais
- **Relatórios em tempo real** para tomada de decisão
- **Eficiência operacional** comprovada

---

## 🔧 **Arquitetura da Solução**

```
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│   Frontend      │    │   API Gateway   │    │   Database      │
│   Dashboard     │◄──►│   Express.js    │◄──►│   MySQL         │
│   React/Vue     │    │   + Middlewares │    │   + Prisma      │
└─────────────────┘    └─────────────────┘    └─────────────────┘
                                │
                       ┌─────────────────┐
                       │   NBIS Engine   │
                       │   Biometric     │
                       │   Processing    │
                       └─────────────────┘
```

---

## 🌟 **Por que SafeEPI?**

A **SafeEPI** não é apenas um sistema de gestão de EPIs - é uma **plataforma de transformação digital** que eleva o padrão de segurança ocupacional através da tecnologia. Com biometria de grau militar, análise inteligente de dados e arquitetura enterprise, oferecemos uma solução completa para empresas que levam a sério a segurança de seus colaboradores.

---

<div align="center">

### 🚀 **Pronto para Revolucionar sua Gestão de EPIs?**

**Developed with ❤️ by Barcelos Engenharia de Segurança**

*Transformando segurança ocupacional através da tecnologia*

</div>

---

## 📞 **Contato**

Para mais informações sobre implementação, customizações ou parcerias:

- **Email**: contato@barcelosengenharia.com.br
- **Website**: www.barcelosengenharia.com.br
- **LinkedIn**: /company/barcelos-engenharia

---

*© 2025 Barcelos Engenharia de Segurança. Todos os direitos reservados.*
