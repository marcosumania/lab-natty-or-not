
### Desenvolvimento de um SCRIPT MUSICAL

```markdown
# TDesenvolvimento de um SCRIPT MUSICAL

## 📒 Descrição
Definir as notas: A música ocidental é baseada em 12 semitons. Temos que mapear essas notas.

Encontrar a terça: Dependendo da tonalidade (maior ou menor), a terça será:

Terça maior: 4 semitons acima da tônica.
Terça menor: 3 semitons acima da tônica.
Entrada do usuário: O script precisa receber a nota da tônica e o tipo de terça (maior ou menor) como entrada.

Saída: A nota correspondente à terça.

## 🤖 Tecnologias Utilizadas
- IA Generativa **[ChatGPT](https://chat.openai.com)** para roteirização e revisão;

## 🧐 Processo de Criação
Interagindo junto ao CHATGPT solicitando o código.

## 🚀 Resultados
O Código gerado pela OPENAI está logo abaixo;

# Definimos as 12 notas da escala cromática
notas = ['C', 'C#', 'D', 'D#', 'E', 'F', 'F#', 'G', 'G#', 'A', 'A#', 'B']

def encontrar_terca(tonica, tipo_terca):
    # Localiza o índice da tônica na lista de notas
    if tonica not in notas:
        return "Tônica inválida!"
    
    indice_tonica = notas.index(tonica)
    
    # Determina quantos semitons são necessários para a terça
    if tipo_terca == 'maior':
        semitons = 4  # Terça maior é 4 semitons acima
    elif tipo_terca == 'menor':
        semitons = 3  # Terça menor é 3 semitons acima
    else:
        return "Tipo de terça inválido! Use 'maior' ou 'menor'."
    
    # Calcula o índice da terça com base na tônica
    indice_terca = (indice_tonica + semitons) % 12  # Usa o módulo 12 para circular nas notas
    
    # Retorna a nota correspondente
    return notas[indice_terca]

# Exemplo de uso
tonica = 'C'
tipo_terca = 'maior'
terca = encontrar_terca(tonica, tipo_terca)
print(f"A terça {tipo_terca} de {tonica} é {terca}")


## 💭 Reflexão (Opcional)
notas: A lista contém as notas cromáticas de uma oitava (de C até B).

encontrar_terca:

Recebe a tônica (como 'C', 'G#', etc.) e o tipo de terça ('maior' ou 'menor').
Calcula a posição da terça baseado nos semitons.
Retorna a nota da terça.
Exemplo de uso: Se a tônica for C e a terça for maior, o resultado será E.
```

### Desenvolvimento Finalizado

## Links Interessantes

[Base10: If You’re Not First, You’re Last: How AI Becomes Mission Critical](https://base10.vc/post/generative-ai-mission-critical/)

![Base10's Trend Map Generative AI](https://github.com/digitalinnovationone/lab-natty-or-not/assets/730492/f4df26e8-f8f7-4419-8252-c69d73ea930c)
