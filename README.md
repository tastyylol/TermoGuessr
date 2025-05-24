# Ajuda para Termo

**Ajuda para Termo** é uma ferramenta web simples e leve para auxiliar jogadores do *Termo* — uma versão em português do popular jogo de palavras *Wordle*. A aplicação ajuda a filtrar e encontrar possíveis palavras baseadas nas pistas que o jogador obtém durante o jogo, facilitando a próxima tentativa.

---

## 📝 Descrição

*Termo* é um jogo de adivinhação de palavras onde o jogador deve descobrir uma palavra de 5 letras em até 6 tentativas. Para isso, o jogo dá dicas sobre quais letras estão na posição correta (verde), quais letras existem na palavra mas não na posição correta (amarelo) e quais letras não existem na palavra (cinza).

Esta ferramenta foi criada para facilitar o raciocínio do jogador, permitindo que ele informe as letras corretas, letras em posições erradas e letras proibidas, e receba sugestões de palavras que atendem a esses critérios.

---

## 🌟 Funcionalidades

- Entrada intuitiva para letras nas posições corretas (verde).
- Entrada para letras que estão na palavra, mas em posições erradas (amarelo).
- Campo para letras que não devem estar na palavra (cinza).
- Busca instantânea no dicionário de palavras de 5 letras.
- Filtro que considera acentos para a língua portuguesa.
- Interface limpa, responsiva e amigável.
- Lista de sugestões atualizada a cada busca.
- Previne busca sem nenhum filtro para evitar resultados excessivos.

---

## 🚀 Como usar

1. Clone ou baixe este repositório.
2. Certifique-se de que está executando um servidor local (por exemplo, `python3 -m http.server`) para evitar problemas de CORS no navegador.
3. Abra o arquivo `index.html` no navegador (ou acesse a versão online, link abaixo).
4. Preencha os campos:
   - Letras na posição correta (verde)
   - Letras em posições erradas (amarelo)
   - Letras proibidas (cinza)
5. Clique em "Buscar" para obter uma lista de palavras que correspondem aos critérios.
6. Utilize as sugestões para facilitar sua próxima jogada em *Termo*.

---

## 🔧 Detalhes técnicos

- **Carregamento das palavras:** O arquivo `database.txt` contém uma lista de palavras de 5 letras, uma por linha, carregadas via fetch API.
- **Filtragem:** O sistema utiliza expressões regulares para filtrar posições corretas e aplica regras para letras em posições erradas e proibidas.
- **Remoção de acentos:** Para facilitar a comparação, as letras são normalizadas removendo acentos, garantindo correspondência correta mesmo que o usuário não digite acentos.
- **Validação:** A busca é bloqueada se não houver nenhuma entrada, evitando retorno de todas as palavras.
- **Estilo:** Layout moderno e responsivo, com cores inspiradas no tema do jogo Wordle/Termo.

---

## 🌐 Acesso online

Você pode acessar a ferramenta online hospedada via GitHub Pages:

[https://tastyylol.github.io/TermoGuessr/](https://tastyylol.github.io/TermoGuessr/)

---

## 💡 Possíveis melhorias futuras

- Implementar backend para esconder o dicionário de palavras e evitar exposição direta.
- Adicionar suporte para diferentes tamanhos de palavras.
- Criar histórico de buscas e jogadas para análise posterior.
- Interface multilíngue.
- Suporte para mobile com aprimoramentos de usabilidade.

---

## 🙌 Contribuições

Contribuições são bem-vindas!  
Sinta-se à vontade para abrir issues, sugerir melhorias ou enviar pull requests.
