# 歌で読む — Leia japonês através da música

Site estático para aprender a ler hiragana/katakana/kanji sílaba por sílaba, com romanji 
embaixo, usando letras de música.


## Formato do texto (usado na caixa de edição e nos .txt)

Cada sílaba é escrita assim: `texto[romanji]`

- **Hífen `-`** separa sílabas dentro da mesma palavra.
- **Espaço** separa palavras.
- **Linha em branco** cria uma quebra/respiro na letra.

Exemplo:

```
正[tada]-し[shi]-さ[sa] と[to] は[wa] 愚[oro]-か[ka]-さ[sa] と[to] は[wa]
```

Isso renderiza como caixinhas: em cima o kanji/kana, embaixo o romanji, agrupadas por
palavra (sublinhado vermelho por baixo de cada palavra).

## Importar / exportar .txt

- **Importar**: aceita um `.txt` só com uma música (o título vira o nome do arquivo),
  ou vários `.txt` de uma vez.
- **Várias músicas em um único arquivo**: separe cada música com uma linha
  `## Título da música`, por exemplo:

```
## Música 1
正[tada]-し[shi]-さ[sa] と[to] は[wa]

## Música 2
紙[kami]-一[ichi]-重[e] な[na] ん[n] だ[da]
```

- **Exportar música atual**: baixa só a letra selecionada.
- **Exportar todas**: baixa um único `.txt` com todas as músicas da sua biblioteca,
  já no formato `## Título` acima — dá pra importar de volta depois (em outro
  navegador/computador, por exemplo).

Tudo fica salvo automaticamente no `localStorage` do navegador, então a biblioteca
persiste entre visitas sem precisar de backend.

## Modo de prática

O botão **"esconder romanji"** borra o romanji de todas as sílabas — clique em uma
sílaba individual para revelar só ela, ótimo para treinar leitura sem depender da
romanização.
