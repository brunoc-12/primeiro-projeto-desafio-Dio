# primeiro-projeto-desafio-Dio
## calculadora-de-notas 
# Calculadora de Notas

```python
notas = []
for i in range(2):
    nota = float(input(f'Digite a nota {i+1}: '))
    notas.append(nota)

with open('notas.txt', 'w') as arquivo:
    for nota in notas:
        arquivo.write(f"{nota}\n")

media = sum(notas)/len(notas)

if media >= 7:
    print(f'Parabéns! Você passou com média {media}')
else:
    print(f'Infelizmente, você não passou. Média: {media}')

