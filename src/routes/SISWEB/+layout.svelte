
<!--Aqui se escribe codigo js / se importan archivos (como imagenes)-->

<script></script>

<!--Layout para el nav bar que se pone en todos los elementos de 
  esta carpeta y de sus subcarpetas

  contiene header

  slot es donde se introduce el +pages.svelte segun el path
    
    !-->
<head>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-GLhlTQ8iRABdZLl6O3oVMWSktQOp6b7In1Zl3/Jr59b6EGGoI1aFkw7cmDA6j6gD" crossorigin="anonymous">
</head>

<div class="navContainer">
  <h1>Sisweb</h1>
  <div class="navOpt">
      <a href="/SISWEB/Products"><p>Product</p></a>
      <a href="/SISWEB/Store"><p>Shop</p></a>
      <button onclick="window.location.href='/';">Logout</button>

  </div>
  
</div>

<slot/>

<style>
  .navContainer {
      background: #7749F8;
      display: flex;
      justify-content: space-around;
      align-items: center;
      height: 60px;
      color: white;

  }

  .navOpt {
      display: flex;
      align-items: center;
      
  }

  .navOpt * {
      padding: 0 15px;
      font-size: 18px;
  }

  .navOpt button {
      margin-left: 20px;
      width: 104px;
      height: 38px;
      color: white;
      background: transparent;
      border: solid 1px white;
      border-radius: 4px;
      text-align: center;

  }

  .navOpt p {
    padding-top: 15px;
  }

  a {
    text-decoration: none;
    color: white;
  }


</style>
