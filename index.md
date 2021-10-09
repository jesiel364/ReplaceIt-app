<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Replace.it</title>
    <link rel="stylesheet" type="text/css" href="./css/bootstrap.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Anton&family=Grenze+Gotisch:wght@100&display=swap" rel="stylesheet">
  
  <script>
function REplace(){
    txt = document.querySelector('textarea#txt').value
    char = document.querySelector('input#char').value
    new_char = document.querySelector('input#new_char').value
    container = document.querySelector('div#container')
    
    new_text = txt.replaceAll(char, new_char)
    novo_copy = document.createElement('button')
    novo_copy.setAttribute('class', 'btn btn-primary mt-2')
    novo_copy.innerHTML = 'Copy'
    novo_copy.setAttribute('id', 'btn-copy')
    card = document.createElement('div')
    card_body = document.createElement('div')
    card.setAttribute('class', 'card mt-4')
    card_body.setAttribute('class', 'card-body')
    card_body.setAttribute('id', 'res')
    // container.appendChild(card)
    card.appendChild(card_body)
    card_body.innerHTML = `<h4 class="mt-4">Resultado</h4>`
    card_body.innerHTML = `<p>${new_text}</p>`
    card_body.appendChild(novo_copy)
    container.appendChild(card)


  }

  // function clipboard(txt){
  //  var res = document.getElementById('res')
  //  res.select()
  //  if(true){
  //    res.document.execCommand('copy')
  // }}

</script>

<style type="text/css">
  body{
    font-family: 'Josefin Sans', sans-serif;"
  }
  #res{
    font-family: 'Grenze Gotisch'
}
</style>
<body>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
  <div class="container-fluid">
    <a style="font-family: 'Grenze Gotisch', cursive, sans-serif;" class="navbar-brand" href="https://jesiel364.github.io/ReplaceIt-app"/>Replace.it</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li class="nav-item">
          <a class="nav-link active" aria-current="page" href="https://jesiel364.github.io/ReplaceIt-app/">Inicio</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="https://github.com/jesiel364/ReplaceIt-app">Doc</a>
        </li>

        <li class="nav-item">
          <a class="nav-link" href="https://github.com/jesiel364/">Contato</a>
        </li>
        
      </ul>
      <form class="d-flex">
        <input class="form-control me-2" type="search" placeholder="Digite algo" aria-label="Search">
        <button class="btn btn-outline-success" type="submit">Pesquisar</button>
      </form>
    </div>
  </div>
</nav>

    <div id="container" class="container mt-4">

    <h1>Substituidor de Caracteres</h1>
      
<div class="mb-3">
  <label for="txt" class="form-label">Texto</label>
  <textarea class="form-control" id="txt" rows="3" placeholder="
manga, banana, laranja, ameixa"></textarea>
</div>

<div class="mb-3">
  <label for="char" class="form-label">Caractere(s) a ser substituido</label>
  <input type="text" class="form-control" id="char" placeholder="*Deixe este campo vazio para nulo.">
</div>

<div class="mb-3">
  <label for="new_char" class="form-label">Novo(s) Caractere(s)</label>
  <input type="text" class="form-control" id="new_char" placeholder="*Deixe este campo vazio para nulo.">
</div>

<button onclick="REplace()" type="button" class="btn btn-success mt-2">Substituir</button>


<!-- <div class="form-group">
  <button class="btn btn-primary mt-2" onclick="clipboard('copy')">Copiar</button>
</div> -->
    
    </div>
</body>
<script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.10.2/dist/umd/popper.min.js" integrity="sha384-7+zCNj/IqJ95wo16oMtfsKbZ9ccEh31eOz1HGyDuCQ6wgnyJNSYdrPa03rtR1zdB" crossorigin="anonymous"></script>
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.2/dist/js/bootstrap.min.js" integrity="sha384-PsUw7Xwds7x08Ew3exXhqzbhuEYmA2xnwc8BuD6SEr+UmEHlX8/MCltYEodzWA4u" crossorigin="anonymous"></script>
<script src="/js/bootstrap.js"></script>
</html><!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Replace.it</title>
    <link rel="stylesheet" type="text/css" href="./css/bootstrap.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Anton&family=Grenze+Gotisch:wght@100&display=swap" rel="stylesheet">
  
  <script>
function REplace(){
    txt = document.querySelector('textarea#txt').value
    char = document.querySelector('input#char').value
    new_char = document.querySelector('input#new_char').value
    container = document.querySelector('div#container')
    
    new_text = txt.replaceAll(char, new_char)
    novo_copy = document.createElement('button')
    novo_copy.setAttribute('class', 'btn btn-primary mt-2')
    novo_copy.innerHTML = 'Copy'
    novo_copy.setAttribute('id', 'btn-copy')
    card = document.createElement('div')
    card_body = document.createElement('div')
    card.setAttribute('class', 'card mt-4')
    card_body.setAttribute('class', 'card-body')
    card_body.setAttribute('id', 'res')
    // container.appendChild(card)
    card.appendChild(card_body)
    card_body.innerHTML = `<h4 class="mt-4">Resultado</h4>`
    card_body.innerHTML = `<p>${new_text}</p>`
    card_body.appendChild(novo_copy)
    container.appendChild(card)


  }

  // function clipboard(txt){
  //  var res = document.getElementById('res')
  //  res.select()
  //  if(true){
  //    res.document.execCommand('copy')
  // }}

</script>

<style type="text/css">
  body{
    font-family: 'Josefin Sans', sans-serif;"
  }
</style>
<body>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
  <div class="container-fluid">
    <a style="font-family: 'Grenze Gotisch', cursive, sans-serif;" class="navbar-brand" href="#">replace.it</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li class="nav-item">
          <a class="nav-link active" aria-current="page" href="https://jesiel364.github.io/ReplaceIt-app/">Inicio</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="https://github.com/jesiel364/ReplaceIt-app">Doc</a>
        </li>

        <li class="nav-item">
          <a class="nav-link" href="https://github.com/jesiel364/">Contato</a>
        </li>
        
      </ul>
      <form class="d-flex">
        <input class="form-control me-2" type="search" placeholder="Digite algo" aria-label="Search">
        <button class="btn btn-outline-success" type="submit">Pesquisar</button>
      </form>
    </div>
  </div>
</nav>

    <div id="container" class="container mt-4">

    <h1>Substituidor de Caracteres</h1>
      
<div class="mb-3">
  <label for="txt" class="form-label">Texto</label>
  <textarea class="form-control" id="txt" rows="3" placeholder="manga, banana, laranja, ameixa"></textarea>
</div>

<div class="mb-3">
  <label for="char" class="form-label">Caractere(s) a ser substituido</label>
  <input type="text" class="form-control" id="char" placeholder="">
</div>

<div class="mb-3">
  <label for="new_char" class="form-label">Novo(s) Caractere(s)</label>
  <input type="text" class="form-control" id="new_char" placeholder="*Deixe este campo vazio para nulo.">
</div>

<button onclick="REplace()" type="button" class="btn btn-success mt-2">Substituir</button>


<!-- <div class="form-group">
  <button class="btn btn-primary mt-2" onclick="clipboard('copy')">Copiar</button>
</div> -->
    
    </div>
</body>
<script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.10.2/dist/umd/popper.min.js" integrity="sha384-7+zCNj/IqJ95wo16oMtfsKbZ9ccEh31eOz1HGyDuCQ6wgnyJNSYdrPa03rtR1zdB" crossorigin="anonymous"></script>
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.2/dist/js/bootstrap.min.js" integrity="sha384-PsUw7Xwds7x08Ew3exXhqzbhuEYmA2xnwc8BuD6SEr+UmEHlX8/MCltYEodzWA4u" crossorigin="anonymous"></script>
<script src="/js/bootstrap.js"></script>
</html>
