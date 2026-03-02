# Projeto-SQL-Phishing

Análise exploratória de dados de URLs de phishing utilizando SQL para identificar quais características indicam maior probabilidade de fraude.

Todos os queries foram executados utilizando SQLite.

Dataset utilizado:
https://www.kaggle.com/datasets/danielfernandon/web-page-phishing-dataset

Estrutura da Tabela:

Tabela: `phishing_data`

Principais colunas:

- url_length  
- n_dots  
- n_hypens  
- n_underline  
- n_slash  
- n_questionmark  
- n_equal  
- n_at  
- n_and  
- n_exclamation  
- n_space  
- n_tilde  
- n_comma  
- n_plus  
- n_asterisk  
- n_hastag  
- n_dollar  
- n_percent  
- n_redirection  
- phishing (0 para legítima, 1 para phishing)


Perguntas do Projeto:

1) Que código SQL você escreveria para consultar todos os dados contidos no conjunto de dados fornecido?

2) Qual(is) campo(s) apresentam maior correlação com o campo “phishing” (se a URL é phishing ou não)?

3) Qual(is) campo(s) apresentam menor correlação com o campo “phishing”?

4) O comprimento da URL (url_length) é um forte indicador de que a URL é phishing?

Justifique sua resposta.

Quais métricas foram utilizadas para apoiar essa conclusão?

5) O número de redirecionamentos (n_redirection) é um forte indicador de que a URL é phishing?

Justifique sua resposta.

Quais métricas foram utilizadas para apoiar essa conclusão?

6) Com base na sua análise, que recomendações você daria para identificar se uma URL pode ser phishing?
