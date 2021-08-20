## Trabalho I - Reinforcement Learning - Problema de Transporte de Objeto

FURB - Pós Graduação em Data Science<br/>
Reinforcement Learning<br/>
Aluno: Felipe Eduardo Gomes<br/><br/>

1. **Modelagem do MDP:**  
	*a) Apresente a modelagem de estados considerada, bem como a quantidade de estados presentes no MDP. Inclua na contagem os estados não válidos;*<br/>
	R: **Os estados são as coordenadas x (colunas) e y (linhas) das células do mundo sendo 7 x 6 respectivamente. Os estados inválidos (agente não consegue transpor) são as coordenadas das células onde encontram-se as paredes.**
	
	b) *Apresente a modelagem das ações que o agente pode executar;*<br/>
	R: **O agente pode mover-se para CIMA, DIREITA, ABAIXO, ESQUERDA ou ainda permanecer na mesma posição (não se move), caso a posição que ele deveria andar confronta com uma parede ou borda do mundo.**
	
	c) *Apresente a modelagem da função de recompensa, com as situações em que o agente é recompensado bem como a magnitude da recompensa. Justifique as suas escolhas.*<br/>
	R: **Cada estado possui 4 ações possíveis (CIMA, DIREITA, ABAIXO, ESQUERDA ) e cada ação possui um atributo qValue que inicialmente possui valor zero.**

3. **Configuração dos Experimentos**  
	a) *Apresente os valores de taxa de aprendizagem (alfa) e fator de desconto (gamma) do algoritmo de aprendizagem Q-Learning;*<br/>
	R: 	
	| alpha | gamma |
	|--|--|
	| 0.1 | 1.0 |  
	
	b) *Apresente as configurações do horizonte de aprendizagem, que é representado pela quantidade máxima de passos de tempo por episódios, quantidade máxima de episódios, e política de exploração ao longo do tempo;*<br/>
	R: 
	| num_episodes | epsilon |
	|--|--|
	| 500 | 0.05 |

4. **Resultados Experimentais**  
	a) *Apresente a curva de convergência, representada pela quantidade de passos (timesteps) necessários para resolver a tarefa ao longo do tempo (episódios).*<br/>
	R:
	![](https://github.com/gomesfg/reinforcement_learning/blob/e40b637a7d387eba2bba011228cb3492f83eb739/curva_aprendizado.PNG?raw=true)
	