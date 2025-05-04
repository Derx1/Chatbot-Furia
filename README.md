# FuriaBot: Assistente Virtual para Fãs da Furia FC

<div align="center">
  <img src="https://via.placeholder.com/200x200" alt="Logo do FuriaBot" width="200">
  <br>
  <strong>Seu assistente virtual para acompanhar a Furia FC na Kings League Brasil</strong>
</div>

## 📋 Índice

- [Sobre o Projeto](#-sobre-o-projeto)
- [Funcionalidades](#-funcionalidades)
- [Tecnologias Utilizadas](#-tecnologias-utilizadas)
- [Estrutura de Dados](#-estrutura-de-dados)
- [Instalação e Configuração](#-instalação-e-configuração)
- [Como Usar](#-como-usar)
- [Exemplos de Interação](#-exemplos-de-interação)
- [Próximos Passos](#-próximos-passos)
- [Contribuição](#-contribuição)
- [Licença](#-licença)

## 🚀 Sobre o Projeto

O FuriaBot é um assistente virtual desenvolvido para fornecer informações detalhadas sobre a equipe Furia FC na Kings League Brasil. Com foco na temporada de março e abril de 2025, o chatbot permite que torcedores acessem estatísticas de jogos, informações sobre jogadores, resultados de partidas e muito mais, tudo em um formato conversacional intuitivo.

### 🎯 Objetivos

- Fornecer acesso fácil e rápido a dados sobre a Furia FC
- Responder dúvidas sobre jogos, jogadores e estatísticas
- Atender necessidades de fãs novos e experientes
- Criar uma experiência conversacional personalizada

## ⚙️ Funcionalidades

O FuriaBot oferece as seguintes funcionalidades principais:

### 📊 Informações sobre Jogos

- Resultados detalhados das partidas (março-abril 2025)
- Estatísticas por jogo (xG, chutes, posse de bola, etc.)
- Informações sobre gols marcados em cada partida

### ⚽ Estatísticas de Jogadores

- Artilharia individual dos jogadores
- Informações sobre gols especiais (gols do presidente e gols duplos)
- Desempenho em diferentes partidas

### 📅 Calendário e Resultados

- Histórico completo dos jogos disputados
- Detalhes sobre horários e locais das partidas
- Acompanhamento dos resultados mais recentes

### 🏆 Desempenho Geral

- Estatísticas de vitórias, empates e derrotas
- Desempenho ofensivo e defensivo da equipe
- Análise de tendências de desempenho

## 💻 Tecnologias Utilizadas

- **Linguagem de Programação**: [Python 3.9+](https://www.python.org/)
- **Frameworks de Chatbot**: [Rasa](https://rasa.com/) / [Botpress](https://botpress.com/)
- **Processamento de Linguagem Natural**: [spaCy](https://spacy.io/) / [NLTK](https://www.nltk.org/)
- **Armazenamento de Dados**: [SQLite](https://www.sqlite.org/) / [MongoDB](https://www.mongodb.com/)
- **Front-end** (opcional): [React](https://reactjs.org/) / [Vue.js](https://vuejs.org/)

## 📁 Estrutura de Dados

O chatbot utiliza uma base de dados estruturada com as seguintes informações:

### Resumo dos Jogos
```
- ID do jogo
- Data e hora
- Adversário
- Local
- Placar
- Resultado
```

### Dados de Gols
```
- ID do jogo
- Minuto do gol
- Jogador
- Tipo de gol (normal, duplo, presidente)
```

### Estatísticas por Jogo
```
- ID do jogo
- xG (Expected Goals)
- Chutes totais
- Chutes no alvo
- Posse de bola
- Precisão nos passes
- Escanteios
- Faltas cometidas
- Cartões amarelos
```

## 🔧 Instalação e Configuração

### Pré-requisitos

- Python 3.9+
- pip (gerenciador de pacotes Python)
- Node.js e npm (opcional, para interfaces web)

### Passos para Instalação

1. Clone o repositório:
```bash
git clone https://github.com/seu-usuario/furiabot.git
cd furiabot
```

2. Instale as dependências:
```bash
pip install -r requirements.txt
```

3. Configure as variáveis de ambiente:
```bash
cp .env.example .env
# Edite o arquivo .env com suas configurações
```

4. Inicialize o banco de dados:
```bash
python scripts/init_database.py
```

5. Treine o modelo (caso use Rasa ou similar):
```bash
rasa train
```

## 🎮 Como Usar

### Iniciar o Chatbot (Linha de Comando)

```bash
python run_bot.py
```

### Iniciar o Servidor Web (opcional)

```bash
python app.py
```
Acesse o chatbot em `http://localhost:5000`

### Integração com Plataformas

O FuriaBot pode ser integrado com:
- Discord
- Telegram
- WhatsApp
- Site da Furia FC

Consulte a documentação específica para cada plataforma na pasta `/docs/integrations/`.

## 💬 Exemplos de Interação

Aqui estão alguns exemplos de como interagir com o FuriaBot:

### Consultar Resultados de Jogos

**Usuário**: Qual foi o resultado do jogo contra o LOUD SC?

**FuriaBot**: O Furia FC venceu o LOUD SC por 6-1 em 14 de abril de 2025. Os gols foram marcados por Leleti (1'), Jeffinho (20'), Murillo Donato (30'), Lipão (32') e Jeffinho novamente (34').

### Informações sobre Jogadores

**Usuário**: Quantos gols o Leleti marcou no total?

**FuriaBot**: Leleti é o artilheiro da Furia FC com 12 gols marcados no período de março-abril de 2025. Ele também marcou 2 gols duplos, contra o Nyvelados FC e o G3X FC.

### Estatísticas Detalhadas

**Usuário**: Quais foram as estatísticas de posse de bola no jogo contra o Desimpedidos Goti?

**FuriaBot**: No jogo contra o Desimpedidos Goti (26 de abril de 2025), a Furia FC teve 76% de posse de bola, enquanto o Desimpedidos Goti ficou com 24%. A precisão nos passes da Furia FC foi de 95%, contra 88% do adversário.

### Gols Especiais

**Usuário**: Quem marcou gols duplos para o Furia FC?

**FuriaBot**: A Furia FC teve 3 gols duplos: Leleti marcou 2 gols duplos (contra Nyvelados FC e G3X FC) e Lipão marcou 1 gol duplo (contra Capim FC).

## 🔮 Próximos Passos

O desenvolvimento do FuriaBot continuará com os seguintes recursos planejados:

- [ ] Integração com dados em tempo real das partidas
- [ ] Alertas personalizados para jogos futuros
- [ ] Expandir a base de conhecimento para temporadas anteriores
- [ ] Recursos de análise preditiva para próximos jogos
- [ ] Suporte para consultas por linguagem natural mais complexas
- [ ] Interface gráfica aprimorada com visualizações estatísticas

## 👥 Contribuição

Contribuições são sempre bem-vindas! Siga estes passos para contribuir:

1. Faça um fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/nova-funcionalidade`)
3. Commit suas mudanças (`git commit -m 'Adiciona nova funcionalidade'`)
4. Push para a branch (`git push origin feature/nova-funcionalidade`)
5. Abra um Pull Request

Por favor, consulte o arquivo [CONTRIBUTING.md](CONTRIBUTING.md) para mais detalhes.

## 📝 Licença

Este projeto está licenciado sob a licença MIT - veja o arquivo [LICENSE.md](LICENSE.md) para mais detalhes.

---

<div align="center">
  Desenvolvido com ❤️ para os fãs da Furia FC
  <br>
  © 2025 FuriaBot
</div>
