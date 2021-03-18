# Variáveis

- Não é <strong>CASE-SENSITIVE</strong>;
- Podem ser utilizadas chaves (<strong>RECOMENDADO</strong>).

```bash
IDADE=22
NOME=Matheus
NOME_COMPLETO='Matheus Lopes Vivas'

echo $NOME tem $IDADE anos
echo ${NOME_COMPLETO}

echo $NOME
echo NOME
```

- Não pode haver espaços na definição de variáveis;

- echo $NOME printa o valor da variável NOME;
- echo NOME printa a palavra NOME;

- NOME e IDADE são variáveis de shell, não poderão ser usadas em conjunto com um arquivo, por exemplo:

```txt
Nome do Arquivo texto: nome_idade

echo $NOME tem $IDADE anos.
```

- Para que esse arquivo possa usar as variáveis criadas, é necessário exportá-las;
- Após a exportação, são variáveis de ambiente.

```bash
export NOME
export IDADE
bash nome_idade
```

- Para listar as variáveis de ambiente, basta digitar <strong>env</strong>, de environment.

```bash
env NOME=Ana IDADE=26 bash nome_idade
Resulta em: Ana tem 26 anos

echo $NOME
Resulta em: Matheus
```

- Variáveis NOME e IDADE foram alteradas somente nesse novo env, mas os valores originais continuam os mesmos de antes;

- Para deixar de exportar: export -n
- Para deixar de exportar remover uma variável do shell: unset

```bash
export -n VARIAVEL
unset VARIAVEL
```

______________

## PS1

- PS1 Linux configuration;
- Substitui o <strong>usuario@nome_do_computador</strong> pelo valor indicado;
- \u indica o usuário;
- \w indica o diretório.

```bash
PS1='$ '
PS1='\u@\w: '
```

## PS2

- Indicador de quebra de linha (>).

```bash
echo 'teste teste teste
> teste teste'
```