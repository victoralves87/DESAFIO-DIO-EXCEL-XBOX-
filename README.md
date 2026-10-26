Planilha de análise de vendas de assinaturas do **Xbox Game Pass**, com base de assinantes, tabelas dinâmicas de apoio e um dashboard visual.
 
- **Período indicado no dashboard:** 01/01/2026 – 31/12/2026
- **Última atualização exibida:** 26/10/2026 09:00
- **Moeda:** R$ (valores sem decimais na base)
---

## Aba D̳ashboard
 
Título: **XBOX GAME PASS SUBSCRIPTIONS SALES**, com saudação de boas-vindas e data de atualização. Componentes:
 
- **Cartões de totais:** Total Xbox Game Pass, Cupons Sold, EA Play Season Pass e Minecraft Season Pass.
- **Gráfico de barras:** Total Value por renovação automática (Yes/No).
- **Slicer "Subscription Type":** filtra Monthly / Quarterly / Annual em todas as tabelas dinâmicas e no gráfico.
- Layout sem linhas de grade, com logos e ícones da aba `A̳ssets`.

- ## Aba C̳álculos — tabelas dinâmicas
 
Todas usam `Tabela1` como origem e são afetadas pelo slicer **Subscription Type**.
 
| Tabela dinâmica | Célula | Métrica | Uso |
|---|---|---|---|
| Tabela dinâmica1 | `G7` | Soma de Coupon Value | Cartão **Cupons Sold** (`H8` usa `GETPIVOTDATA`) |
| Tabela dinâmica3 | `G12` | Soma de Total Value por **Plan** | Total por plano (Core / Standard / Ultimate) |
| tbl_annual_value | `C12` | Soma de Total Value por **Auto Renewal** (Yes/No) | **Gráfico de barras** do dashboard |
| Tabela dinâmica2 | `C20` | Soma de EA Play Season Pass Price por Plan | Cartão **EA Play Season Pass** (`G24` usa `GETPIVOTDATA`) |
| Tabela dinâmica5 | `C31` | Soma de Minecraft Season Pass Price por Plan | Cartão **Minecraft Season Pass** (`G35` usa `GETPIVOTDATA`) |

<img width="1864" height="757" alt="image" src="https://github.com/user-attachments/assets/f6e32bec-7147-42d5-af56-ebbd66d114f6" />
