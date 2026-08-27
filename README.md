# 🎮 Jogo da Forca (Hangman) — Terminal Edition

![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

Um clássico Jogo da Forca desenvolvido em **JavaScript**, executado diretamente no terminal com **Node.js**. O projeto utiliza o módulo nativo `readline/promises` para capturar a entrada do usuário de forma assíncrona, sem a necessidade de bibliotecas externas.

## 📋 Sobre o Projeto

Este projeto implementa a lógica completa do tradicional Jogo da Forca: o sistema sorteia uma palavra secreta de uma lista pré-definida, e o jogador deve tentar descobri-la letra por letra antes que suas tentativas (vidas) se esgotem.

O objetivo é praticar conceitos fundamentais de **lógica de programação**, **manipulação de arrays e strings**, **estruturas de repetição** e **programação assíncrona (async/await)** em Node.js.

## ✨ Funcionalidades

- 🔤 Sorteio aleatório de palavras a partir de uma lista pré-definida
- ⌨️ Entrada de letras via terminal, com conversão automática para maiúsculas
- 🔄 Atualização em tempo real do progresso da palavra (`_ _ _ _`)
- ❌ Feedback imediato para letras incorretas
- 🏆 Mensagem de vitória ao completar a palavra corretamente
- 💀 Controle de vidas/tentativas restantes

## 🛠️ Tecnologias Utilizadas

- [Node.js](https://nodejs.org/)
- Módulo nativo `readline/promises`
- JavaScript (ES6+)

## 📦 Pré-requisitos

Antes de começar, certifique-se de ter o [Node.js](https://nodejs.org/) (versão 14 ou superior) instalado em sua máquina.

```bash
node --version
```

## 🚀 Como Executar

1. Clone este repositório:
```bash
git clone https://github.com/MarcosvhGoncalves/Jogo-da-Forca
```

2. Acesse a pasta do projeto:
```bash
cd jogo-da-forca
```

3. Execute o jogo:
```bash
node index.js
```

## 🕹️ Como Jogar

1. Ao iniciar, o jogo sorteia automaticamente uma palavra secreta.
2. A palavra é exibida em forma de underlines (`_`), representando cada letra oculta.
3. Digite uma letra e pressione `Enter`.
4. Se a letra existir na palavra, ela será revelada em todas as posições correspondentes.
5. Se a letra não existir, uma vida é perdida.
6. O jogo termina quando a palavra é completamente descoberta ou caso perca todas as vidas.

## 📁 Estrutura do Código

O jogo é controlado pela função assíncrona `iniciarJogo()`, que segue o seguinte fluxo lógico:

| Etapa | Descrição |
|-------|-----------|
| 1. Sorteio | Uma palavra é escolhida aleatoriamente do array `palavras` |
| 2. Inicialização | Cria um array de underlines representando as letras ocultas |
| 3. Loop principal | Solicita letras ao jogador enquanto `jogoRodando` for `true` |
| 4. Verificação | Checa se a letra existe na palavra e atualiza o progresso |
| 5. Condição de vitória | Encerra o jogo quando não há mais underlines restantes |

## 🐞 Melhorias Futuras

Durante a análise do código, foram identificados alguns pontos de evolução para as próximas versões:

- [ ] Exibir visualmente a quantidade de vidas restantes a cada rodada (ex: `Vidas: ❤️❤️❤️❤️❤️❤️`).
- [ ] Impedir que a mesma letra seja contabilizada duas vezes como erro.
- [ ] Adicionar validação de entrada (impedir números, símbolos ou strings vazias).
- [ ] Exibir um desenho ASCII da forca de acordo com o número de erros.
- [ ] Permitir que o jogador escolha o nível de dificuldade (categorias de palavras).

## 🤝 Contribuindo

Contribuições são sempre bem-vindas! Sinta-se à vontade para abrir uma *issue* ou enviar um *pull request* com sugestões de melhoria.

1. Faça um fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/nova-feature`)
3. Faça o commit das suas alterações (`git commit -m 'Adiciona nova feature'`)
4. Faça o push para a branch (`git push origin feature/nova-feature`)
5. Abra um Pull Request


## 👤 Autor

Desenvolvido por **[Marcos Vinnicius]**.

- GitHub: [@MarcosvhGoncalves](https://github.com/MarcosvhGoncalves)
- LinkedIn: [Marcos Vinnicius Herculano Gonçalves](https://www.linkedin.com/in/marcosvhg/)

---

⭐️ Se este projeto foi útil para você, considere deixar uma estrela no repositório!