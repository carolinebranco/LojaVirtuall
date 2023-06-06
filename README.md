# LojaVirtuall
echo "#LojaVirtual" >> README.md 
git init 
git add README.md 
git commit -m "first commit" 
git branch -M main 
git remote add origin https://github.com/carolinebranco/LojaVirtual.git
 git push - sua origem principal
 <!DOCTYPE html>
<html>
<head>
  <title>LojaVirtual</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: Arial, sans-serif;
    }

    header {
      background-color: #f2f2f2;
      padding: 20px;
      text-align: center;
    }

    main {
      max-width: 800px;
      margin: 0 auto;
      padding: 20px;
    }

    ul {
      list-style-type: none;
    }

    li {
      margin-bottom: 20px;
      display: flex;
      align-items: center;
    }

    img {
      width: 100px;
      height: 100px;
      margin-right: 10px;
    }

    .product-details {
      flex-grow: 1;
    }

    .add-to-cart {
      background-color: #4CAF50;
      color: #fff;
      border: none;
      padding: 10px 20px;
      cursor: pointer;
    }

    .product-info {
      display: none;
      padding: 10px;
      border: 1px solid #ccc;
      margin-top: 10px;
    }

    .product:hover .product-info {
      display: block;
    }

    footer {
      background-color: #f2f2f2;
      padding: 20px;
      text-align: center;
    }
  </style>
</head>
<body>
  <header>
    <h1>Minha Loja Virtual</h1>
  </header>

  <main>
    <h2>Produtos</h2>
    <ul>
      <li class="product">
        <img src="item1.jpg" alt="Item 1">
        <div class="product-details">
          <div>Item 1 - R$ 10.99</div>
          <button class="add-to-cart">Adicionar ao carrinho</button>
          <div class="product-info">
            <p>Descrição do Item 1</p>
            <p>Outras informações sobre o Item 1</p>
          </div>
        </div>
      </li>
      <li class="product">
        <img src="item2.jpg" alt="Item 2">
        <div class="product-details">
          <div>Item 2 - R$ 19.99</div>
          <button class="add-to-cart">Adicionar ao carrinho</button>
          <div class="product-info">
            <p>Descrição do Item 2</p>
            <p>Outras informações sobre o Item 2</p>
          </div>
        </div>
      </li>
      <!-- Adicione os outros itens aqui -->
    </ul>
  </main>

  <footer>
    <p>&copy; 2023 Minha Loja Virtual. Todos os direitos reservados.</p>
  </footer>

  <script>
    const addButtons = document.querySelectorAll('.add-to-cart');
    addButtons.forEach(button => {
      button.addEventListener('click', () => {
        const productInfo = button.nextElementSibling;
        productInfo.classList.toggle('show');
      });
    });
  </script>
</body>
</html>
