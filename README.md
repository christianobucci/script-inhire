# InHire Autofill

Userscript para preenchimento automático de dados cadastrais em formulários de candidatura da **InHire**.

Preenche automaticamente informações previamente configuradas pelo próprio usuário.

> **Importante:** este projeto é uma ferramenta de preenchimento assistido. Perguntas específicas da vaga, revisão das informações e envio da candidatura continuam sob responsabilidade e controle do usuário.

## ✨ Funcionalidades

O script pode preencher automaticamente dados cadastrais como:

* Nome completo
* Nome e sobrenome
* CPF
* E-mail
* Telefone
* LinkedIn
* País
* Cidade
* Pretensão salarial

O preenchimento utiliza exclusivamente informações configuradas pelo próprio usuário no script.

## 🚫 O que este projeto não faz

Este projeto **não é um bot de candidaturas**.

Ele não foi desenvolvido para:

* buscar vagas automaticamente;
* realizar scraping de vagas;
* navegar automaticamente entre vagas;
* responder perguntas específicas de processos seletivos;
* gerar respostas para perguntas da candidatura;
* enviar candidaturas automaticamente;
* realizar candidaturas em massa;
* contornar CAPTCHA;
* contornar mecanismos de segurança ou proteção contra automação.

A decisão de se candidatar, as respostas específicas da vaga, a revisão dos dados e o envio permanecem manuais.

## 🔄 Como funciona

O fluxo é simples:

```text
Usuário acessa a candidatura
        ↓
Abre o formulário da InHire
        ↓
Userscript identifica os campos suportados
        ↓
Dados cadastrais são preenchidos
        ↓
Usuário responde perguntas específicas
        ↓
Usuário revisa as informações
        ↓
Usuário envia manualmente a candidatura
```

## 📦 Requisitos

Para utilizar o script você precisa de:

* navegador compatível com userscripts;
* extensão **Tampermonkey** ou equivalente;
* acesso ao formulário de candidatura da InHire.

## 🚀 Instalação

1. Instale o Tampermonkey para o seu navegador - https://www.tampermonkey.net/
2. Abra o painel do Tampermonkey.
3. Crie um novo userscript.
4. Copie o conteúdo do script deste repositório.
5. Cole no editor do Tampermonkey.
6. Configure seus dados pessoais.
7. Salve o script.
8. Acesse um formulário de candidatura compatível com inhire.

## ⚙️ Configuração

Antes de utilizar, altere o objeto `DATA` com suas próprias informações.

Exemplo:

```javascript
const DATA = {
  fullName: 'João da Silva',
  firstName: 'João',
  lastName: 'da Silva',
  cpf: '000.000.000-00',
  email: 'usuario@exemplo.com',
  phone: '11999999999',
  linkedin: 'https://www.linkedin.com/in/seu-usuario/',
  country: 'Brasil',
  city: 'São Paulo - SP',
  salaryExpectation: 'R$ 10.000,00',
};
```

**Nunca publique uma versão do script contendo seus dados pessoais reais.**

Caso mantenha seu próprio fork público, considere armazenar configurações pessoais separadamente do código versionado.

## 🔐 Privacidade

Os dados utilizados pelo autofill são definidos pelo próprio usuário.

O projeto não tem como objetivo coletar, armazenar ou transmitir informações pessoais para servidores externos.

Antes de utilizar uma versão modificada do script, revise o código para verificar como seus dados serão tratados.

## ⚠️ Disclaimer

Este é um projeto independente e não possui vínculo, associação, autorização ou endosso da InHire.

O projeto foi desenvolvido exclusivamente como ferramenta de preenchimento assistido de formulários.

O usuário é responsável pela utilização da ferramenta e pelo cumprimento dos termos de uso, políticas e regras das plataformas em que decidir utilizá-la.

Alterações realizadas por terceiros podem modificar o comportamento originalmente proposto pelo projeto.

## 🤝 Contribuições

Contribuições são bem-vindas, especialmente para:

* correções de compatibilidade;
* melhoria na identificação dos campos;
* tratamento de diferentes componentes de formulário;
* melhoria da experiência de configuração;
* documentação;
* correções de bugs.

Contribuições que transformem o projeto em ferramenta de candidatura automática, scraping, submissão em massa ou contorno de mecanismos de segurança não fazem parte do escopo proposto.

## 📄 Licença

Este projeto é disponibilizado sob a **MIT License**.

Consulte o arquivo `LICENSE` para mais informações.

---

### Objetivo do projeto

Automatizar a digitação repetitiva, **não a decisão de candidatura**.
