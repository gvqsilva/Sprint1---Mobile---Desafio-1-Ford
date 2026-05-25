# 🚙 AutoIntel AI | Ford Market Intelligence

![Ford Logo](https://upload.wikimedia.org/wikipedia/commons/thumb/a/a0/Ford_Motor_Company_Logo.svg/512px-Ford_Motor_Company_Logo.svg.png)

## 📌 a) Sobre o Projeto

**Nome do Aplicativo:** AutoIntel AI
**Desafio Escolhido:** Inovação em Inteligência de Mercado e Engenharia de Produto (P&D).

**Por que escolhemos este desafio?**
A indústria automotiva é altamente competitiva e a tomada de decisão para o lançamento de novos produtos ou *facelifts* exige o cruzamento de milhares de dados. Escolhemos este desafio porque identificamos uma lacuna: analistas perdem dias tabulando fichas técnicas e preços da concorrência. O AutoIntel AI resolve isso utilizando Inteligência Artificial Generativa para extrair dados do mercado em tempo real, gerar comparativos (Duelos) contra a linha Ford (especificamente a Ranger Raptor) e ditar as diretrizes da próxima geração de veículos (Next-Gen).

**Lista Completa de Funcionalidades:**
- **Varredura de Mercado (Matriz de Dados):** Extração de atributos técnicos e preços atualizados de SUVs e Picapes concorrentes via IA.
- **Duelo Estratégico vs. Raptor:** Cruzamento analítico avaliando Força, Tecnologia, Off-Road e Custo-Benefício.
- **Radar Estratégico (Dashboard Executivo):** Tela avançada gerando Mapa de Ameaças, Matriz de Lacunas de Equipamentos (White-space) e Diretrizes P&D escritas pela IA.
- **Copiloto Tático de Vendas:** Chatbot treinado para responder a objeções de clientes através de "Battle Cards" focados nos diferenciais da Ford.
- **Cofre de Inteligência:** Armazenamento local *offline* do histórico de relatórios simples e dashboards avançados.
- **Exportação de Dossiê:** Geração e compartilhamento do relatório executivo em formato Imagem/PDF via WhatsApp ou E-mail.

---

## 👥 b) Integrantes do Grupo

| Nome Completo | RM | Turma |
| :--- | :--- | :--- |
| **Augusto Mendonça** | RM 558371 | [3ESPG] |
| **Gabriel Vasquez** | RM 557056 | [3ESPG] |
| **Gustavo Oliveira** | RM 559163 | [3ESPG] |


---

## 🚀 c) Como Rodar o Projeto

**Pré-requisitos:**
- Node.js instalado (versão LTS recomendada)
- Aplicativo **Expo Go** no smartphone ou um emulador (Android/iOS)
- npm ou yarn

**Passo a passo para execução:**

1. Clone o repositório e acesse a pasta do projeto:

```bash
git clone https://github.com/seu-usuario/autointel-ford.git
cd autointel-ford
```

2. Instale as dependências e inicie o servidor do Expo (limpando o cache recomendado):

```bash
npm install
npx expo start -c
```

Ou, com yarn:

```bash
yarn install
yarn expo start --clear
```

3. Teste o aplicativo: abra o app Expo Go no celular e escaneie o QR Code exibido no terminal. Certifique-se de que computador e celular estão na mesma rede Wi‑Fi.

### 📱 Demonstração Visual (OBRIGATÓRIO)

Substituam os links/indicadores abaixo pelas imagens reais do projeto. Arrastem as imagens para a pasta do repositório ou usem links públicos (Imgur/GitHub):
- Fluxo Principal: GIF/Vídeo mostrando Home → Pesquisa → Geração do Duelo → Radar
- Telas: Painel (Home), Matriz de Dados (Pesquisa), Radar (Dashboard), Copiloto, Cofre de Inteligência

---

## 🧠 d) Decisões Técnicas

**Stack escolhida e justificativa:**
- Front-end: React Native com Expo — prototipação rápida e multiplataforma.
- IA: Groq Cloud API com modelo LLaMA-3.1-8B-Instant (nota: integrar conforme política de chaves e custos).
- Armazenamento: AsyncStorage para funcionamento offline e histórico local.

**Estrutura e integrações:**
- Navegação: `react-navigation` com BottomTabNavigator (Home, Pesquisa, Copiloto, Cofre) e Stack para `RadarScreen`.
- Exportação: `expo-sharing` + `react-native-view-shot` para gerar e compartilhar dossiês.

---

## 🔮 e) Próximos Passos (evolução)

- Web scraping dinâmico para preços (ex.: FIPE/Webmotors) via backend (Azure/AWS).
- Sincronização em nuvem (Firestore) para compartilhar dashboards entre usuários.
- Módulo de TCO para comparar custo total de propriedade em 3 anos.

---

## 📌 Notas de desenvolvimento

- Telas principais: [src/screens](src/screens) — altere `HomeScreen.js`, `PesquisaScreen.js`, `CopilotoScreen.js`, `RadarScreen.js`, `PerfilScreen.js` conforme necessidade.
- Mantenha chaves de API fora do repositório (use variáveis de ambiente / secrets).
- Se quiser, adapto este README para inglês, adicionar badges (build/Expo/license) ou criar um `CONTRIBUTING.md`.

