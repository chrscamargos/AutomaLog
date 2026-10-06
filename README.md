# Painel de Controle de Lotes Industriais

Atividade de Desenvolvimento Web Front-End, feita em React no componente `src/componentes/Contador/index.jsx`.

## Sobre

A AutomaLog usava um contador de caixas por palete que permitia lote negativo, passar de 50 caixas e perdia o valor do último lote ao zerar. Aqui o contador foi evoluído para um controle de lotes com regras que evitam esses erros.

## O que foi feito

- O contador fica sempre entre 0 e 50, e os botões ficam desabilitados quando a próxima ação passaria do limite.
- O fundo muda conforme o palete enche: azul até 39 caixas, amarelo/laranja a partir de 40 ("Capacidade quase atingida") e vermelho com o badge "Lote Fechado" em 50.
- O campo do passo aceita só de 1 a 10. Fora disso, ajusta para o limite mais próximo, e vazio volta para 1.
- O estado `ultimoLoteRegistrado` guarda o valor do lote ao clicar em "Zerar" e mostra na tela.

## Como rodar

```bash
npm install
npm run dev
```