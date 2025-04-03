# Conceitos Básicos de Programação C# para Unity

<br>

## Variáveis
Espaço na memória que armazena um valor mutável.

### Tipos primitivos:
```csharp
int nomeVar = 10;       // Números inteiros
float nomeVar = 10.5f;  // Números decimais
bool nomeVar = true;    // Valores booleanos (true ou false)
string nomeVar = "texto"; // Texto
```

### Tipos exclusivos da Unity:
```csharp
GameObject nomeVar; // Referência a um objeto na cena
Transform nomeVar;  // Referência à transformação (posição, rotação, escala) de um objeto
```

Por padrão, variáveis são privadas. Para torná-las acessíveis publicamente:
```csharp
public int nomeVar;
```

## Métodos
Blocos de instruções que alteram valores de variáveis e executam ações.

Declaração:
```csharp
void NomeMetodo()
{
    // Instruções
}
```
O tipo de retorno pode ser `void` (nenhum valor) ou tipos como `int`, `bool`, etc.

## Classe
Agrupa variáveis e métodos, podendo ser usada em um ou mais objetos.
```csharp
public class NomeClasse : MonoBehaviour
{
    // Variáveis e métodos da classe
}
```

## Condicionais
### `if` e `else`
O if executa um bloco de código caso a condição especificada seja verdadeira. Caso contrário, o else será executado.
```csharp
if (condicao)
{
    Debug.Log("Mensagem no console");
}
else
{
    Debug.Log("Outra mensagem");
}
```

### `switch`
Alternativa ao `if` quando há múltiplas condições.
```csharp
switch (variavel)
{
    case valor1:
        // Comando
        break;
    case valor2:
        // Comando
        break;
    default:
        // Caso padrão
        break;
}
```

### Entrada do usuário (teclas)
```csharp
if (Input.GetKey(KeyCode.Space)) // Enquanto a tecla estiver pressionada
{
}
if (Input.GetKeyDown(KeyCode.Space)) // Quando a tecla for pressionada uma vez
{
}
if (Input.GetKeyUp(KeyCode.Space)) // Quando a tecla for solta
{
}
```

## Estruturas de Dados
### Array
Armazena múltiplos valores do mesmo tipo.
```csharp
public int[] arrayInt = {1, 2, 3, 4, 5};
```

### List
Semelhante ao array, mas mais flexível.
```csharp
public List<int> listaInt = new List<int>();
listaInt.Add(10);   // Adiciona elemento
listaInt.Remove(10); // Remove elemento
listaInt.Clear();   // Limpa todos os elementos
```

## Laços de Repetição
### `for`
Executa um bloco de código um número definido de vezes.
```csharp
for (int i = 0; i < 10; i++)
{
    // Instruções
}
```

### `foreach`
Percorre arrays ou listas.
```csharp
foreach (int valor in arrayInt)
{
    Debug.Log(valor);
}
```

## Atalho útil
Para comentar várias linhas ao mesmo tempo:
**Windows:** `Ctrl + K + C`
**Mac:** `Cmd + K + C`

---

