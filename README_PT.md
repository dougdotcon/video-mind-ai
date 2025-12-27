# VideoMind AI

<div align="center">
  <img src="logo.png" alt="VideoMind AI Logo" width="200"/>
</div>

Uma solução avançada de automação para criação de conteúdo em vídeo para YouTube Shorts utilizando Inteligência Artificial.

## Sobre o Projeto

VideoMind AI é uma ferramenta de automação desenvolvida em Node.js que revoluciona o processo de criação de conteúdo para YouTube Shorts. Através da integração de tecnologias de ponta em IA, o sistema automatiza todo o pipeline de produção, desde a geração do roteiro até a publicação do vídeo.

Artigo detalhado sobre o projeto: [Automatizando a Geração de Conteúdo no YouTube com Inteligência Artificial e Programação](https://medium.com/@thiagobergamig/automatizando-a-gera%C3%A7%C3%A3o-de-conte%C3%BAdo-no-youtube-com-intelig%C3%AAncia-artificial-e-programa%C3%A7%C3%A3o-f50f095d0e70)

## Funcionalidades Principais

### 1. Geração Automatizada de Roteiros
- Utilização do ChatGPT-4 para criação de roteiros otimizados
- Análise contextual para garantir relevância do conteúdo
- Adaptação automática para o formato de Shorts

### 2. Síntese Avançada de Voz
- Integração com Google Cloud Text-to-Speech
- Suporte a múltiplos idiomas e sotaques
- Controle de entonação e velocidade da fala
- Processamento de áudio em alta qualidade

### 3. Processamento Profissional de Vídeo
- Edição automatizada utilizando FFmpeg
- Sistema robusto de composição de cenas
- Suporte a múltiplos formatos de entrada
- Otimização para formato vertical (9:16)
- Controle preciso de qualidade e compressão

### 4. Sistema de Legendagem
- Geração automática de legendas via CapCut
- Sincronização precisa com o áudio
- Estilos personalizáveis de legendas
- Suporte a múltiplos idiomas

### 5. Otimização para SEO
- Geração inteligente de descrições com ChatGPT-4
- Análise de tendências para keywords
- Otimização de títulos e tags
- Conformidade com boas práticas do YouTube

## Requisitos do Sistema

### Software
- Node.js 16.x ou superior
- FFmpeg 4.x ou superior
- CapCut (última versão)
- Conta ativa no Google Cloud Platform
- Acesso à API do ChatGPT-4

### Hardware Recomendado
- Processador: Intel i5/AMD Ryzen 5 ou superior
- Memória RAM: 8GB mínimo (16GB recomendado)
- Armazenamento: SSD com 256GB de espaço livre
- Conexão de Internet: 10Mbps ou superior

## Estrutura do Projeto


src/
├── audio/
│   └── audio.js         # Processamento de áudio
├── chatGPT/
│   ├── chatGPT.js      # Integração com ChatGPT
│   └── longText.js      # Processamento de texto longo
├── video/
│   ├── cropVideo.js     # Recorte de vídeo
│   ├── editVideo.js     # Edição principal
│   └── joinVideo.js     # Composição final
└── index.js             # Ponto de entrada


## Instalação

1. Clone o repositório:
bash
git clone https://github.com/seu-usuario/videomind-ai.git
cd videomind-ai


2. Instale as dependências:
bash
npm install


3. Configure as variáveis de ambiente:
bash
cp .env.example .env
# Edite o arquivo .env com suas credenciais
