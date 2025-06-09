# PowerBI

## Formulas

% Preventiva = [Preventivas]/[Total de Ordens]

Meta de Preventiva = 80/100 

Ordens Corretivas = CALCULATE(COUNT(ordem_de_servico_da_manutencao_2021_bonisambiental[tipo_de_evento]),ordem_de_servico_da_manutencao_2021_bonisambiental[tipo_de_evento]="Corretiva")

Ordens Preventivas = CALCULATE(COUNT(ordem_de_servico_da_manutencao_2021_bonisambiental[tipo_de_evento]),ordem_de_servico_da_manutencao_2021_bonisambiental[tipo_de_evento]="Preventiva")

Preventivas = [Total de Ordens]-[Ordens Corretivas]

Total de Ordens = COUNT(ordem_de_servico_da_manutencao_2021_bonisambiental[tipo_de_evento])
