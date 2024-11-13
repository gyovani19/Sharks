Análise de Dados de Captura de Tubarões no Rio de Janeiro

Este script em Python realiza a análise de dados de captura de tubarões no estado do Rio de Janeiro. Ele utiliza bibliotecas como Pandas e NumPy para carregar, processar e calcular proporções de dados relacionados a capturas específicas ao longo dos anos.
Requisitos

    Python 3.x
    Bibliotecas: Pandas e NumPy

Para instalar as bibliotecas necessárias, execute:

pip install pandas numpy

Descrição do Script
1. Coleta e Carregamento dos Dados

O script começa carregando os dados a partir de um arquivo Excel especificado no caminho 'C:/Users/Meu Computador/Documents/Tubaroes/RJ_Reconstrucao_Tubaroes_2024_11_04.xlsx'. Os dados contêm informações sobre diferentes tipos de capturas de tubarões ao longo dos anos.
2. Seleção e Preparação de Dados

Após carregar os dados, o script:

    Seleciona colunas de interesse, incluindo 'Ano', 'Cacao_art', 'Cacao_ind', 'Cacao_art_ind', 'Cacao_anequim_art', 'Cacao_anequim_ind' e 'Cacao_azul_art'.
    Calcula uma coluna chamada 'Soma', que representa a soma dos valores de captura para cada ano. Valores ausentes (NaN) são ignorados na soma.

3. Filtragem de Linhas

Para garantir a precisão da análise, o script remove quaisquer linhas onde a coluna 'Soma' seja igual a zero ou NaN, mantendo apenas linhas com dados válidos.
4. Cálculo da Proporção

Uma nova coluna, 'Prop_Cacao_ind', é criada, representando a proporção de 'Cacao_ind' em relação à coluna 'Soma'.
5. Exibição Completa dos Dados

O script configura o Pandas para exibir todas as linhas do DataFrame resultante, permitindo a visualização de todos os anos com dados disponíveis.
6. Predição (Opcional)

O script organiza os anos com dados existentes e um conjunto adicional de anos para prever possíveis capturas. Esses anos são combinados e ordenados em um único array chamado todos_anos.
Exemplo de Uso

Após executar o script, os dados processados serão exibidos no console, mostrando:

    Ano
    Valores de 'Cacao_ind'
    A soma dos valores de captura para cada ano ('Soma')
    A proporção de 'Cacao_ind' em relação a 'Soma' ('Prop_Cacao_ind')

Observações

    Certifique-se de que o arquivo Excel esteja no caminho especificado.
    O script inclui mensagens de verificação para auxiliar na inspeção e depuração dos dados carregados.

Autor

Esse script foi desenvolvido para facilitar a análise de dados históricos de captura de tubarões no Rio de Janeiro.
