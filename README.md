# Estagio_Ribeirao_Preto_2024
Desafio técnico Respostas

## 1) Ao final do processamento, qual será o valor da variável SOMA?

O valor da variável SOMA ao final do processamento será 91. Isso ocorre porque o código está somando todos os números de 1 até 13. 
Então, a soma seria 1 + 2 + 3 + ... + 13, que é igual a 91.

## 2) Esse número pode ser informado através de qualquer entrada de sua preferência ou pode ser previamente definido no código;

```
def verifica_fibonacci(numero):
    a, b = 0, 1
    while b < numero:
        a, b = b, a + b
    if b == numero:
        return True
    else:
        return False

numero_informado = int(input("Digite um número para verificar se pertence à sequência de Fibonacci: "))

if verifica_fibonacci(numero_informado):
    print(f"O número {numero_informado} pertence à sequência de Fibonacci.")
else:
    print(f"O número {numero_informado} não pertence à sequência de Fibonacci.")
```

## 3) Descubra a lógica e complete o próximo elemento:

a) 1, 3, 5, 7, **9**

b) 2, 4, 8, 16, 32, 64, **128**

c) 0, 1, 4, 9, 16, 25, 36, **49**

d) 4, 16, 36, 64, **100**

e) 1, 1, 2, 3, 5, 8, **13**

f) 2, 10, 12, 16, 17, 18, 19, **20**

## 4) Como você faria para descobrir, usando apenas duas idas até uma das salas das lâmpadas, qual interruptor controla cada lâmpada?

Primeiro, eu ligaria um interruptor e esperaria alguns minutos. Em seguida, desligaria esse interruptor e ligaria outro. Eu entraria na sala e verificaria qual lâmpada está acesa. Se estiver acesa, o interruptor que liguei inicialmente controla aquela lâmpada. Se estiver apagada, tocaria a lâmpada para sentir se está quente. Se estiver, o interruptor que liguei primeiro controla aquela lâmpada; caso contrário, o interruptor desligado inicialmente controla a lâmpada. O terceiro interruptor controla automaticamente a lâmpada restante. Dessa forma, descobriria qual interruptor controla cada lâmpada com apenas duas visitas a uma das salas das lâmpadas.

## 5) Escreva um programa que inverta os caracteres de um string.

```
def inverter_string(string):
    inverted_string = ''
    for i in range(len(string) - 1, -1, -1):
        inverted_string += string[i]
    return inverted_string

# Exemplo de uso
string_original = input("Digite uma string para inverter: ")
string_invertida = inverter_string(string_original)
print("String original:", string_original)
print("String invertida:", string_invertida)
```
