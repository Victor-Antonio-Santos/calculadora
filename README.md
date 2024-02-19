# calculadora
calculadora simples

x = True


while x == True:
    try:
        def soma(a,b):
            return a + b
        def subtracao(a,b):
            return a - b
        def divisao(a,b):
            if a != 0:
                return a / b 
            else:
                print('Erro. Divisão por 0')
        def multiplicacao(a,b):
            return a * b
    
        numero1 = int(input('Digite o primeiro numero: '))
    
        numero2 = int(input('Digite o segundo numero: '))

        opcao = input(''' 
[1] SOMA 
[2] SUBTRAÇÃO 
[3] DIVISÃO 
[4] MULTIPLICAÇÃO
Digite qual operação deseja realizar: ''')
        
        
        if opcao == '1':
            resultado1 = soma(numero1,numero2)
            print(resultado1)  
        elif opcao == '2':  
            resultado2 = subtracao(numero1,numero2)
            print(resultado2)
        elif opcao == '3':  
            resultado3 = divisao(numero1,numero2)
            print(resultado3)
        elif opcao == '4':  
            resultado4 = multiplicacao(numero1,numero2)
            print(resultado4)
        else:   
            print('Opção invalida!')
    except:
        print('Por favor digite apenas numeros!')
        continue
