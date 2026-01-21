# AR Mobile - Model7

Aplicação de Realidade Aumentada otimizada para dispositivos Android usando A-Frame e AR.js.

## 📱 Características

- **Otimizado para Android**: Interface touch-friendly e performance otimizada
- **Modelo Model7**: Carrega e exibe o arquivo `model7.glb` com animações
- **Múltiplos Marcadores**: Suporte para marcadores HIRO e códigos de barras
- **Controles Interativos**: Botões para controlar modelos e animações
- **Responsivo**: Adapta-se a diferentes tamanhos de tela

## 🎯 Marcadores Suportados

### Marcador HIRO
- **Modelo**: Model7 principal com animação de rotação
- **Efeitos**: Elementos decorativos animados ao redor
- **Escala**: 0.8x para melhor visualização

### Marcador Código #17
- **Modelo**: Model7 em escala menor (0.4x)
- **Extras**: Octaedro e cubo animados
- **Texto**: "Model7 AR Experience"

### Marcador Código #10
- **Modelo**: Model7 como elemento principal
- **Secundário**: Helicóptero com hélices animadas
- **Posição**: Movimento vertical suave

## 🚀 Como Usar

### 1. Preparação dos Arquivos
```
projeto/
├── index.html
├── model7.glb (arquivo principal)
└── objetos/
    ├── helicoptero.glb
    ├── helicea.glb
    └── heliceb.glb
```

### 2. Marcadores
Você precisa dos seguintes marcadores impressos:
- **HIRO**: Marcador padrão do ARToolKit
- **Código #17**: Barcode disponível no ARToolKit5
- **Código #10**: Barcode disponível no ARToolKit5

### 3. Servidor Local
```bash
# Usando Python
python -m http.server 8000

# Usando Node.js
npx serve .

# Usando PHP
php -S localhost:8000
```

### 4. Acesso no Android
1. Abra o navegador (Chrome recomendado)
2. Acesse `http://seu-ip:8000`
3. Permita o acesso à câmera
4. Aponte para os marcadores

## 🎮 Controles

- **Toggle Model7**: Mostra/oculta o modelo principal
- **Toggle Animação**: Liga/desliga todas as animações
- **Reset Scale**: Restaura escala padrão dos modelos

## 📋 Requisitos

### Dispositivo Android
- **Android 7.0+** (recomendado)
- **Chrome 90+** ou navegador compatível com WebRTC
- **Câmera** com foco automático
- **Conexão à internet** (primeira carga)

### Arquivo Model7.glb
- Coloque o arquivo `model7.glb` na raiz do projeto
- Tamanho recomendado: < 10MB para melhor performance
- Formatos suportados: GLB, GLTF

## ⚡ Otimizações Mobile

### Performance
- Renderer otimizado para mobile
- Anti-aliasing desabilitado em dispositivos menos potentes
- Iluminação balanceada para economia de bateria

### Interface
- Botões grandes para touch
- Prevenção de zoom acidental
- Auto-reload na mudança de orientação

### Detecção de Marcadores
- Ratio de padrão otimizado (0.8)
- Múltiplos métodos de detecção
- Buffer logarítmico para melhor profundidade

## 🐛 Solução de Problemas

### Câmera não funciona
- Verifique permissões do navegador
- Use HTTPS ou localhost
- Teste em Chrome/Firefox

### Model7.glb não carrega
- Verifique se o arquivo está na raiz
- Confirme o nome exato do arquivo
- Teste o arquivo em um visualizador GLB

### Performance baixa
- Reduza a qualidade do modelo GLB
- Use modelos com menos polígonos
- Feche outros aplicativos

### Marcadores não detectam
- Imprima em alta qualidade
- Use boa iluminação
- Mantenha distância adequada (20-50cm)

## 📦 Estrutura do Código

### HTML/CSS
- Layout responsivo
- Controles fixos na tela
- Estilos otimizados para mobile

### A-Frame Components
- Múltiplos marcadores AR
- Assets precarregados
- Animações suaves

### JavaScript
- Controle de visibilidade
- Gerenciamento de eventos
- Otimizações de performance

## 📄 Licença

Este projeto é baseado em:
- **A-Frame**: Mozilla (MIT License)
- **AR.js**: Jerome Etienne (MIT License)
- **ARToolKit**: University of Washington (GPL License)

## 🤝 Contribuição

Sinta-se livre para:
1. Fazer fork do projeto
2. Criar uma branch para sua feature
3. Commit suas mudanças
4. Push para a branch
5. Abrir um Pull Request

---

**Desenvolvido para dispositivos Android com foco em performance e usabilidade.**
