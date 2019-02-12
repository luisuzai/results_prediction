# Previsão de resultados de jogos através de dados  
  
Prevendo resultados de jogos através de resultados utilizando Machine Learning.

## Entendendo as variáveis

'home_name': Nome do mandante,  
'away_name': Nome do visitante,  
'home_score': Gols feitos pelo mandante na partida,  
'away_score': Gols feitos pelo visitante na partida,  
'final_result': Essa é a variável que queremos prever, trata-se do resultado final, sendo H (Home) Vitória do Mandante, D (Draw) Empate, e, por fim, A (Away) visitante,  
'time': Tempo em formato unix,  
'home_pos': A posição do mandante antes dessa partida,  
'away_pos': A posição do visitante antes dessa partida,  
'round': A rodada do campeonato,  
'home_last5all_home': Saldo de gols do mandante nas últimas 5 partidas,  
'home_last5all_home_win': Nº de vitórias do mandante nas últimas 5 partidas,  
'home_last5all_home_draw': Nº de empates do mandante nas últimas 5 partidas,  
'home_last5all_home_lose': Nº de derrotas do mandante nas últimas 5 partidas,  
'away_last5all_away': Saldo de gols do visitante nas últimas 5 partidas,  
'away_last5all_away_win': Nº de vitórias do visitante nas últimas 5 partidas,  
'away_last5all_away_draw': Nº de empates do visitante nas últimas 5 partidas,  
'away_last5all_away_lose': Nº de derrotas do visitante nas últimas 5 partidas,  
'last5all_home_away_dif': A diferença do saldo entre as equipes, ou seja: 'home_last5all_home' - 'away_last5all_away'  
'fifa_home_ova': Score Geral do Mandante no Fifa  
'fifa_home_att': Score de ataque do Mandante no Fifa  
'fifa_home_mid': Score de meio de campo do Mandante no Fifa  
'fifa_home_def': Score de defesa do Mandante no Fifa  
'fifa_away_ova': Score Geral do Visitante no Fifa  
'fifa_away_att': Score de ataque do Visitante no Fifa  
'fifa_away_mid': Score de meio de campo do Visitante no Fifa  
'fifa_away_def': Score de defesa do Visitante no Fifa  
'elo_home_score': Score Elo do Mandante  
'elo_away_score': Score Elo do Visitante   
'tfm_value_home': Valor de mercado do elenco mandante em Euros  
'tfm_value_away': Valor de mercado do elenco visitante em Euros  

Estamos aqui com um problema de aprendizagem supervisionada, uma classificação. A variável dependente (target value) é o 'final_result', que possui 3 possíveis valores: H, D ou A, assim ela será o 'y' da sua modelagem. Ao criar a matriz de variáveis não esqueça de remover 'home_score' e 'away_score', afinal se o algoritmo sabe o placar final da partida ele será capaz de fazer previsões 100% acuradas. =)

