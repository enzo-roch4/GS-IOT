# GS-IOT


#Identificação de Carregadores de Carros Elétricos com Visão Computacional
Este projeto utiliza um modelo de Deep Learning de Visão Computacional para identificar carregadores de carros elétricos em imagens. O modelo foi desenvolvido para ser aplicado em soluções de monitoramento e localização de carregadores, visando auxiliar motoristas e gerentes de infraestrutura de recarga elétrica.

Objetivo
Desenvolver um modelo de visão computacional capaz de reconhecer diferentes tipos de carregadores de carros elétricos com alta precisão.

Estrutura do Projeto
Preparação dos Dados

Definição das classes de carregadores a serem detectados.
Coleta de imagens em diferentes condições de luz e ângulos para criar um dataset diversificado.
Anotação das imagens com uma ferramenta dedicada para marcar as áreas dos carregadores.
Configuração do Projeto no Roboflow

Criação de um projeto no Roboflow para gerenciamento do dataset.
Upload das imagens e categorização dos carregadores.
Aplicação de técnicas de aumento de dados (data augmentation) para melhorar a robustez do modelo.
Pré-processamento dos Dados

Redimensionamento das imagens para uma resolução padrão de 640x640 pixels.
Divisão do dataset em 70% para treinamento, 20% para validação e 10% para testes.
Treinamento do Modelo

Utilização do modelo YOLOv5 no Roboflow para detecção de objetos.
Configuração de parâmetros como 50 épocas e tamanho de lote de 16.
Monitoramento das métricas e ajuste dos hiperparâmetros conforme necessário.
Avaliação do Modelo

Avaliação do desempenho usando métricas de precisão, como mAP (mean Average Precision).
Ajustes para alcançar uma acurácia satisfatória de 92% no dataset de teste.
Testes adicionais com imagens inéditas para avaliar a generalização do modelo.
Teste Final com Input de Imagens

Para validar o funcionamento em cenários reais, fornecemos imagens adicionais como input. O modelo identificou os carregadores de forma precisa, demonstrando seu potencial de aplicação.
Exportação e Integração

Exportação do modelo em formato TensorFlow para facilitar a integração com sistemas de produção.
Pronto para integração com OpenCV, permitindo uso em tempo real.
Requisitos para o Projeto
Conta no Roboflow para gerenciamento do dataset e execução do treinamento.
Bibliotecas como TensorFlow e OpenCV para exportação e integração.
Conhecimento básico de Python e manipulação de datasets de visão computacional.
Testes e Avaliação
O modelo foi testado com um conjunto variado de imagens para garantir sua precisão. Durante o teste final, fornecemos imagens como input e o modelo conseguiu identificar carregadores corretamente em diferentes condições.

Conclusão
O modelo está pronto para implementação prática em sistemas de monitoramento e localização de carregadores de carros elétricos. Com a atualização contínua do dataset e ajustes no modelo, a precisão pode ser ainda mais refinada.
