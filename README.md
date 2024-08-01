# Sistema-de-consulta-de-b-nus-dos-funcion-rios.
Criando um sistema de consulta de bônus dos funcionários


- Pegar o valor de vendas do funcinoário por meio de um input
- Calcular o bônus do funcionário de acordo com a seguinte regra:
      - Se o funcionário vendeu mais de 1000 unidades, ele ganha R$2 de bonus para cada unidade vendida
      - Se o funcionário vendeu mais de 5000 unidades, ele ganha R$2 de bônus para cada unidade + um valor fixo de R$1000
      - Se o funcionário vendeu menos de 1000 unidades, ele não ganha bônus
- Printar no final o valor do bônus do funcionário


vendas = float(input("Digite as unidades vendidas (apenas números):"))
if vendas > 5000:
    bonus = vendas * 2 + 1000
elif vendas > 1000:
    bonus = vendas * 2
else:
    bonus = 0
print(f"Bônus {bonus}")
