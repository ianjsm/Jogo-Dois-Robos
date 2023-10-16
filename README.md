# Simulação de Busca de Alimento por Robôs

Este projeto simula uma competição entre dois robôs em busca de alimento. Os robôs se movem aleatoriamente, um de cada vez, até que um deles encontre o alimento. Ao final da simulação, o programa mostrará qual robô encontrou o alimento primeiro, bem como o número de movimentos válidos e inválidos de cada robô.

### Classe `Robo`

A classe `Robo` representa um robô em nosso cenário de busca de alimento. Cada robô possui os seguintes atributos:
- Posição atual no eixo x.
- Posição atual no eixo y.
- Cor que identifica o robô.
- Número de movimentos válidos.
- Número de movimentos inválidos.

A classe `Robo` possui os seguintes métodos:
- `moverAleatoriamente()`: Este método gera um movimento aleatório para o robô, onde ele pode se mover para cima, para baixo, para a direita ou para a esquerda. Antes de executar o movimento, ele verifica se o movimento é válido (ou seja, não resultará em uma posição negativa no eixo cartesiano). Os movimentos válidos aumentam o contador de movimentos válidos, e os movimentos inválidos aumentam o contador de movimentos inválidos.

- `encontrouAlimento(xAlimento, yAlimento)`: Este método verifica se o robô encontrou o alimento, comparando suas posições atuais com as coordenadas do alimento. Se o robô encontrar o alimento, ele retornará `true`; caso contrário, retornará `false`.

### Classe `Main`

A classe `Main` é a classe principal que controla a simulação da busca de alimento pelos robôs. Ela faz o seguinte:
1. Solicita ao usuário as coordenadas do alimento.
2. Instancia dois robôs com cores diferentes.
3. Inicia uma simulação em que os robôs se movem aleatoriamente, um de cada vez, até que um deles encontre o alimento.
4. Registra o número de movimentos válidos e inválidos de cada robô durante a simulação.
5. Quando um dos robôs encontra o alimento, o programa mostra qual robô o encontrou e exibe as estatísticas de movimentos válidos e inválidos de ambos os robôs.
