# Quando os Gigantes Enviam Emails?  
### Análise de +500.000 emails recebidos: horário exato que LinkedIn, NYT, Google, Globo, Meta, Substack e outros disparam suas mensagens

![Banner](grafico1_visao_geral.png)

**Um estudo real baseado em dados pessoais de inbox (incluindo Spam e Lixeira) de vários anos**  
Horários em **fuso horário de Brasília (BRT / UTC-3)**

## O que este projeto revela?

- Qual é o **horário de pico** de cada categoria (Portais de Notícias, Redes Sociais, Consultorias, Big Techs)
- Os **Top 15 remetentes** e o horário exato que eles mais enviam
- Heatmap completo: **hora × dia da semana**
- Comparativo percentual entre todas as categorias
- Insights estratégicos: **melhores horários para enviar seu próprio email/newsletter** (menor concorrência)

### Principais descobertas (exemplo real dos meus dados):

| Categoria              | Horário de Pico (BRT) | Período mais forte       | Dia preferido  |
|-----------------------|-----------------------|--------------------------|----------------|
| Portais de Notícias   | 7h–9h                 | Manhã (6h–11h)           | Terça-feira    |
| Redes Sociais         | 8h–10h / 18h–20h      | Manhã e início da noite  | Quarta-feira   |
| Consultorias          | 6h–8h                 | Início da manhã          | Segunda-feira  |
| Big Techs             | 9h–11h                | Final da manhã           | Quinta-feira   |

> Horários com **menor concorrência** (oportunidade!): 2h, 3h, 4h, 5h, 23h

## Gráficos gerados automaticamente

| Gráfico | Descrição |
|--------|---------|
| `grafico1_visao_geral.png` | Visão por categoria com pico destacado |
| `grafico2_comparativo.png` | Comparativo % hora a hora (todas as categorias) |
| `grafico3_top_fontes.png` | Top 15 fontes ordenadas pelo horário preferido |
| `grafico4_heatmap.png` | Heatmap hora × dia da semana (por categoria) |
| `grafico5_redes_sociais.png` | Detalhamento das 8 principais redes sociais |
| `grafico6_portais_noticias.png` | Detalhamento dos 10 principais portais/newsletters |

## Como usar este notebook

1. Faça upload do seu arquivo `.mbox` (exportado do Gmail, Outlook, etc.)
2. Altere a variável `MBOX_FILE` para o caminho do seu arquivo no Google Drive
3. Execute todas as células

> O script já converte automaticamente para o fuso horário de Brasília (BRT)

### Arquivo de entrada esperado
- Formato: `.mbox` (pode ser "Todos os e-mails, incluindo Spam e Lixeira" do Takeout do Google)
- Exemplo de caminho: `/content/drive/MyDrive/Todos os e-mails, incluindo Spam e Lixeira-002.mbox`

## Tecnologias usadas

- Python 3
- pandas não necessário → tudo feito com `collections` e `matplotlib` (mais rápido em grandes volumes)
- Google Colab + Google Drive
- matplotlib com tema dark personalizado (ideal para posts no LinkedIn)

## Autor

Feito por **Guilherme Favaron**  
Site: [guifav.github.io](https://guifav.github.io)  
Post original com os resultados: [[link do post no LinkedIn](https://www.linkedin.com/pulse/analisei-500-mil-emails-para-descobrir-quando-os-gigantes-favaron-e57gf)]

## Licença

MIT © 2025 – Sinta-se à vontade para fork, usar com seus próprios dados e publicar seus resultados!
