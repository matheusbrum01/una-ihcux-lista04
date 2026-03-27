# ⚠️ Tratamento de Erros com try-catch em C#

## 📌 Descrição

Este documento explica o conceito de **tratamento de exceções** em C# utilizando `try-catch`, e como ele se relaciona com a **Prevenção de Erros**, uma das heurísticas de usabilidade de Nielsen.

---

## 🧠 O que é try-catch?

O `try-catch` é uma estrutura utilizada para **capturar e tratar erros (exceções)** que podem acontecer durante a execução do programa.

### 🔧 Estrutura básica:

```id="ex1"
try
{
    // Código que pode gerar erro
}
catch (Exception ex)
{
    // Tratamento do erro
    Console.WriteLine("Ocorreu um erro: " + ex.Message);
}
```

---

## ❌ O que acontece sem try-catch?

Sem o uso de `try-catch`, quando ocorre um erro:

* O programa pode **crashar (parar de funcionar)**
* O usuário vê mensagens confusas
* A experiência fica ruim

---

## ✅ Benefícios do try-catch

* Evita que o programa quebre
* Permite mostrar mensagens amigáveis
* Ajuda a identificar problemas
* Torna o sistema mais seguro e estável

---

## 🎯 Relação com a Heurística de Nielsen

### 🛡️ Prevenção de Erros

Essa heurística diz que:

> O sistema deve ser projetado para evitar erros antes que eles aconteçam ou lidar com eles de forma adequada.

---

## 🔗 Conexão entre try-catch e Prevenção de Erros

O `try-catch` contribui diretamente para essa heurística porque:

* ⚠️ **Intercepta erros antes que afetem o usuário**
* 💬 **Exibe mensagens claras ao invés de falhas técnicas**
* 🔄 **Permite que o sistema continue funcionando**
* 🧩 **Facilita a correção de problemas**

---

## 💻 Exemplo prático

```id="ex2"
try
{
    Console.Write("Digite um número: ");
    int numero = int.Parse(Console.ReadLine());

    Console.WriteLine("Você digitou: " + numero);
}
catch (FormatException)
{
    Console.WriteLine("Erro: Digite apenas números válidos.");
}
```

---

## 📚 Conclusão

O uso de `try-catch` é essencial para criar aplicações mais robustas e amigáveis.

Além de evitar falhas, ele melhora a experiência do usuário ao lidar com erros de forma controlada e compreensível, alinhando-se diretamente com o princípio de **Prevenção de Erros**.

---

## 👨‍💻 Autor

Desenvolvido por **Matheus Brum**

