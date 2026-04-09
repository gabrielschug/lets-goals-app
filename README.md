# 🎯 LetsGoals

> "Cofrinho Digital" para amigos e famílias organizarem, acompanharem e alcançarem objetivos financeiros em conjunto.

![Status](https://img.shields.io/badge/Status-Em_Desenvolvimento-yellow)
![React](https://img.shields.io/badge/React-19.0-blue)
![Tailwind](https://img.shields.io/badge/Tailwind_CSS-4.0-38B2AC)
![Mobile First](https://img.shields.io/badge/Design-Mobile_First-purple)

## 🚀 Sobre o Projeto

O **LetsGoals** tem como objetivo resolver o problema da organização financeira em grupo (viagens de amigos, presentes coletivos, eventos). 
Em vez de planilhas confusas, o sistema oferece uma interface clara onde um líder cria uma meta, convida os participantes através de um código único, e todos registram suas contribuições de forma transparente.

### 📚 Projeto Acadêmico
Este projeto foi desenvolvido para **Avaliação Final do 2º semestre** do curso de Análise e Desenvolvimento de Sistemas (Senac/Unisenac), integrando as disciplinas de *Programação Web* e *Desenvolvimento Web para Dispositivos Móveis*. 

O objetivo principal foi aplicar na prática os fundamentos de consumo de APIs, ciclo de requisição/resposta, gerenciamento de estado e design responsivo.

---

## 📱 Mobile-First & UI/UX

Idealizado para ser um aplicativo, a interface, navegação e disposição de elementos (utilizando CSS Grid Layout e Flexbox via Tailwind) foram elaboradas para a proporção e usabilidade de dispositivos móveis.

---

## 🏗️ Arquitetura do Sistema

Para manter um fluxo ágil de desenvolvimento e separar as responsabilidades, o projeto foi estruturado deste modo:

* **Front-End React + Mock API**
  Toda a interface do usuário, rotas (`react-router`) e controle de requisições foram construídos. Aplicamos conceitos-chave exigidos na arquitetura Web:
  * **Processamento de Formulários:** Validação robusta utilizando `react-hook-form`.
  * **Web Storage API:** Utilização do `localStorage` para manter a persistência da sessão do usuário autenticado (Context API).
  * **Integração com Web Services:** Consumo de uma API simulada (`json-server`) realizando operações assíncronas (CRUD) com o método `fetch`.

---

## 💻 Funcionalidades Principais (RFs)

- [x] **Gestão de Usuários:** Cadastro, Login e edição de perfil.
- [x] **Criação de Metas:** Definição de título, valor-alvo e prazos.
- [x] **Convites:** Sistema de adesão à meta via código gerado dinamicamente.
- [x] **Dashboard (Home):** Visão geral das metas ativas do usuário.
- [x] **Gestão de Contribuições:** Participantes podem registrar aportes financeiros, atualizando o saldo geral da meta.
- [x] **Detalhes da Meta:** Extrato transparente de quem contribuiu, quando e com qual valor.

---

## ⚙️ Como rodar o projeto localmente

Para testar o LetsGoals na sua máquina, você precisará de dois terminais abertos simultaneamente (um para o Front-End e outro para a API simulada). 
*Para a melhor experiência visual, utilize o modo "Inspecionar" do navegador simulando a tela de um celular.*

**1. Clone o repositório e instale as dependências:**
```bash
git clone [https://github.com/gabrielschug/letsgoals.git](https://github.com/gabrielschug/letsgoals.git)
cd letsgoals
npm install
```

**2. No primeiro terminal, inicie a Mock API (Banco de Dados):**
```
# Isso fará o json-server rodar na porta 3000
npx json-server --watch db.json --port 3000
```

**3. No segundo terminal, inicie o Front-End React:**
```
npm run dev
```

Acesse a aplicação no seu navegador através do link gerado pelo Vite (geralmente `http://localhost:5173`).

---

## 🤝 Desenvolvedores

Projeto desenvolvido em colaboração por:

- **Gabriel Schug**
- **Joaquim Pedro**
