## **AULA 1- A tag form**

Na aula de número 1 vimos a respeito da tag form e alguns atributos dela, entre eles temos:

```html
<!-- O action envia os dados para determinado servidor -->

    <!-- Existe o method, nele possui duas possibilidades, o get e o post -->

    <!-- Get envia diretamente pro server -->

    <!-- O method POST encapsula a informação e envia -->

    <!-- Existe também o target, que funciona como uma forma de como redirecionar a informação -->

    <!-- O autocomplete serve para determinar se o browser vai ou não armazenar as credenciais -->

    <!-- O on(alguma coisa) indica uma ação, normalmente usado com javascript -->
```

---

---

## **AULA 2- A tag input**

Nessa aula, vimos as funcionalidades da tag input e alguns de seus atributos, entre eles temos:

```html
<form>
        <!-- No input temos o type, que indica o tipo de informação que deve ser inserido -->
        <label >Texto: </label><input type="text">
        <!-- O min e o max indica o máximo que pode ser colocado no campo de número -->
        <!-- O step serve para ir pulando o número de quantidade em quantidade -->
        <label>Número: </label><input type="number" min="0" max="99" step="2">
        <!-- O value indica o nome do elemento e mostra na tela -->
        <label>Button: </label><input type="button" value="Enviar"> <!-- ou --><button>Enviar</button>
        <label>Range: </label><input type="range" min="0" max="50" value="100">
         
        <label>Color: </label><input type="color"> 
        <!-- Indica uma forma de escolher uma cor -->
       <label>E-mail: </label><input type="email"> 

       <label>URL: </label><input type="url"> 

       <label>Date: </label><input type="date">
       
       <label>Week: </label><input type="week"> 
       <!-- Não funciona no Fire Fox -->
       <label>month: </label><input type="month">
       
       <!-- Também existe o checkbox e o radio -->
       <!-- Existe todas no w3b =schools -->
       <label>hidden: </label><input type="hidden"> 
       <!-- Hidden é um elemento booleano que indica se o elemento é ou não importante -->
       <label>file: </label><input type="file" multiple>
       <!-- Multiple serve para poder aceitar vários arquivos -->
       
       <label>search: </label><input type="search">
       <!-- Campo de pesquisa --> 
       
    </form>
```

## **AULA 3- As tags checkbox e radio**

Na aula 3, foi resolvido um problema comum do HTML, nele também, vimos o tratamento de variáveis dentro do HTML, veja mais:

```html
<h3>Faça o seu pedido de pizza:</h3>
    <form method="get">
        <!-- Exemplo de checkbox -->
        <label >Escolha os sabores da pizza: </label><br>
        <input type="checkbox" name="opcional[]" value="calabresa"><label>Calabresa</label><br>
        <input type="checkbox" name="opcional[]" value="queijo"><label>Queijo</label><br>
        <input type="checkbox" name="opcional[]" value="catupiri"><label>Catupiri</label><br>
        <input type="checkbox" name="opcional[]" value="carne-de-sol"><label>Carne-de-sol</label><br><br>
        <!-- O checkbox pode ser selecionado, já o radio, só pode ser escolhido uma única vez -->
        <!-- É necessário guardar as informações dos checkboxs na mesma variável(name) -->
        <!-- Se o checkbox for uma lista, é necessário pôr colchetes na frente do name para indicar que é uma lista -->

        <label>Borda Recheada?</label><br><br>
        <input type="radio" name="Borda"value="sim"><label>Sim</label><br>
        <input type="radio" name="Borda"value="não"><label>Não</label><br>
    </form>
```

## **AULA 4- Button e os seus tipos**

Na aula foram vistos os tipos de botões além de possíveis problemas de segurança que podem haver. Através da aula, foi aprendido que a validação pelo servidor é indispensável e alguns tipos de botões, entre eles temos:

```html
<form method="post">
        <label>Nome: </label><input type="text" name="name"><br>
        <label>Idade: </label><input type="number" name="age"><br>
        <label>Senha: </label><input type="password" name="password"><br>
        
        <button type="button" onclick="alert('Cliquei aqui')"> Clicável</button>

        <button type="reset">Limpar</button>

        <button type="submit">Enviar</button>

        <!-- Sempre aplicar uma validação do formulário -->

    </form>
```

## **AULA 5- Select e os seus tipos**

Na aula foi passado a tag Select, a qual já é auto explicativa. Em resumo, ela serve para pré-definir campos de escolha. Alguns exemplos:

```html
<form>
        <label>Nome: </label><input type="text" name="name"><br>
        <label>Cargo: </label>

        <!-- No select também existe o comando multiple -->
        <select name="role" id="">
            <option value="">Selecione o cargo</option>
            <option value="Front-end">Front-end</option>
            <option value="Back-end">Back-end</option>
            <option value="Full-Stack">Full-Stack</option>
            <option value="Designer">Designer</option>

        </select>
        <br>
        <label>Assunto: </label><input type="text" name="name"><br>

        <button type="submit">Enviar</button>
    </form>
```

## **AULA 6 - Textarea**

Nessa aula foi visto que a Textarea é uma simples área de texto adicional. Demonstração:

```html
<form>
        <label>Nome: </label><input type="text" name="name"><br>
        <label>Cargo: </label>

        <!-- No select também existe o comando multiple -->
        <select name="role" id="">
            <option value="">Selecione o cargo</option>
            <option value="Front-end">Front-end</option>
            <option value="Back-end">Back-end</option>
            <option value="Full-Stack">Full-Stack</option>
            <option value="Designer">Designer</option>

        </select>
        <br>
        <label>Assunto: </label><input type="text" name="name"><br>
        <!-- O textarea é uma área de texto maior do que o normal -->
        <!-- Os atributos rows e cols servem para definir a altura e a largura da área de texto -->
        <label >Mernsagem: </label><Textarea rows="2" cols="50"name="message"></Textarea>
        <button type="submit">Enviar</button>
    </form>
```

# 📝Módulo 7 ⇒ Estruturando o seu HTML

---

## Aula X ⇒

---

## **AULA 1- Formatando textos**

Na aula 1 foi visto alguns tipo de formatação, veja a seguir:

```html
<!-- Itálico -->
    <h2>Olá a <i><todos></i></h2>
    <!-- Negrito -->
    <h2>Olá a <b>todas</b></h2>
    <!-- Sublinhado -->
    <h2>Olá a <u>todos</u></h2>
    <!-- Marcar texto -->
    <h2>Olá a <mark>todos</mark></h2>
    <!-- Deixar o número com forma de potência -->
    <h2>Olá a <sup>todos</sup></h2>
    <!-- Deixar em forma de log -->
    <h2>Olá a todos <sub>de novo</sub></h2>
    <!-- Dar um espaçameto do texo aos outros -->
    <blockquote>Olá a todos</blockquote>
    <!-- O strong deixa o código em HTML mais semãntica -->
    <strong>Olá a todos</strong>

    <!-- A TAG FONT -->
    <font>Olá a todos</font>
    <!-- Atributos da tag font -->

    <!-- color -->

    <font color="red">Olá a todos</font>

    <!-- Face -->

    <font color="blue" face="Arial, Tahoma">Olá a todos</font>

    <!-- A tag font pode estar ficando em desuso devido ao CSS -->
```

## **AULA 2⇒ Div e Span**

Nessa aula foi visto que a tag Div e Span não servem para delimitar espaços, textos e etc. A tag Div separa um bloco de código deixando ele com display block e fazendo com que ele prencha todo o espaço da horizontal, veja mais:

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Estudando Div e Span</title>
</head>

<style>
    span{
        color: red;
        font-weight: bold;
    }
</style>
<body>
    <!-- Criando a planta do site -->
    <!-- Div e span são tags coringas de estruturação -->

    <!-- Exemplo de div -->
   <div class="Menu-lateral">
    <div class="content">
        <ul>
            <li><a href="#">Link 1</a></li>
            <li><a href="#">Link 2</a></li>
            <li><a href="#">Link 3</a></li>
        </ul>
    </div>
   </div>
   <!-- A div é display block e ocupa toda a horizontal da página -->
   <!-- Já a tag span não ocupa o espaço inteiro da pagina -->

   <!-- Ex: -->

   <p>Div pratice <div>.</div>mio</p>
   <p>Div pratice <span>.</span>mio</p>
   
</body>
</html>
```

## **AULA 3 ⇒Fieldsets**

Dessa vez, foi notado que as tags Fieldsets, servem, principalmente, para dar um aspecto visual mais harmônico e bonito. Além disso, elas vem acompanhadas da tag legend a qual serve para colocar o título da divisória. Veja mais:

```html
<style>
        .row{
            margin: 8px;
        }
        label{
            width: 100px;
            text-align: right;
            display: inline-block;
            padding-right: 5px;
        }
        fieldset{
            margin: 1rem;
            border-radius: 1rem;
            border: purple solid;
        }
    </style>
</head>
<body>
    <!-- Formulário de exemplo -->
    <form>
        <h1>Formulário de Cadastro</h1> <br>
        <fieldset>
            <legend>Dados pessoais</legend>
                <div class="row">
                    <label>Nome: </label> <input type="text" name="name">
                    <label>E-mail: </label> <input type="text" name="name"><br>

                <div class="row">
                    <label>Profissão: </label> <input type="text" name="name">
                    <label>Empresa: </label> <input type="text" name="name"><br>
                </div>
                    
                </div>
            
        </fieldset>
        <!-- O fieldset é um recurso visual de delimitação -->
       
        <fieldset>
            <legend>Endereço</legend>
                <div class="row">
                    <label>Endereço: </label> <input type="text" name="name">
                    <label>Número: </label> <input type="number" name="name"><br>
                </div>
                <div class="row">
                    <label>Bairro: </label> <input type="text" name="name"><br>
                    <label>Cidade: </label> <input type="text" name="name"><br>
                </div>
        </fieldset>
        <fieldset>
            <legend>Dados de contato</legend>
            <div class="row">
                <label>Celular: </label> <input type="text" name="name">
                <label>WhatsApp: </label> <input type="text" name="name"><br>
            </div>
            <div class="row">
                <label>Linkedin: </label> <input type="text" name="name">
                <label>GitHub: </label> <input type="text" name="name"><br>
            </div>
        </fieldset>
        <button type="reset">Limpar</button> <button type="submit">Enviar</button>
    </form>
```

## **AULA 4 ⇒ Embeds**

O embed é uma antiga tag que surgiu com o intuito de carregar conteúdos externos, hoje em dia não é mais usado, mas antigamente representou um grande avanço. Veja mais:

```html
<!-- O embed não é mais usada -->
    <!-- O embed serve para carregar um plug-in externo de forma independente-->
    <embed src="videos/ferrari-slow.mp4" type="">

    <p><span>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Voluptates quod quibusdam dolorem ullam eaque tempora asperiores, illum, illo totam accusamus quasi quisquam sequi expedita corporis cum quia accusantium maiores. Tempore.</span><span>Ab, aperiam, corporis dolores blanditiis fuga veniam nulla, nemo amet similique nobis molestiae modi facere. Earum ad iure esse at tenetur quam, soluta quod delectus labore consequatur maiores molestiae! Cupiditate.</span><span>Earum labore iste neque dignissimos, accusamus dolorum quae ratione veniam dolorem deleniti totam esse, illo vero. Culpa doloribus, omnis velit, maiores saepe molestias aspernatur exercitationem cumque itaque sed expedita recusandae.</span></p>
    <p><span>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Numquam molestias nihil commodi dolorem, quo deserunt nulla laudantium eaque. Dolor, sed officia iure maxime neque atque aperiam autem illum dicta totam.</span><span>Impedit dignissimos qui totam sint ratione, accusamus temporibus soluta? Aperiam ullam dolorem reprehenderit error! Non, impedit ullam saepe nemo, officia expedita obcaecati, voluptate delectus molestiae voluptates laborum atque modi dicta?</span><span>Explicabo libero architecto provident rem, assumenda harum earum corporis ea fugit non beatae obcaecati itaque fugiat quam accusamus aliquid voluptatum, id soluta repellendus nobis veniam perferendis quasi, similique saepe? Aliquam.</span></p>

    <!-- O embed não é semanticamente forte -->

    <!-- Vale mais a pena usar a tag video -->
    <video controls autoplay height="250px" width="250px">
        <source src="videos/ferrari-slow.mp4">
    </video>
```

## **AULA 5- Iframes**

O Iframe é uma tag muito útil e utilizada, nela é possível espelhar muitos tipos de conteúdos, como sites, vídeos, imagens e até localizações. Ela também está associada com segurança e com Javascript. Veja mais:

 

```
<!-- Pode afetar a segurança do site -->

    <!-- O Iframe abre uma janela na sua página com o conteúdo de outra página -->

    <!-- Exemplos: -->
    
    <iframe src="http://dio.me" frameborder="0"></iframe>
    <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3973.5058473426825!2d-39.29441504180432!3d-5.182854928012585!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x7bc3492b212c219%3A0xf31b81e5d45baea8!2sR.%20Luiz%20Saldanha%20de%20Almeida%20-%20Vila%20Betania%2C%20Quixeramobim%20-%20CE%2C%2063800-000!5e0!3m2!1spt-BR!2sbr!4v1698520456602!5m2!1spt-BR!2sbr" width="500" height="400" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
```
