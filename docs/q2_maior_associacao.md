2) Quais campos apresentam maior associação com o campo phishing (se a URL é phishing ou não)?


Código usado:

```sql
SELECT 
    phishing,
    AVG(url_length) AS avg_url_length,
    AVG(n_dots) AS avg_n_dots,
    AVG(n_hypens) AS avg_n_hypens,
    AVG(n_slash) AS avg_n_slash,
    AVG(n_questionmark) AS avg_n_questionmark,
    AVG(n_equal) AS avg_n_equal,
    AVG(n_at) AS avg_n_at,
    AVG(n_redirection) AS avg_n_redirection
FROM phishing_data
GROUP BY phishing;
```

Resultado:

<img width="1017" height="312" alt="Image" src="https://github.com/user-attachments/assets/4b37ea7e-c0b3-4365-8424-2f00a1f239b3" />


Podemos analisar que as variáveis com maior diferença da média são:

- url_length: Uma diferença de aproximadamente 43 caracteres entre as médias.
- n_slash: Uma diferença de aproximadamente 2.4 ocorrências entre as médias.
- n_equal: Também apresenta aumento relevante entre as médias.
- n_hypens: Indica maior presença de hífens em URLs phishing.

Assim podemos associar mais as variáveis url_length, n_slash, n_equal e n_hypens com a variável phishing.
