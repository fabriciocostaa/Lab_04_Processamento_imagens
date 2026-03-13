# Projeto de Filtragem de Imagem com Webcam 🎥

Autores

- Fabricio da Costa Fernandes (RA: 11202321635)
- Felipe de Lima Major (RA: 11202230321)
- Lilian Gimenez Teixeira (RA: 11202332321)

Estrutura do projeto

O notebook contém uma série de experimentos com filtros de suavização, incluindo média, gaussiano, mediana e bilateral, aplicados sobre imagens estáticas e também sobre o fluxo de vídeo da webcam em tempo real.

Conteúdo dos experimentos

1. **Leitura e exibição de imagens**: carregamento de imagens estáticas (`foto-grupo.jpeg` e `avatares.png`) utilizando OpenCV e visualização com matplotlib.
2. **Funções de filtragem**:
   - `mediana()` - aplica o filtro da mediana com diferentes tamanhos de kernel
   - `gaussian()` - aplica o filtro gaussiano
   - `bilateral()` - aplica o filtro bilateral
   - `media()` - aplica o filtro de média (homogeneous blur)
3. **Inserção de ruído**: função `add_gaussian_noise()` para adicionar ruído gaussiano às imagens.
4. **Sistema interativo com webcam**: um programa completo que permite ao usuário:
   - Escolher entre diferentes filtros (média, gaussiano, mediana, bilateral)
   - Ajustar o tamanho do kernel (3x3, 5x5, 11x11, 29x29, 47x47)
   - Selecionar o tipo de ruído a ser inserido (sem ruído, gaussiano, sal-e-pimenta)
   - Visualizar o resultado em tempo real

Começando

Para reproduzir os experimentos em sua máquina:

1. **Pré-requisitos**:
   - Python 3.8+
   - Bibliotecas listadas no arquivo `requirements.txt` ou instaladas via pip:
     ```bash
     pip install numpy opencv-python matplotlib scikit-image ipywidgets Pillow
     ```
   - Jupyter Notebook ou JupyterLab
   - Webcam funcional para os experimentos ao vivo

2. **Executar o notebook**:
   ```bash
   jupyter notebook main.ipynb
   
3. **Executar o programa de webcam interativo**:
   O notebook contém uma célula específica com o código completo para filtragem em tempo real. Para executá-lo, basta rodar a célula correspondente. O programa oferece controles via teclado:
   - **Filtros**: `a` (média), `g` (gaussiano), `m` (mediana), `b` (bilateral)
   - **Kernels**: `3` (3x3), `5` (5x5), `7` (11x11), `9` (29x29), `x` (47x47)
   - **Ruído**: `o` (sem ruído), `y` (gaussiano), `p` (sal-e-pimenta)
   - **ESC** para sair

4. **Resultados**:
   - As imagens filtradas são salvas automaticamente na pasta `static/` com nomes como `borramento_mediana3x3.jpg`, `borramento_gaussiano5x5.jpg`, etc.
   - O notebook também gera visualizações comparativas dos diferentes filtros aplicados.

Adaptações e melhorias

O código original foi adaptado para funcionar de maneira mais fluida, com comentários reduzidos e uma mistura de português e inglês nas variáveis, tornando-o mais didático e acessível para estudantes.

Conclusão

Este projeto demonstra na prática os conceitos fundamentais de filtragem de imagens utilizando OpenCV. Através dos experimentos realizados, foi possível observar:
- O efeito dos diferentes tipos de filtros na suavização de imagens
- A influência do tamanho do kernel no resultado final
- O comportamento dos filtros na presença de ruído
- A implementação de um sistema interativo em tempo real

Os resultados obtidos servem como base para experimentos mais avançados em processamento de imagens e visão computacional.

Para detalhes metodológicos e explicações mais aprofundadas, consulte o próprio notebook `main.ipynb`.

Referências

- Biblioteca OpenCV: https://opencv.org/
- Documentação do scikit-image: https://scikit-image.org/
- Documentação do Jupyter Notebook: https://jupyter.org/

*Última atualização: 13 de março de 2026*
