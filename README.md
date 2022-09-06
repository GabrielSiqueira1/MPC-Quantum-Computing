# MPC-Quantum-Computing
Esse projeto usa MPC (Modelo de controle preditivo) juntamente com o controle quântico para manipulação da função de onda apresentada na equação de Schrodinger, a base para mecânica quântica

Para realizar tal procedimento, é utilizado a linguagem Python no projeto Jupyter. 

---

## Atividade 1

### Projeção das soluções - Invariante no tempo

O objetivo dessa atividade é desenvolver gráficos referentes a solução da equação de Schrodinger e em um primeiro momento foi desenvolvido para a solução usando polinômios de Hermite.

Para que seja possível utilizar tal solução, considerou-se um sistema massa mola, ou seja, um oscilador harmônico simples $V(x)=m\cdot\omega^{2}\cdot x²/2$

Na imagem abaixo é apresentado a solução para os polinômios 0 e 1, sua complementação está disposto no projeto .ipynb.

<div align="center">
  <img src="curvas.png" />
</div>

Afim de mostrar a transação entre os polinômios de Hermite, construiu-se o gráfico em vermelho, mostrando todas as posições até o polinômio de grau 50.

https://user-images.githubusercontent.com/109818266/188744905-b86a165a-71fa-478f-a492-ec43c457f8bf.mp4

Para análise completa, recomenda-se visitar o projeto .ipynb.

Ainda nessa etapa estamos considerando a equação de Schrodinger invariante no tempo, e conforme visto em Mecânica Quântica, a solução da equação pode ser vista com a combinação linear das soluções da função de onda, nesse caso, as de grau 0 e 1. Quando realizamos as possíveis combinações lineares é conseguimos ver a transição de uma função de onda à outra conforme abaixo:


https://user-images.githubusercontent.com/109818266/188745487-5d7f9ff4-e84f-4d32-9f7c-f1ed00cedae6.mp4

### A variação no tempo

Para compor a resposta e representar a variação no tempo podemos multiplicar cada fator achado por $e^{-iE_nt/\hbar}$ e conforme disposto no projeto, a solução concebida variará em x conforme o gráfico e em t ocorrerá uma manipulação acreditando que a equação esteja certa.

### Método de Crank-Nicolson
