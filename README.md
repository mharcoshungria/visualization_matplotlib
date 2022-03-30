<img src="https://i.imgur.com/YX6UATs.png"  width="160">

# Visualização de Dados com Matplotlib

## Considerações iniciais

O objetivo deste notebook é fazer com que o leitor assimile os recursos de uma das bibliotecas mais importantes do Python: o Matplotlib. Para isso, exemplos e conceitos desta biblioteca serão apresentados ao longo da jornada. Concomitantemente, serão solicitadas algumas tarefas práticas ao leitor.

### Por que o Matplotlib?
Apesar do Python possuir um ecossitema de feramentas de visualização muito rico para o cientista de dados, o Matplotlib, sem dúvidas, também detém seu lugar de destaque.

> "Matplolib tenta facilitar as coisas fáceis e tornar as coisas difíceis possíveis."
>
> [Site do Matplotlib](https://matplotlib.org/)

Além do Matplotlib, utilizaremos, também, um conjunto de dados e outras bibliotecas de apoio, como o [Pandas](https://pandas.pydata.org/), por exemplo. Afinal, o Matplotlib é ótimo, mas não brilha sozinho.

### Prepare seu ambiente

Se necessário, faça a instalação da biblioteca no seu sistema usando o gerenciador de pacotes da linguagem, no prompt/terminal/cmd digite:
```
$ pip install matplotlib
```

Ou caso esteja usando o Anaconda:
```
$ conda install matplotlib
```

### Conjunto de dados
O conjunto de dados utilizado são os registros de milhares de lutas no Ultimate Fight Championship (UFC). O arquivo [ufc.csv](https://github.com/mharcoshungria/visualization_matplotlib/blob/main/ufc.csv) possui mais de 145 colunas, o que é demasiadamente grande para as nossas intenções. Deste modo, iremos focar apenas uma parte dos dados.

#### Descrição do dados

De todas as colunas do arquivo [ufc.csv](https://github.com/mharcoshungria/visualization_matplotlib/blob/main/ufc.csv), iremos praticar com:
- R_fighter: Nome do lutador do canto vermelho.
- B_fighter: Nome do lutador do canto azul.
- Referee: Nome do árbitro da luta.
- date: Data do evento
- location: Local do evento.
- Winner: Cor do vencedor - Red ou Blue.
- title_bout: Se é uma disputa pelo título.
- weight_class: Classe de peso da luta.
