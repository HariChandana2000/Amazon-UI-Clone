# Amazon-UI-Clone

1. Created this navbar by using display flex property and the icons like map, search and cart are included using goole font icons.
   <img width="946" alt="image" src="https://github.com/HariChandana2000/Amazon-UI-Clone/assets/44540754/f17d0edf-51e1-40bf-b49a-1596a7107348"/><br>                                
   Included this in the head tag for google font icons<br>
   ```<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@24,400,0,0"/>```<br>
   HTML Code: <br>
   ```
   <nav>
          <img class="amazon-logo" src="images/logo.png" alt="Amazon_logo" />
          <div class="map">
            <p>Deliver</p>
            <span>
              <span class="material-symbols-outlined"> location_on </span>
              <a href="#">India</a>
            </span>
          </div>
          <div class="search">
            <form action="">
              <select name="cateogry" id="cateogry">
                <option value="All">All</option>
                <option value="All Categories">All Categories</option>
                <option value="Amazon Devices">Amazon Devices</option>
              </select>
              <input type="text" name="search-box" placeholder="Search Amazon" />
              <button type="submit">
                <span class="material-symbols-outlined"> search </span>
              </button>
            </form>
          </div>
          <div class="right-icons">
            <div class="sign-in">
              <p>Hello, sign in</p>
              <a href="#">Account & Lists</a>
            </div>
            <div class="sign-in">
              <p>Returns</p>
              <a href="#">& Orders</a>
            </div>
            <div class="cart">
              <span
                ><span class="material-symbols-outlined"> shopping_cart </span>
                Cart</span
              >
            </div>
          </div>
        </nav>
   ```
   CSS Properties used:
   <pre>
      nav {
      display: flex;
      justify-content: space-around;
      align-items: center;
      width: 100%;
      height: 65px;
      background-color: #131921;
      color: white;
      line-height: 20px;
      cursor: pointer;
    }
    
    .amazon-logo {
      width: 150px;
      height: 60px;
      object-fit: cover;
    }
    
    .map {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      width: 150px;
      height: 60px;
    }
    
    .map > span {
      display: flex;
      align-items: center;
    }
    
    .map > p {
      color: #ccc;
      font-size: 12px;
      font-weight: 400;
    }
    
    .map a {
      font-size: 17px;
      text-decoration: none;
      color: white;
    }
    
    .map a:focus,
    a:visited {
      text-decoration: none;
      color: white;
    }
    
    nav a:hover {
      color: #ccc;
    }
    
    .search > form {
      display: flex;
      justify-content: center;
      align-items: center;
      white-space: nowrap;
      margin-right: 40px;
    }
    
    .search input {
      width: 500px;
      padding: 10px;
      border: 0;
    }
    
    .search input:focus {
      outline: none;
    }
    
    .search select {
      border: 0;
      color: #555;
      background-color: rgb(244, 241, 241);
      width: 65px;
      padding: 9.7px;
      border-top-left-radius: 5px;
      border-bottom-left-radius: 5px;
    }
    
    .search button {
      background-color: #f9ba5b;
      padding: 4px 12px;
      border: 0;
      border-top-right-radius: 5px;
      border-bottom-right-radius: 5px;
      cursor: pointer;
    }
    
    .right-icons {
      display: flex;
      justify-content: space-around;
      gap: 30px;
      align-items: center;
    }
    
    .right-icons > .sign-in {
      display: flex;
      flex-direction: column;
      flex-wrap: wrap;
    }
    
    .right-icons p {
      font-size: 12px;
      font-weight: 700;
    }
    
    .right-icons a {
      font-size: 14px;
      text-decoration: none;
      color: white;
      font-weight: 700;
    }
    
    .right-icons a:focus,
    a:visited {
      text-decoration: none;
    }
    
    .right-icons > .sign-in:hover {
      color: #ccc;
    }
    
    .cart .material-symbols-outlined {
      font-size: 40px;
    }
    
    .cart:hover {
      color: #ccc;
    }
  </pre>
  <br><br>

2. Created this header with display flex property with justify content as space between for left and right items.
   <img width="945" alt="image" src="https://github.com/HariChandana2000/Amazon-UI-Clone/assets/44540754/d92ef8c8-2c9b-4207-b1fe-ea9cd8fc70fa">
   HTML Code:<br>
   ```<header>
      <div class="left">
        <span class="material-symbols-outlined"> menu </span>
        <ul>
          <li><a href="#">All</a></li>
          <li><a href="#">Today's Deals</a></li>
          <li><a href="#">Customer Service</a></li>
          <li><a href="#">Registry</a></li>
          <li><a href="#">Gift Cards</a></li>
          <li><a href="#">Sell</a></li>
        </ul>
      </div>
      <div class="right">
        <a href="#"> Shop deals in Electronics</a>
      </div>
    </header>
   ```
   CSS Properties used:
   <pre>
     header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        background-color: #232f3e;
        color: white;
        width: 100%;
        height: 45px;
      }
      
      header > .left {
        display: flex;
        justify-content: space-between;
        gap: 10px;
        align-items: center;
        margin-left: 20px;
      }
      
      header > .right {
        margin-right: 20px;
      }
      
      header > .left > span {
        cursor: pointer;
      }
      
      header > .left > ul {
        list-style: none;
      }
      header > .left > ul > li {
        display: inline-block;
        margin: 5px;
      }
      
      header a {
        font-size: 14.5px;
        text-decoration: none;
      }
      
      header a:hover {
        color: #ccc;
      }
      
      header a:focus,
      a:visited {
        text-decoration: none;
      }
  </pre>
  <br><br>


3. Created this hero section to render the image. Used object-fit as contain to fit the full image in the container
   <img width="945" alt="image" src="https://github.com/HariChandana2000/Amazon-UI-Clone/assets/44540754/c4b1c65d-fc60-4e9c-a501-2c84ac9fbce3"><br>
   HTML Code:<br>
   ```
   <section class="hero">
      <img src="images/bg-image.png" alt="bg-image" />
    </section>
   ```
   CSS Properties used:
   <pre>
     .hero {
        width: 100%;
        height: fit-content;
        background-color: rgb(244, 241, 241);
      }
      
      .hero > img {
        width: 100%;
        height: auto;
        object-fit: contain;
      }
  </pre><br><br>


4. Created Shopping category container in which display flex is used to arrange the cards. Within each card display flex in column direction is used to arrange the h3, img     and a elements in vertical direction. Moreover transition property is used to zoom the card on hover.<br>
   HTML Code:<br>
   ```
   <section class="categories">
      <div class="card">
        <h3>Shop Laptops & Tables</h3>
        <img src="images/laptop-tables.png" alt="laptops and tables" />
        <a href="#">Shop now</a>
      </div>
      <div class="card">
        <h3>Shop Smartwatches</h3>
        <img src="images/smart-watches.png" alt="smart-watches" />
        <a href="#">Shop now</a>
      </div>
      <div class="card">
        <h3>Create with Strip Lights</h3>
        <img src="images/strip-lights.png" alt="strip-lights" />
        <a href="#">Shop now</a>
      </div>
      <div class="card">
        <h3>Home Refresh Ideas</h3>
        <img src="images/home-refresh.png" alt="home-refresh" />
        <a href="#">Shop now</a>
      </div>
    </section>
   ```
   
   CSS Properties:
   <pre>
      .categories {
        display: flex;
        justify-content: space-around;
        align-items: center;
        flex-wrap: wrap;
        gap: 20px;
        background-color: rgb(244, 241, 241);
        width: 100%;
        height: auto;
        margin: 0;
        padding-top: 40px;
        padding-bottom: 40px;
        overflow: hidden;
      }
      
      .card {
        display: flex;
        flex-direction: column;
        background-color: white;
        width: 285px;
        height: 400px;
        padding: 30px;
        cursor: pointer;
        white-space: nowrap;
        transform: scale(1);
        transition: transform 0.7s ease-in-out;
      }
      
      .card:hover {
        transform: scale(1.1);
      }
      
      .card > img {
        width: 100%;
        height: 240px;
        margin-top: 10px;
        object-fit: cover;
      }
      
      .card > a {
        color: blue;
        text-decoration: none;
        margin-top: 20px;
      }
      
      .card > a:hover {
        color: #c7511f;
        text-decoration: underline;
      }
   </pre><br><br>


5. Created this div element with paragraph element in it. Used onclick attribute on the div element to go to the top on click and the text color changes to light grey on       hover.<br>
   HTML Code:
   ```
   <div class="back-to-top" onclick="window.location.href='#'">
      <p>Back to top</p>
    </div>
   ```

   CSS Properties Used:
   <pre>
      .back-to-top {
        display: flex;
        align-items: center;
        justify-content: center;
        background-color: #354557;
        color: white;
        width: 100%;
        height: 60px;
        font-size: 14.5px;
        font-weight: 700;
        cursor: pointer;
        padding: 20px;
      }
      
      .back-to-top:hover {
        color: #ccc;
      }
   </pre><br><br>


6. Created this footer element with display property as flex. Each element in this footer is separate container with p and ul elements arranged in flex column direction.<br>
   HTML Code:<br>
   ```
   <footer>
      <div class="footer-item">
        <p>Get to Know Us</p>
        <ul>
          <li><a href="#">About us</a></li>
          <li><a href="#">Careers</a></li>
          <li><a href="#">Press Release</a></li>
          <li><a href="#">Amazon Science</a></li>
        </ul>
      </div>
      <div class="footer-item">
        <p>Connect with Us</p>
        <ul>
          <li><a href="#">Facebook</a></li>
          <li><a href="#">Twitter</a></li>
          <li><a href="#">Instagram</a></li>
        </ul>
      </div>
      <div class="footer-item">
        <p>Connect with Us</p>
        <ul>
          <li><a href="#">Sell on Amazon</a></li>
          <li><a href="#">Sell under Amazon Accelerator</a></li>
          <li><a href="#">Protect and Build Your Brand</a></li>
          <li><a href="#">Amazon Global Selling</a></li>
          <li><a href="#">Become an Affiliate</a></li>
          <li><a href="#">Fulfillment by Amazon</a></li>
          <li><a href="#">Advertise Your Products</a></li>
          <li><a href="#">Amazon Pay on Merchants</a></li>
        </ul>
      </div>
      <div class="footer-item">
        <p>Let Us Help You</p>
        <ul>
          <li><a href="#">COVID-19 and Amazon</a></li>
          <li><a href="#">Your Account</a></li>
          <li><a href="#">Return Centre</a></li>
          <li><a href="#">100% Purchase Protection</a></li>
          <li><a href="#">Amazon App Download</a></li>
          <li><a href="#">Help</a></li>
        </ul>
      </div>
    </footer>
   ```

   CSS Properties Used:<br>
   <pre>
      footer {
        display: flex;
        justify-content: space-around;
        background-color: #232f3e;
        width: 100%;
        height: auto;
        padding: 20px;
      }
      
      .footer-item {
        display: flex;
        flex-direction: column;
        color: white;
        line-height: 25px;
      }
      
      .footer-item p {
        font-size: 16.5px;
        font-weight: 400;
        margin-bottom: 15px;
      }
      
      .footer-item ul {
        list-style: none;
      }
      
      .footer-item ul > li > a {
        color: #ccc;
        text-decoration: none;
      }
      
      .footer-item ul > li > a:hover {
        text-decoration: underline;
      }
      
      .footer-item ul > li > a:visited {
        color: #ccc;
        text-decoration: none;
      }
   </pre>
   
