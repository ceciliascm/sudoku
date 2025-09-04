# 🧩 Jogo de Sudoku em Java

Este projeto implementa um **jogo de Sudoku** em Java, com menu interativo no terminal e regras básicas do jogo. Ele pode ser utilizado tanto para treinar lógica de programação quanto para praticar conceitos de **POO**, **persistência de estado** e **validação de regras de negócio**.  

📖 [O que é Sudoku?](https://pt.wikipedia.org/wiki/Sudoku)

---

## 🚀 Funcionalidades

O programa possui um **menu interativo**, que permite ao jogador:  

1. **Iniciar um novo jogo**  
   - O jogo inicial é carregado com números fixos informados via argumentos (`args`) do método `main`.  
   - Caso nenhum argumento seja informado, o tabuleiro começa vazio.  

2. **Colocar um novo número**  
   - Solicita do usuário: **coluna**, **linha** e **valor (1–9)**.  
   - Não é permitido sobrescrever números fixos do jogo.  

3. **Remover um número**  
   - Permite remover apenas números adicionados pelo jogador.  
   - Números fixos não podem ser removidos.  

4. **Visualizar o jogo atual**  
   - Mostra o tabuleiro atualizado com os números já inseridos.  

5. **Verificar status do jogo**  
   - Status possíveis:  
     - `Não iniciado`  
     - `Incompleto`  
     - `Completo`  
   - O status também informa se o jogo contém erros (valores duplicados na mesma linha, coluna ou bloco 3x3).  

6. **Limpar jogo**  
   - Remove apenas os números adicionados pelo usuário, mantendo os fixos.  

7. **Finalizar jogo**  
   - Caso o tabuleiro esteja completo e válido, exibe mensagem de vitória.  
   - Caso contrário, informa o que falta: posições vazias ou erros.  

8. **Sair**  
   - Encerra a execução do programa.  

---

## ⚙️ Estrutura do Projeto

O projeto segue uma divisão em **pacotes** para facilitar manutenção e clareza:  

- `br.com.dio.Main` → Classe principal com o menu interativo.  
- `br.com.dio.model.Board` → Representa o tabuleiro, contendo a lógica de verificação e manipulação.  
- `br.com.dio.model.Space` → Representa cada célula (espaço) do Sudoku.  
- `br.com.dio.util.BoardTemplate` → Template para exibir o tabuleiro de forma formatada.  

---

🛠️ Tecnologias Utilizadas
Java 17+ (compatível também com versões anteriores)

Paradigma de Programação Orientada a Objetos

Coleções (List, Map, Stream API)

Boas práticas de clean code e modularização

👨‍💻 Autor

Projeto criado como exercício prático para treino de lógica e POO em Java, baseado no curso da Digital Innovation One (DIO) GFT Start #7 - Java.
Cecília Costa.
