# Ambiente de Simulação DREX

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Solidity](https://img.shields.io/badge/Solidity-%5E0.8.0-blue)
![Foundry](https://img.shields.io/badge/Framework-Foundry-orange)

Este projeto é um ambiente de simulação para a plataforma **DREX**, o Real Digital do Banco Central do Brasil. O objetivo é recriar e testar as funcionalidades-chave da arquitetura do DREX em um ambiente de desenvolvimento blockchain local, utilizando o framework **Foundry**.

## 🚀 Sobre o Projeto

A simulação implementa uma arquitetura de múltiplos Smart Contracts para representar as diferentes entidades e ativos do ecossistema DREX, permitindo a interação entre eles de forma segura e automatizada.

### ✨ Funcionalidades Principais

* **Arquitetura de Múltiplos Contratos:** Representação de entidades como Banco Central, Bancos Comerciais e Clientes.
* **Emissão de Ativos Digitais:** Funcionalidades para a criação (mint) de Real Digital (RD) e Real Tokenizado (RT).
* **Transferências Seguras:** Mecanismos para a transferência de saldos de RD e RT entre as diferentes carteiras.
* **Funcionalidade de SWAP:** Implementação de um sistema de troca atômica (swap) entre diferentes tipos de ativos dentro do ecossistema simulado.
* **Testes Abrangentes:** Cobertura de testes unitários e de integração para garantir a segurança e o correto funcionamento dos contratos.
* **Automação:** Scripts para deploy e interação com os contratos, facilitando a simulação de operações.

## 🛠️ Tecnologias Utilizadas

Este projeto foi construído com as seguintes tecnologias e ferramentas do ecossistema Web3:

* **[Solidity](https://soliditylang.org/):** Linguagem principal para a escrita dos Smart Contracts.
* **[Foundry](https://getfoundry.sh/):** Framework moderno para desenvolvimento, teste e deploy de contratos, utilizando as ferramentas `forge` e `cast`.
* **[Git](https://git-scm.com/):** Para versionamento de código.
* **[GitHub Actions](https://github.com/features/actions):** Para automação de workflows e CI/CD.

## 📂 Estrutura do Projeto

O repositório está organizado da seguinte forma:

```
.
├── .github/workflows   # Arquivos de CI/CD com GitHub Actions
├── lib                 # Dependências e bibliotecas (via forge)
├── script              # Scripts para deploy e interação com os contratos
├── src                 # Código-fonte dos Smart Contracts em Solidity
├── test                # Testes para os contratos
└── foundry.toml        # Arquivo de configuração do Foundry
```

## 🚀 Como Executar o Projeto

Para clonar e executar este projeto localmente, você precisará ter o [Foundry](https://getfoundry.sh/) instalado.

**1. Clone o repositório:**
```bash
git clone [https://github.com/CiceroGGS/ambiente-drex-simulado.git](https://github.com/CiceroGGS/ambiente-drex-simulado.git)
cd ambiente-drex-simulado
```

**2. Instale as dependências:**
```bash
forge install
```

**3. Compile os contratos:**
```bash
forge build
```

**4. Execute os testes:**
```bash
forge test
```

**5. Execute um script (exemplo):**
```bash
forge script script/SeuScript.s.sol --rpc-url <sua_url_rpc> --broadcast
```

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.
