# Projeto 1, Redes Neurais Profundas

Este projeto consiste no desenvolvimento do primeiro trabalho avaliativo pela disciplina de Redes Neurais Profundas (UFG). Meu objetivo foi de atender aos critérios do trabalho e também de saciar minha curiosidade quanto ao impacto das técnicas de data augmentation e transfer learning na performance de modelos de deep learning.

O problema tratado aqui envolve a classificação de imagens dentre 100 classes de esportes possíveis. O dataset está disponível publicamente no Kaggle e contém cerca de 14000 imagens no total (contando treino, validação e teste). Como solução, foi implementado uma ResNet *from scratch* usando o PyTorch e também uma mistura entre a ResNet e a GoogLeNet (mais especificamente, juntei a ResNet com blocos _inception_). Esses dois modelos foram treinados em dois contextos diferentes: com e sem data augmentation. Por último, foi feito o finetuning por transfer learning da ResNet18, disponível no PyTorch.

O único arquivo disponível neste repositório é um pdf, que contém tanto o texto explicando as ideias por trás de tudo que fiz e também o código em Python que foi implementado. Como highlights deste projeto, pode-se citar uma função bastante interessante que foi implementada com a intenção de facilitar a visualização dos `classification_report`s para problemas de múltiplas classes. Os resultados convergiram com o que já era esperado, e deixaram clara a importância do data augmentation para a melhora na generalização das CNNs. Foi visto também que a técnica de transfer learning é promissora quando é passível de ser aplicada.

Faça bom proveito!
