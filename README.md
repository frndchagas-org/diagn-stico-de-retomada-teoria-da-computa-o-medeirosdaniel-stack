# Diagnóstico de retomada - Teoria da Computação

Esta atividade serve para mapear o que você já domina sobre linguagens formais, autômatos, gramáticas e computabilidade.

Responda individualmente. Use suas palavras. Se usar IA depois da primeira tentativa, registre o uso na seção 7.

## 1. Mapa do que eu lembro

Marque cada tópico como: lembro bem, lembro parcialmente, não lembro, nunca vi ou não tenho certeza.

- alfabeto: `lembro bem`
- cadeia:`lembro parcialmente`
- linguagem:`lembro parcialmente`
- gramática:`lembro parcialmente`
- autômato finito:`lembro parcialmente`
- linguagem regular:`lembro parcialmente`
- linguagem livre de contexto: `não lembro`
- linguagem sensível ao contexto: `não lembro`
- linguagem irrestrita: `não lembro`
- hierarquia de Chomsky: `não lembro`
- computabilidade: `não lembro`
- máquina de Turing: `não lembro`

## 2. Definições com exemplo

Explique, com suas palavras e com um exemplo simples, usando o alfabeto `Sigma = {a, b}`.

1. O que é um alfabeto? `É um conjunto finito e não vaziu de simbolos, repesentado pelo sigma`
2. O que é uma cadeia? `É uma sequência finita de simbolos de uma alfabeto`
3. O que é uma linguagem? `É um conjunto de cadeias possiveis de do alfabeto`
4. O que é uma gramática? `É o conjunto de regras que devem ser seguidas para construir cadeias de uma linguagem`

## 3. Linguagens

Considere as linguagens:

```text
L1 = { w em {0,1}* | w termina com 01 }
L2 = { a^n b^n | n >= 0 }
L3 = { a^n b^n c^n | n >= 0 }
```

Para cada linguagem:

1. escreva três palavras que pertencem à linguagem;
 `L1 = {01,001,101}, L2 = {vaziu, ab,aabb}, L3 = {vaziu, abc,aabbcc}`  
2. escreva duas palavras que não pertencem;
`L1 = {10,0011}, L2 = {abb,aab}, L3 = {ac,aabc}`
3. diga, se souber, em qual classe ela provavelmente se encaixa;
`não sei`
4. explique o motivo em linguagem simples.
`Não sei como classificar a qual clase pertence`
Não há problema em dizer "não sei". Nesse caso, escreva o que te deixou em dúvida.

## 4. Autômato finito

Considere o autômato abaixo, sobre o alfabeto `{0,1}`:

```text
Estados: q0, q1, q2
Estado inicial: q0
Estado final: q2

Transições:
q0 --0--> q1
q0 --1--> q0
q1 --0--> q1
q1 --1--> q2
q2 --0--> q1
q2 --1--> q0
```

Responda:

1. Qual linguagem esse autômato parece reconhecer? `L={w∈{0,1}∗∣w termina com 01}`
2. Execute manualmente as cadeias abaixo e diga se aceita ou rejeita:
   - `01` - `aceita`
   - `101` - `aceita`
   - `100` - `rejeita`
   - `1101` - `aceita`
   - `111` - `rejeita`
3. Monte uma tabela curta mostrando o caminho dos estados para pelo menos duas cadeias.
```
Cadeia 101
| Símbolo | Estado atual | Próximo estado |
| ------- | ------------ | -------------- |
| início  | q0           | q0             |
| 1       | q0           | q0             |
| 0       | q0           | q1             |
| 1       | q1           | q2             |

Cadeia 100
| Símbolo | Estado atual | Próximo estado |
| ------- | ------------ | -------------- |
| início  | q0           | q0             |
| 1       | q0           | q0             |
| 0       | q0           | q1             |
| 0       | q1           | q1             |

```
## 5. Gramática

Considere a gramática:

```text
S -> aS
S -> b
```

Responda:

1. Gere cinco cadeias produzidas por essa gramática.`não sei como identificar a regra de criação`
2. Descreva a linguagem em palavras. `não sei descrever ela  `
3. Essa gramática parece regular, livre de contexto ou outra classe? Justifique de forma simples.`não sei`

## 6. Ponto de dificuldade

Escolha um tópico da lista inicial e escreva: `Autômato finito`

1. o que você entende dele;`autômo finito é usado quando é feita uma comparação simples, sem necessidade de comparação em armazenamento, fezendo uma checagem se o objeto é igual a regra da cadeia`
2. onde você se confunde;`Na parte das transições`
3. que tipo de explicação ajudaria: desenho, exemplo, exercício guiado, analogia, prova passo a passo ou lista curta.
`exercício guiado`
## 7. Uso de IA, se houver

Se você usou IA depois da primeira tentativa, registre:

```text
Pergunta feita:  Qual linguagem esse autômato parece reconhecer?
Resumo da resposta: me deu a forma de construção; 
Como eu verifiquei: observei que seguia a forma de transição
O que eu alterei na minha resposta: não sabia responder
O que ainda não entendi: como usar as forma de transição para criar a regra da linguagem
```

## Submissão no Moodle

Depois de finalizar, copie no Moodle:

```text
Repositório:
Commit final:
Autoavaliação: nível atual, maior dificuldade e tópico que precisa ser retomado.
```
