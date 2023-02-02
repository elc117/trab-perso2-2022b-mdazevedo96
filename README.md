# Pattern Matching em Haskell

## Introdução
Neste trabalho será apresentado uso de Pattern Matching em Haskell
> Link no Replit: https://replit.com/@Marcelo-Da-Silv/Pattern-Matching#patternmatching.hs

O **Pattern Matching** (correspondência de padrões) é uma das formas de construção sintática presente em Haskell. Por meio dele alguns padrões podem ser especificados, verificados e adequados, se houver necessidade. Com isso, economiza-se recursos computacionais durante a execução do código.
Deve-se utiliza-se dentro de funções e adequa-se a qualquer tipo de dado (numéricos, char's, listas, tuplas, etc). Isso leva a construção de um código simples, organizado e legível. 

## Desenvolvimento

### Onde podemos aplicar Pattern Matching?

Existem vários exemplos de uso de pattern matching em Haskell, aqui estão alguns:

1. Cálculo de um número fatorial

A função **factorial** usa pattern matching para selecionar o caso especial quando o **argumento é igual a zero**, no qual resulta em 1. Para os demais valores de **n**, a função é chamada recursivamente com **n-1**.

![Captura de tela_20230202_000644](https://user-images.githubusercontent.com/42869269/216221786-89d63b37-ad75-47ea-9967-6e192167e40b.png)

**OBS: (Eq p, Num p) => p -> p significa que p deve ser um tipo que seja tanto comparável quanto numérico. Isso é necessário porque a função usa o operador == para comparar 0 e o operador * para calcular o produto.**

![Captura de tela_20230201_234912](https://user-images.githubusercontent.com/42869269/216219182-93e21ef2-b9b8-488e-ae7d-ded2c6147ad3.png)


Fonte: Trecho do código patternmacthing.hs
 
 ![Calculadora fatorial](https://user-images.githubusercontent.com/42869269/216217474-db67c7a5-524b-4321-8540-72c19316e968.png)
 
 
## Exercícios aplicados em práticas de Haskell
  ![Captura de tela_20230202_004948](https://user-images.githubusercontent.com/42869269/216227130-b0727781-eae7-4b2b-a6c5-2e06a22b68f4.png)

    
  A solução empregada para o problema foi a seguinte:
  
  
  ![image](https://user-images.githubusercontent.com/42869269/216227584-137082fa-cfb3-4c10-9af1-00061fa7eb5f.png)
  

   A temperatura que nos importa são apenas aquelas **maiores que 37.8 graus** então, ocorre um desperdício de recursos computacionais e por conseguinte, o aumento do  tempo de execução do código. Dessa forma, o pattern matching reduz esse impacto à aplicação.
   
   **Reformulando o código com Pattern Matching
   
   ![Captura de tela_20230202_013059](https://user-images.githubusercontent.com/42869269/216232126-6c4d85af-89cf-4576-84c4-ce167549b890.png)

  
  **OBS: Podemos notar um elemento diferente no código...**
  
  O Pattern Matching utiliza-se de **guardas** em Haskell
  
  **Guardas em Haskell são uma forma de condicionar a execução de uma função baseada em uma condição. Elas são escritas após o nome da função e antes dos casos de pattern matching.**
  
  
  ![image](https://user-images.githubusercontent.com/42869269/216231003-e2a9c814-1456-4246-9fab-c37604e09c8c.png)


 

 ### Comparando
 
 ![Captura de tela_20230202_010927](https://user-images.githubusercontent.com/42869269/216229591-b06a576e-68b7-4c1c-a19c-13d40828b00d.png)
 
 ![Captura de tela_20230202_011219](https://user-images.githubusercontent.com/42869269/216229924-998269c0-3a50-42b5-bb5a-00081ebcd66a.png)

 
 


## Conclusão
Segundo a litetura, não há uma resposta exata quanto a economia computacional promovida com o emprego de Pattern Matching em códigos em Haskell pois, depende de outros fatores como, complexidade do algoritmo, tamanho dos dados de entrada, finalidade etc.
É necessário avaliar caso a caso para determinar se o seu caso é apropriado e ofecere benefícios para resolução do problema.
Por reduzir a complexidade da legibilidade para os desenvolvedores, auxilia na melhor compreensão nos códigos desenvolvidos


## Créditos

> http://learnyouahaskell.com/syntax-in-functions#pattern-matching
