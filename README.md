# Campanhas Service EprofessionalTi
##### v1.0

&nbsp;
### Uso

Você encontrará um exemplo físico [aqui](https://github.com/angeloevangelista/exemplo-api-campanhas/blob/master/exemplo.html)

```javascript
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
    <script type="text/javascript">

    const tempoEp='2';
    const tamanhoEp='1';
    const categoriaEp = 'saude';
    const containerIdEp ='campanha-container';

        (function () {
            var s1 = document.createElement("script"), s0 = document.getElementsByTagName("script")[0];
            s1.async = true;
            s1.src = `https://www.eprofessionalti.com/api/scripts/campanhas?container=${containerIdEp}&tempo=${tempoEp}&tamanho=${tamanhoEp}&categoria=${categoriaEp}`;
            s0.parentNode.insertBefore(s1, s0);
        })();
    </script>
```

Para carregar as propagandas é necessário incluir este trecho de código [JavaScript](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript) no topo da sua página [HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML).

&nbsp;
### Parâmetros

Note que no trecho de código há algums parâmetros:

``` javascript
    const tempoEp='2';
    const tamanhoEp='1';
    const categoriaEp = 'saude';
    const containerIdEp ='campanha-container';
```

Abaixo está uma tabela de definição com os detalhes:

|   Parâmeto  | Tipo    | Obrigatório            | Valor Padrão
| ----------- |---------| ---------------------- | -------
| tempoEp       | int     |                        | <center>```20```</center>
| tamanhoEp     | int     |                        | <center>```1```</center>
| categoriaEp   | string  |                        | <center>```saude```</center>
| containerIdEp | string  |<center>**Sim**</center>| <center>```undefined```</center>

&nbsp;
### Descrição

```containerIdEp``` : Define o [ID](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Global_attributes/id) do elemento que receberá a campanha.
&nbsp;

```categoriaEp``` : Define a categoria das campanhas que serão exibidas. Ex. ```saude```, ```social```. Ainda em prototipação!
&nbsp;

```tempoEp``` : Intervalo, em segundos, de atualização das campanhas.
&nbsp;

```tamanhoEp``` : Define o tamanho da imagem que será renderizada. Intervalo de 1 a 4.
&nbsp;

 #### Tamanhos

 | Tamanho | Resolução |
 | ------- | --------- |
 | 1       | 720x90    |
 | 2       | 420x350   |
 | 3       | 262x90    |
 | 4       | 524x90    |
