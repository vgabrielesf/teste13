# Pasta para Modelos 3D

Esta pasta deve conter os modelos 3D utilizados na aplicação AR:

## Arquivos Necessários:

### 📁 Raiz do projeto:
- `model7.glb` - **PRINCIPAL**: Seu modelo personalizado

### 📁 /objetos/ (esta pasta):
- `helicoptero.glb` - Modelo do helicóptero (corpo principal)
- `helicea.glb` - Hélice principal (animada)
- `heliceb.glb` - Hélice traseira (animada)

## 📋 Instruções:

1. **Coloque o `model7.glb` na raiz do projeto** (mesmo nível do index.html)
2. **Coloque os outros modelos nesta pasta** (/objetos/)
3. **Certifique-se de que os nomes dos arquivos estão exatos** (case-sensitive)

## 🎨 Formatos Suportados:
- ✅ **GLB** (recomendado) - Binário, menor tamanho
- ✅ **GLTF** - Texto, com arquivos separados

## ⚡ Otimizações para Mobile:
- **Tamanho máximo recomendado**: 10MB por modelo
- **Polígonos**: < 50,000 para melhor performance
- **Texturas**: Máximo 2048x2048 pixels
- **Compressão**: Use Draco quando possível

## 🔧 Ferramentas Úteis:
- **Otimização**: [glTF Optimizer](https://gltf.ensoftcorp.com/optimize)
- **Visualização**: [glTF Viewer](https://gltf-viewer.donmccurdy.com/)
- **Conversão**: [Blender](https://www.blender.org/) (File > Export > glTF 2.0)

---

**Nota**: Se você não tiver alguns dos modelos secundários (helicóptero), pode comentar as respectivas linhas no `index.html` ou substituir por outros modelos GLB/GLTF.
