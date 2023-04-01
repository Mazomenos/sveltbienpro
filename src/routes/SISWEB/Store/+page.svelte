<!--Aqui se escribe codigo js / se importan archivos (como imagenes)-->
<!--Store 
    Path: /SISWEB/Store
    !-->
    <body>
        <div class="mainContainer">
        <div><h1>Shop</h1></div>
        <div class="container">
          <div id="all" class="row">
            <div class="col-sm-8">
              <div id="cards" class="d-flex">
                <img src="/images/sephora.png" alt="product" />
                <div>
                  <div>
                    <h5><strong>PRODUCT ID: COS01</strong></h5>
                    <h4>Sephora Skin Care - 1 u</h4>
                    <h3><strong>IN STOCK: </strong>4 UNITS</h3>
                    <p id="price">$45.50</p>
                  </div>
                  <div id="qtybox">
                    <label for="qty">Qty: </label>
                    <input type="text" id="qty" name="qty" placeholder="1" /><br />
                  </div>
                  <button type="button"
                    ><i class="fa fa-shopping-cart" /> ADD TO CART</button
                  >
                </div>
              </div>
              <div>
                <div id="cards" class="d-flex">
                  <img src="/images/sephora.png" alt="product" />
                  <div>
                    <div>
                      <h5><strong>PRODUCT ID: COS01</strong></h5>
                      <h4>Sephora Skin Care - 1 u</h4>
                      <h3><strong>IN STOCK: </strong>4 UNITS</h3>
                      <p id="price">$45.50</p>
                    </div>
                    <div id="qtybox">
                      <label for="qty">Qty: </label>
                      <input type="text" id="qty" name="qty" placeholder="1" /><br />
                    </div>
                    <button type="button"
                      ><i class="fa fa-shopping-cart" /> ADD TO CART</button
                    >
                  </div>
                </div>
              </div>
            </div>
            <div id="cart" class="col-sm-4">
              <table>
                <th id="shoppingCartTitle"
                  ><i class="fa fa-shopping-cart" /> SHOPPING CART
                </th>
                <tr id="products" /><tr>
                  <tc id="product">
                    <label>
                      <input type="checkbox" id="product1" value="first_checkbox" />2
                      Sephora Skin Care - 1u
                    </label>
                    <strong>$91.00</strong>
                  </tc>
                </tr>
                <tr>
                  <tc id="product">
                    <label>
                      <input type="checkbox" id="product2" value="second_checkbox" />
                      1 Dior Face Beauty - 1u
                    </label>
                    <strong>$50.00</strong>
                  </tc>
                </tr>
                <tr id="total">
                  <button id="eraseFromCart" type="button"
                    ><i class="fal fa-trash-alt" /></button
                  >
                  <tc><strong>TOTAL</strong></tc>
                  <tc><strong>$141.00</strong></tc>
                </tr>
                <tr id="rowCheckout">
                  <button id="checkout" type="button">CHECKOUT</button>
                </tr>
              </table>
            </div>
          </div>
        </div>
        </div>
      </body>
      
      <!--Aqui dentro del style se agrega todo el codigo CSS
      ESTE CSS SOLO AFECTA A ELEMENTOS DE ESTE ARCHIVO/PAGINA-->
      <style>
        h1 {
          border-bottom: 1px solid rgb(201, 198, 198);
          padding-bottom: 1%;
        }
        #cards {
          margin-bottom: 50px;
        }
        #qty {
          display: flex;
          text-align: center;
        }
        #qtybox {
          display: flex;
        }
        img {
          margin-right: 5%;
        }
        #price {
          font-size: 1.5rem;
          color: blueviolet;
          margin: 1.8rem auto 1.8rem auto;
        }
        button {
          margin-top: 1rem;
          background-color: white;
          border: 1px solid blueviolet;
          color: blueviolet;
          border-radius: 4px;
          width: 100%;
        }
        button:hover {
          margin-top: 1rem;
          background-color: blueviolet;
          border: 1px solid blueviolet;
          color: #f7f5f8;
          border-radius: 4px;
          width: 100%;
        }
        button:active {
          margin-top: 1rem;
          background-color: rgb(182, 125, 235);
          border: 1px solid blueviolet;
          color: #f7f5f8;
          border-radius: 4px;
          width: 100%;
        }
        table {
          width: 100%;
        }
        #shoppingCartTitle {
          color: blueviolet;
        }
        tr,
        th {
          background-color: rgb(234, 231, 231);
        }
        th {
          padding: 2% 7% 2% 7%;
          border-bottom: 1px solid rgb(201, 198, 198);
        }
        tc,
        label {
          display: flex;
          margin: 2% 7% 2% 7%;
        }
        #product {
          display: flex;
          align-items: center;
          justify-content: space-between;
        }
        #total {
          display: flex;
          justify-content: space-between;
          border-top: 1px solid rgb(201, 198, 198);
          padding: 2% 0 2% 7%;
          align-items: center;
        }
        #eraseFromCart {
          border: 0;
          margin: 0;
          width: auto;
          background-color: rgb(234, 231, 231);
          align-items: top;
        }
        #eraseFromCart:hover {
          color: rgb(179, 132, 222);
        }
        #eraseFromCart:active {
          color: rgb(234, 231, 231);
        }
        #checkout {
          margin: 0 10% 2% 53%;
          width: 40%;
          background-color: rgb(234, 231, 231);
        }
        #checkout:hover {
          background-color: blueviolet;
          border: 1px solid blueviolet;
          color: #f7f5f8;
        }
        #checkout:active {
          background-color: rgb(182, 125, 235);
          border: 1px solid blueviolet;
          color: #f7f5f8;
        }

        .mainContainer {
            width: 90%;
            margin: auto;
        }
        
      </style>