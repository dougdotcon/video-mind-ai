# VideoMind AI

<div align="center">
  <img src="logo.png" alt="VideoMind AI Logo" width="200"/>
</div>

Uma solução avançada de automação para criação de conteúdo em vídeo para YouTube Shorts utilizando Inteligência Artificial

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

```
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
```

## Instalação

1. Clone o repositório:
```bash
git clone https://github.com/seu-usuario/videomind-ai.git
cd videomind-ai
```

2. Instale as dependências:
```bash
npm install
```

3. Configure as variáveis de ambiente:
```bash
cp .env.example .env
# Edite o arquivo .env com suas credenciais
```

4. Configure o Google Cloud:
- Crie um projeto no Google Cloud Console
- Ative a API do Text-to-Speech
- Baixe e configure as credenciais de serviço

## Guia de Uso

1. Preparação do ambiente:
```bash
npm run setup
```

2. Geração de roteiro:
```bash
node src/chatGPT/chatGPT.js --prompt="seu-prompt-aqui"
```

3. Criação do áudio:
```bash
node src/audio/audio.js --input="roteiro.txt"
```

4. Processamento do vídeo:
```bash
node src/video/editVideo.js --input="video.mp4"
```

## Troubleshooting

### Problemas Comuns

1. **Erro na síntese de voz**
   - Verifique as credenciais do Google Cloud
   - Confirme a cota disponível de requisições
   - Valide o formato do texto de entrada

2. **Falha no processamento de vídeo**
   - Verifique a instalação do FFmpeg
   - Confirme o espaço em disco disponível
   - Valide o formato do vídeo de entrada

3. **Erro na geração de legendas**
   - Atualize o CapCut para a última versão
   - Verifique a compatibilidade do formato de áudio
   - Confirme as permissões de acesso

## Contribuindo

1. Fork o projeto
2. Crie sua Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a Branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

## Licença

Este projeto está licenciado sob a MIT License - veja o arquivo [LICENSE](LICENSE) para detalhes.

## Suporte

Para suporte e dúvidas, abra uma issue no repositório do GitHub.

## Reconhecimentos

- ChatGPT-4 pela geração de conteúdo inteligente
- Google Cloud pela infraestrutura de Text-to-Speech
- FFmpeg pelo processamento robusto de mídia
- CapCut pelas ferramentas de legendagem
