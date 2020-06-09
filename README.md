# Campanhas Service EprofessionalTi
##### v1.0

&nbsp;
### Uso

```javascript
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
    <script type="text/javascript">

    const tempo='2';
    const tamanho='1';
    const categoria = 'saude'; 
    const containerId ='campanha-container';

        (function () {
            var s1 = document.createElement("script"), s0 = document.getElementsByTagName("script")[0];
            s1.async = true;
            s1.src = `http://www.eprofessionalti.com/api/scripts/campanhas?container=${containerId}&tempo=${tempo}&tamanho=${tamanho}&categoria=${categoria}`;
            s0.parentNode.insertBefore(s1, s0);
        })();
    </script>
```

Para carregar as propagandas é necessário incluir este trecho de código [JavaScript](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript) no topo da sua página [HTML](https://developer.mozilla.org/pt-BR/docs/Web/HTML).

&nbsp;
### Parâmetros

Note que no trecho de código há algums parâmetros:

``` javascript
    const tempo='2';
    const tamanho='1';
    const categoria = 'saude'; 
    const containerId ='campanha-container';
```

Abaixo está uma tabela de definição com os detalhes:

|   Parâmeto  | Tipo    | Obrigatório            | Valor Padrão
| ----------- |---------| ---------------------- | -------
| tempo       | int     |                        | <center>```20```</center>
| tamanho     | int     |                        | <center>```1```</center>
| categoria   | string  |                        | <center>```saude```</center>
| containerId | string  |<center>**Sim**</center>| <center>```undefined```</center>

&nbsp;
### Descrição

```containerId``` : Define o [ID](https://developer.mozilla.org/pt-BR/docs/Web/HTML/Global_attributes/id) do elemento que receberá a campanha. 
&nbsp;

```categoria``` : Define a categoria das campanhas que serão exibidas. Ex. ```saude```, ```social```. Ainda em prototipação!
&nbsp;

```tempo``` : Intervalo, em segundos, de atualização das campanhas.
&nbsp;

```tamanho``` : Define o tamanho da imagem que será renderizada. Intervalo de 1 a 4.
&nbsp;

 #### Tamanhos
 
 | Tamanho | Dimensões |
 | ------- | --------- |
 | 1       | 720x90    |
 | 2       | 420x350   |
 | 3       | 262x90    |
 | 4       | 524x90    |
 