# GS-IOT - Identificação de Carregadores de Carros Elétricos com Visão Computacional

Este projeto aplica Deep Learning e Visão Computacional para identificar carregadores de carros elétricos em imagens, visando auxiliar motoristas e gerentes de infraestrutura de recarga elétrica em soluções de monitoramento e localização.

---

## Video Apresntação
https://youtu.be/anItmY5qJ_U

## Integrantes
RM: 553227 - Herbert Santos de Sousa
RM: 553698 - João Pedro Pereira
RM: 553643 - Enzo Franco Rocha

## Objetivo
Desenvolver um modelo de visão computacional de alta precisão para reconhecimento de carregadores de carros elétricos.
Nosso projeto busca auxiliar motoristas de carros elétricos na identificação de pontos de recarga e planejamento de viagens. Usando Deep Learning e Visão Computacional, o objetivo é criar uma solução capaz de identificar carregadores de carros elétricos em imagens, oferecendo suporte para motoristas que precisam encontrar pontos de recarga durante suas viagens. Com futuras atualizações buscamos atualizar os mapas para dar mais opções de pontos de interesse para os usuários. Nosso modelo será implementado nos mapas fornecidos pelo nosso Front-End, atuando de maneira conjunta para a identificação dos “ChargePoints”.

## Estrutura do Projeto

### 1. Preparação dos Dados
- **Definição de Classes**: Identificação dos tipos de carregadores a serem detectados.
- **Coleta de Imagens**: Obtenção de imagens variadas em condições de luz e ângulos distintos.
- **Anotação de Imagens**: Marcação das áreas de interesse utilizando uma ferramenta de anotação.

### 2. Configuração do Projeto no Roboflow
- **Gerenciamento**: Criação de um projeto no Roboflow para organizar e categorizar o dataset.
- **Upload e Categorização**: Envio das imagens e categorização dos carregadores.
- **Data Augmentation**: Aplicação de técnicas de aumento de dados para melhorar a robustez do modelo.

### 3. Pré-processamento dos Dados
- **Redimensionamento**: Ajuste das imagens para uma resolução padrão de 640x640 pixels.
- **Divisão do Dataset**: Separação dos dados em 70% para treinamento, 20% para validação e 10% para testes.

### 4. Treinamento do Modelo
- **Modelo Utilizado**: YOLOv5, um dos principais modelos de detecção de objetos.
- **Parâmetros**: Configuração de 50 épocas e tamanho de lote de 16.
- **Ajuste de Hiperparâmetros**: Monitoramento das métricas para melhorar o desempenho.

### 5. Avaliação do Modelo
- **Métricas de Precisão**: Avaliação com mAP (mean Average Precision).
- **Ajustes de Precisão**: Melhorias para alcançar 92% de precisão no dataset de teste.
- **Testes Adicionais**: Testes com imagens inéditas para verificar a generalização.

### 6. Teste Final com Input de Imagens
- **Validação Realista**: Teste com imagens adicionais para validar o modelo. Os carregadores foram identificados de forma precisa, comprovando a aplicabilidade.

### 7. Exportação e Integração
- **Exportação do Modelo**: Exportação em formato TensorFlow para facilitar a implementação em sistemas de produção.
- **Integração com OpenCV**: Preparado para integração em tempo real.

## Requisitos para o Projeto

- **Conta no [Roboflow](https://roboflow.com/)**: Gerenciamento do dataset e treinamento.
- **Bibliotecas**: TensorFlow e OpenCV para exportação e integração.
- **Conhecimento Básico**: Python e manipulação de datasets de visão computacional.

## Testes e Avaliação
O modelo foi testado com um conjunto variado de imagens para garantir sua precisão. Durante o teste final, fornecemos imagens como input, e o modelo identificou carregadores corretamente em diferentes condições.

## Conclusão
O modelo está pronto para uso em sistemas de monitoramento e localização de carregadores de carros elétricos, com precisão que pode ser melhorada com ajustes e novos dados.

## Configuração

1. **Roboflow**: Crie um projeto e organize o dataset, aplicando data augmentation conforme necessário.
2. **YOLOv5**: Use YOLOv5 com os parâmetros especificados (50 épocas, tamanho de lote 16).
3. **Exportação**: Exporte o modelo para TensorFlow e configure-o com OpenCV.
4. **Testes**: Realize testes variados para ajustar a precisão e verificar a eficácia em cenários reais.

--- 

Este projeto representa um passo em direção ao uso de visão computacional para aprimorar a infraestrutura de carregadores de veículos elétricos e oferecer uma experiência de recarga mais eficiente e acessível.
