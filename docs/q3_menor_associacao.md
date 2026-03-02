3) Quais campos apresentam menor correlação com o campo “phishing”?

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

Usamos o mesmo código da questão 2.

As variáveis com menor diferença foram:

- n_dots
- n_redirection

Essas variáveis apresentaram valores médios muito próximos entre URLs legítimas e phishing, indicando baixa capacidade de distinção entre os dois grupos
