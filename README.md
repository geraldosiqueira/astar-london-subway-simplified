# astar-london-subway-simplified

Adaptative Cognitive Agents' first assignment using A* algorithm

# London Subway Problem with Simplified Map

Using A* algorithm to solve the London Subway Problem with Simplified Map

The users can choose the staions from witch they will depart and where they will arrive, and the output is given as the best path between the stations, considering the time taken in the journey. Other informations given is the distance to travel and the lines color info. 
Border evaluation for time taken from goal to destination is considered with the train at 40 km/h and a 3 minute interval when changing subway lines.



This code was adapted from the Paris Subway Simplified Problem to consider the london map and the time as a factor, not the distance.


**Output Exemple: From E5, Yellow => E7, Blue**

Busca A* no mapa de londres

	 Percurso: E5, Amarelo => E7, Azul

====================================

Fronteira de Busca 		: [(23.4, 'E4, Amarelo')]
Estações Expandidas 		: ['E5, Amarelo']  #1

Fronteira de Busca 		: [(26.4, 'E4, Vermelho'), (28.35, 'E8, Amarelo')]
Estações Expandidas 		: ['E5, Amarelo', 'E4, Amarelo']  #2

Fronteira de Busca 		: [(27.750000000000004, 'E3, Vermelho'), (28.35, 'E8, Amarelo'), (42.3, 'E14, Vermelho')]
Estações Expandidas 		: ['E5, Amarelo', 'E4, Amarelo', 'E4, Vermelho']  #3

Fronteira de Busca 		: [(28.35, 'E8, Amarelo'), (30.750000000000004, 'E3, Azul'), (39.6, 'E2, Vermelho'), (42.3, 'E14, Vermelho')]
Estações Expandidas 		: ['E5, Amarelo', 'E4, Amarelo', 'E4, Vermelho', 'E3, Vermelho']  #4

Fronteira de Busca 		: [(30.750000000000004, 'E3, Azul'), (31.35, 'E8, Azul'), (37.800000000000004, 'E9, Amarelo'), (39.6, 'E2, Vermelho'), (42.3, 'E14, Vermelho')]
Estações Expandidas 		: ['E5, Amarelo', 'E4, Amarelo', 'E4, Vermelho', 'E3, Vermelho', 'E8, Amarelo']  #5

Fronteira de Busca 		: [(31.35, 'E8, Azul'), (31.950000000000003, 'E7, Azul'), (37.800000000000004, 'E9, Amarelo'), (39.6, 'E2, Vermelho'), (42.3, 'E14, Vermelho')]
Estações Expandidas 		: ['E5, Amarelo', 'E4, Amarelo', 'E4, Vermelho', 'E3, Vermelho', 'E8, Amarelo', 'E3, Azul']  #6

Fronteira de Busca 		: [(31.950000000000003, 'E7, Azul'), (37.800000000000004, 'E9, Amarelo'), (39.6, 'E2, Vermelho'), (42.3, 'E14, Vermelho'), (46.95, 'E10, Azul')]
Estações Expandidas 		: ['E5, Amarelo', 'E4, Amarelo', 'E4, Vermelho', 'E3, Vermelho', 'E8, Amarelo', 'E3, Azul', 'E8, Azul']  #7

Fronteira de Busca 		: [(37.800000000000004, 'E9, Amarelo'), (39.6, 'E2, Vermelho'), (42.3, 'E14, Vermelho'), (46.95, 'E10, Azul')]
Estações Expandidas 		: ['E5, Amarelo', 'E4, Amarelo', 'E4, Vermelho', 'E3, Vermelho', 'E8, Amarelo', 'E3, Azul', 'E8, Azul', 'E7, Azul']  #8


=======================================================

Menor caminho 	: ['E5, Amarelo', 'E4, Amarelo', 'E4, Vermelho', 'E3, Vermelho', 'E3, Azul', 'E7, Azul']
Numero de estações visitas 			: 6
Distancia total percorrida 			: 17.3Km
Tempo total da viagem 			: 31.950000000000003min
