# desafio-target
___

- Questão 1 - O valor da variável é 65.

- Questão 2
  - a- Caso a sequencia seja de números ímpares, o elemento faltante é 9, caso seja referente a sequencia de números primos, é 11
  - b- O elemento faltante é 128. N_(i) = 2 * N_(i-1) 
  - c- O elemento faltante é 49. O próximo elemento é a soma do item anterior com o número ímpar atual da sequência.
  - d- O elemento faltante é 100. O proximo elemento é a soma do item anterior com o número ímpar atual da sequência vezes o número 4.
  - e - O elemento faltante é 13, pois é a sequência fibonacci. N_(i+1) = N_(i) + N_(i-1) considerando i diferente de 0 e 1
  - f - O elemento faltante é o 200, pois a sequência é formada por números que começam com D.
  
- Questão 3
```python
def calculaInformacoesFaturament(vetor_faturamento_ano):
  faturamento_minimo = math.Infinity
  faturamento_maximo = -math.Infinity
  dias_faturados = 0
  somatorio_faturamento
  for faturamento_dia in vetor_faturamento_ano:
    if (faturamento_dia == 0):
      continue
    if (faturamento_dia > faturamento_maximo):
      faturamento_maximo = faturamento_dia
    elif (faturamento_dia < faturamento_minimo):
      faturamento_minimo = faturamento_dia
    dias_faturados = dias_faturados + 1
    somatorio_faturamento = somatorio_faturamento + faturamento_dia
  media_faturamento = somatorio_faturamento * 1.0 / dias_faturados 
  
  return (faturamento_minimo, faturamento_maximo, media_faturamento)
```

- Questão 4

![diagrama Teste equipe Fiscon drawio](https://github.com/user-attachments/assets/22258573-0359-4a3c-baaa-dfd57418a3c8)

- Questão 5

Depende do posicionamento dos pedágios. Considerando que os pedágios estão igualmente distribuídos no trajeto, então quando ambos os veículos se cruzarem na pista, eles estarão mais próximos de Barretos. Considerando que os 3 pedágios estão mais próximos de Barretos que de Ribeirão preto, então, ambos os veículos estarão mais próximos de Ribeirão Preto.

A lógica foi a seguinte, o carro gasta 1.38 horas em seu trajeto sem o tempo dos pedágios, e 1.63 horas considerando o tempo dos pedágios, enquanto que o caminhão gasta ~1.56 horas no percurso. Cada 5 minutos, convertido em horas, representa 0.08 horas, logo, o carro atrasa seu percurso em um tempo maior que o do caminhão caso ele passe dos 3 pedágios. Logo, a única situação que o Caminhão esteja mais perto de seu destino é quando o carro já passou pelos 3 pedágios.
