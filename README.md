print('===[ Bem-Vindo ao Gamehub ]===')
print('# Para iniciarmos Digite seu nome #')

x = input('Qual é o seu nome bravo guerreiro(a)? : ')
y = int(input('Escolha um número de 1 a 100 para o NÍVEL: '))

if y <= 100:
    print('Nível criado')
    print('Salvando o Jogo...')
else:
    print('Escolha um número de 1 a 100 para continuar')

U = int(input('Escolha um número de 1 a 15 para a VIDA: '))
if U <= 15:
    print('Vida em criação')
    print('Salvando o Jogo...')
else:
    print('Escolha um número de 1 a 15 para continuar')

z = U  # vida

jogo = {
    'personagem': x,
    'nivel': y,
    'vida': z
}

print(jogo)

print('muito tempo depois...')

jogo['nivel'] = 100
del jogo['vida']

print('Sem uma vida, o jogo não pode continuar...')
print('===[ GAME OVER ]===')