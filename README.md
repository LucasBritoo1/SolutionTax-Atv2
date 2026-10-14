# Tax Solution ApK

Ferramenta de apoio à organização dos dados do **Imposto de Renda**, criada no **Excel (versão web)**, com navegação lateral, formulários de preenchimento e uma identidade visual própria.

> Todos os dados que aparecem nas imagens e na planilha de exemplo são **fictícios**, criados apenas para demonstração.

---

## Sobre o projeto

O objetivo é reunir em um só arquivo as informações que normalmente são necessárias na hora de declarar o Imposto de Renda: dados pessoais, saldos bancários e entradas de receita. A planilha foi pensada para ser simples de preencher, com um menu lateral que leva o usuário de uma etapa à outra.

## Identidade visual

- Logo criada para o projeto: um hexágono com circuitos e um **check verde**, passando a ideia de tecnologia e de declaração conferida.
- Paleta: azul-marinho `#0F1F3D`, ciano `#22D3EE` e verde `#2EE6A6`.
- Menu lateral escuro com a logo no topo e os itens **Titular**, **Informes** e **Notas**.

## Estrutura da planilha

A ferramenta tem três telas, uma para cada etapa do preenchimento.

### 1. Dados do Titular

Formulário com os dados da pessoa física:

- Nome, CPF, data de nascimento e título de eleitor
- Cônjuge
- Endereço (rua, rua abreviada e CEP)
- Telefone, celular e e-mail
- Perguntas de resposta rápida: houve alterações desde a entrega anterior, dependente cônjuge e residente no exterior

### 2. Informes de Rendimentos Bancários

Área para cadastrar os dados atuais de cada banco:

- Nome do banco
- Valor atual
- Anexo (nome do arquivo do informe, em PDF)
- Campo **TOTAL**, que soma os valores informados nos bancos

### 3. Notas Bancárias ou Extrato de Holerites

Tabela de **entradas** mês a mês, com as colunas:

- **Data**
- **Categoria** (por exemplo, holerite)
- **Valor**

A tabela tem filtros nos cabeçalhos para facilitar a consulta.

## Como usar (passo a passo)

1. Abra o arquivo `.xlsx` no Excel (versão web ou desktop).
2. No menu lateral, clique em **Titular** e preencha os campos em azul-claro com os seus dados.
3. Clique em **PRÓXIMO ->** (ou em **Informes** no menu) para ir à segunda tela.
4. Em **Informes**, preencha o banco, o valor atual e o nome do anexo de cada instituição. O **TOTAL** é calculado automaticamente.
5. Clique em **PRÓXIMO ->** para abrir a tela de **Notas**.
6. Registre cada entrada de receita com data, categoria e valor.
7. Use **<- ANTERIOR** a qualquer momento para voltar e corrigir informações.

## Como o projeto foi construído

1. **Layout fixo:** altura das linhas definida manualmente, para que o logo e o menu não se desloquem ao editar as células.
2. **Menu lateral:** coluna escura com a logo no topo e os itens de navegação.
3. **Uma aba por etapa:** Titular, Informes e Notas, cada uma com título, faixa de instrução e área de preenchimento.
4. **Navegação por links:** os botões **PRÓXIMO ->** e **<- ANTERIOR** e os itens do menu levam às outras telas.
5. **Campos de preenchimento destacados** em azul-claro, para o usuário saber onde digitar.
6. **Total automático** nos informes bancários, com a fórmula de soma.
7. **Tabela com filtros** na tela de notas.

## Tecnologias e ferramentas

- Microsoft Excel (versão web)
- Formas e imagens do Excel para o menu e a logo
- SVG e PNG para a criação da logo
- Git e GitHub para versionamento e publicação

## Imagens do projeto

Adicione aqui as capturas de tela das três telas (salve-as em uma pasta `imagens/`):

```md
![Dados do titular](imagens/titular.png)
![Informes bancários](imagens/informes.png)
![Notas e holerites](imagens/notas.png)
```

## Próximos passos

- [ ] Calcular automaticamente o total de entradas na tela de notas
- [ ] Adicionar uma tela de resumo com o total de rendimentos e bancos
- [ ] Incluir lista de categorias de receita para escolha
- [ ] Proteger as células de layout, liberando apenas os campos de preenchimento
- [ ] Criar uma versão com cálculo estimado do imposto

## Aviso

Esta ferramenta é um projeto de estudo e **não substitui** o programa oficial da Receita Federal nem a orientação de um contador. Não publique no repositório planilhas com dados pessoais reais (CPF, endereço, valores).

## Autor

**Lucas Brito**
GitHub: [@LucasBritoo1](https://github.com/LucasBritoo1)
