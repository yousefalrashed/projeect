css
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@100;300;400;500;600&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Satisfy&display=swap");
* {
  font-family: 'Poppins', sans-serif;
  margin: 0;
  padding: 0;
  -webkit-box-sizing: border-box;
          box-sizing: border-box;
  outline: none;
  border: none;
  text-decoration: none;
  text-transform: capitalize;
  -webkit-transition: .2s linear;
  transition: .2s linear;
}

html {
  font-size: 62.5%;
  overflow-x: hidden;
  scroll-behavior: smooth;
  scroll-padding-top: 8.5rem;
}

html::-webkit-scrollbar {
  width: 1rem;
}

html::-webkit-scrollbar-track {
  background: #fff;
}

html::-webkit-scrollbar-thumb {
  background: #27ae60;
  border-radius: 5rem;
}

section {
  padding: 2rem 9%;
}

.heading {
  text-align: center;
  padding-bottom: 2rem;
}

.heading span {
  font-family: 'Satisfy', cursive;
  font-size: 3rem;
  color: #27ae60;
}

.heading h3 {
  font-size: 3rem;
  color: #130f40;
}

.btn {
  display: inline-block;
  margin-top: 1rem;
  padding: .7rem 1.8rem;
  font-size: 1.7rem;
  cursor: pointer;
  color: #fff;
  background: #27ae60;
  border-radius: .5rem;
}

.btn:hover {
  background: #130f40;
}

.header {
  position: -webkit-sticky;
  position: sticky;
  top: 0;
  left: 0;
  right: 0;
  z-index: 1000;
  background: #fff;
  -webkit-box-shadow: 0 1rem 1rem rgba(0, 0, 0, 0.05);
          box-shadow: 0 1rem 1rem rgba(0, 0, 0, 0.05);
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-align: center;
      -ms-flex-align: center;
          align-items: center;
  -webkit-box-pack: justify;
      -ms-flex-pack: justify;
          justify-content: space-between;
  padding: 2rem 9%;
}

.header .logo {
  font-size: 2.5rem;
  font-weight: bolder;
  color: #130f40;
}

.header .logo i {
  padding-right: .5rem;
  color: #27ae60;
}

.header .navbar a {
  font-size: 1.7rem;
  margin: 0 1rem;
  color: #666;
}

.header .navbar a:hover {
  color: #27ae60;
}

.header .icons div {
  height: 4.5rem;
  width: 4.5rem;
  line-height: 4.5rem;
  font-size: 2rem;
  background: #f7f7f7;
  color: #130f40;
  border-radius: .5rem;
  margin-left: .3rem;
  cursor: pointer;
  text-align: center;
}

.header .icons div:hover {
  color: #fff;
  background: #27ae60;
}

#menu-btn {
  display: none;
}

@-webkit-keyframes fadeUp {
  0% {
    -webkit-transform: translateY(5rem);
            transform: translateY(5rem);
    opacity: 0;
  }
}

@keyframes fadeUp {
  0% {
    -webkit-transform: translateY(5rem);
            transform: translateY(5rem);
    opacity: 0;
  }
}

.search-form-container {
  position: fixed;
  top: 8.5rem;
  left: 0;
  right: 0;
  height: calc(100vh - 8.5rem);
  background: #fff;
  z-index: 1000;
  display: none;
}

.search-form-container.active {
  display: block;
}

.search-form-container form {
  height: 7rem;
  border-bottom: 0.2rem solid #130f40;
  width: 100%;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-align: center;
      -ms-flex-align: center;
          align-items: center;
  -webkit-animation: fadeUp .4s linear;
          animation: fadeUp .4s linear;
}

.search-form-container form input {
  height: 100%;
  width: 100%;
  font-size: 1.7rem;
  color: #130f40;
  text-transform: none;
  padding-right: 1rem;
}

.search-form-container form label {
  font-size: 3rem;
  cursor: pointer;
  color: #130f40;
}

.search-form-container form label:hover {
  color: #27ae60;
}

.shopping-cart-container {
  position: fixed;
  top: 8.5rem;
  left: 0;
  right: 0;
  z-index: 1000;
  height: calc(100vh - 8.5rem);
  background: #fff;
  overflow-y: scroll;
  padding-bottom: 8rem;
  display: none;
}

.shopping-cart-container.active {
  display: block;
}

.shopping-cart-container::-webkit-scrollbar {
  width: 1rem;
}

.shopping-cart-container::-webkit-scrollbar-track {
  background: #fff;
}

.shopping-cart-container::-webkit-scrollbar-thumb {
  background: #130f40;
  border-radius: 5rem;
}

.shopping-cart-container .title {
  font-size: 2.5rem;
  padding: 1rem;
  color: #130f40;
  border-bottom: 0.1rem solid rgba(0, 0, 0, 0.2);
  text-align: center;
}

.shopping-cart-container .products-container {
  border: 0.1rem solid rgba(0, 0, 0, 0.2);
  border-radius: .5rem;
  -webkit-animation: fadeUp .4s linear;
          animation: fadeUp .4s linear;
}

.shopping-cart-container .products-container .box-container {
  display: -ms-grid;
  display: grid;
  -ms-grid-columns: (minmax(30rem, 1fr))[auto-fit];
      grid-template-columns: repeat(auto-fit, minmax(30rem, 1fr));
  gap: 1.5rem;
  padding: 1.5rem;
}

.shopping-cart-container .products-container .box-container .box {
  border-radius: .5rem;
  background: #f7f7f7;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-align: center;
      -ms-flex-align: center;
          align-items: center;
  gap: 1.5rem;
  padding: 2rem;
  position: relative;
}

.shopping-cart-container .products-container .box-container .box .fa-times {
  position: absolute;
  top: .7rem;
  right: 1rem;
  font-size: 2rem;
  cursor: pointer;
  color: #130f40;
}

.shopping-cart-container .products-container .box-container .box .fa-times:hover {
  color: #27ae60;
}

.shopping-cart-container .products-container .box-container .box img {
  height: 8rem;
}

.shopping-cart-container .products-container .box-container .box .content h3 {
  font-size: 2rem;
  color: #130f40;
}

.shopping-cart-container .products-container .box-container .box .content span {
  font-size: 1.5rem;
  color: #666;
}

.shopping-cart-container .products-container .box-container .box .content span.price {
  color: #27ae60;
  font-size: 1.7rem;
}

.shopping-cart-container .products-container .box-container .box .content input {
  width: 8rem;
  padding: .5rem 1.2rem;
  font-size: 1.5rem;
  color: #130f40;
  margin: .7rem 0;
}

.shopping-cart-container .cart-total {
  margin-top: 2rem;
  border: 0.1rem solid rgba(0, 0, 0, 0.2);
  border-radius: .5rem;
  -webkit-animation: fadeUp .4s linear .4s backwards;
          animation: fadeUp .4s linear .4s backwards;
}

.shopping-cart-container .cart-total .box {
  padding: 1.5rem;
}

.shopping-cart-container .cart-total .box h3 {
  color: #130f40;
  font-size: 2rem;
  padding-bottom: .7rem;
}

.shopping-cart-container .cart-total .box h3 span {
  color: #27ae60;
}

.login-form-container {
  position: fixed;
  top: 8.5rem;
  left: 0;
  right: 0;
  z-index: 1000;
  height: calc(100vh - 8.5rem);
  background: #fff;
  padding: 0 2rem;
  display: none;
}

.login-form-container.active {
  display: block;
}

.login-form-container form {
  margin: 2rem auto;
  max-width: 40rem;
  -webkit-box-shadow: 0 1rem 1rem rgba(0, 0, 0, 0.05);
          box-shadow: 0 1rem 1rem rgba(0, 0, 0, 0.05);
  border: 0.1rem solid rgba(0, 0, 0, 0.2);
  padding: 2rem;
  border-radius: .5rem;
  -webkit-animation: fadeUp .4s linear;
          animation: fadeUp .4s linear;
}

.login-form-container form h3 {
  padding-bottom: 1rem;
  font-size: 2.5rem;
  text-transform: uppercase;
  color: #130f40;
}

.login-form-container form .box {
  margin: .7rem 0;
  border-radius: .5rem;
  background: #f7f7f7;
  padding: 1rem 1.2rem;
  font-size: 1.6rem;
  color: #130f40;
  text-transform: none;
  width: 100%;
}

.login-form-container form .remember {
  padding: 1rem 0;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-align: center;
      -ms-flex-align: center;
          align-items: center;
  gap: .5rem;
}

.login-form-container form .remember label {
  font-size: 1.5rem;
  cursor: pointer;
  color: #666;
}

.login-form-container form .btn {
  margin: 1rem 0;
  width: 100%;
  text-align: center;
}

.login-form-container form p {
  padding-top: 1rem;
  font-size: 1.5rem;
  color: #666;
}

.login-form-container form p a {
  color: #27ae60;
}

.login-form-container form p a:hover {
  color: #130f40;
  text-decoration: underline;
}

.home {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-align: center;
      -ms-flex-align: center;
          align-items: center;
  -ms-flex-wrap: wrap-reverse;
      flex-wrap: wrap-reverse;
  gap: 2rem;
  position: relative;
  overflow: hidden;
}

.home .content {
  -webkit-box-flex: 1;
      -ms-flex: 1 1 41rem;
          flex: 1 1 41rem;
}

.home .content span {
  font-size: 2rem;
  color: #27ae60;
}

.home .content h3 {
  font-size: 4rem;
  color: #130f40;
  padding-top: 1rem;
}

.home .content p {
  font-size: 1.4rem;
  color: #666;
  line-height: 2;
  padding: 1rem 0;
}

.home .image {
  -webkit-box-flex: 1;
      -ms-flex: 1 1 41rem;
          flex: 1 1 41rem;
  margin: 2rem 0;
  pointer-events: none;
}

.home .image .home-img {
  width: 100%;
  margin-top: 5rem;
}

.home .home-parallax-img {
  position: absolute;
  top: -10rem;
  right: -10rem;
  width: 80vw;
}

.category {
  display: -ms-grid;
  display: grid;
  -ms-grid-columns: (minmax(16rem, 1fr))[auto-fit];
      grid-template-columns: repeat(auto-fit, minmax(16rem, 1fr));
  gap: 1.5rem;
  padding-bottom: 5rem;
}

.category .box {
  padding: 2rem;
  text-align: center;
  border-radius: .5rem;
  background: #f7f7f7;
}

.category .box:hover {
  background: #27ae60;
}

.category .box:hover h3 {
  color: #fff;
}

.category .box img {
  height: 7rem;
}

.category .box h3 {
  font-size: 1.8rem;
  color: #130f40;
}

.about {
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -ms-flex-wrap: wrap;
      flex-wrap: wrap;
  -webkit-box-align: center;
      -ms-flex-align: center;
          align-items: center;
  gap: 2rem;
  background: #f7f7f7;
  margin-bottom: 30px;
}

.about .image {
  -webkit-box-flex: 1;
      -ms-flex: 1 1 40rem;
          flex: 1 1 40rem;
}

.about .image img {
  width: 100%;
}

.about .content {
  -webkit-box-flex: 1;
      -ms-flex: 1 1 40rem;
          flex: 1 1 40rem;
}

.about .content span {
  font-family: 'Satisfy', cursive;
  font-size: 3rem;
  color: #27ae60;
}

.about .content .title {
  font-size: 3rem;
  padding-top: .5rem;
  color: #130f40;
}

.about .content p {
  padding: 1rem 0;
  line-height: 2;
  font-size: 1.4rem;
  color: #666;
}

.about .content .icons-container {
  margin-top: 2rem;
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -ms-flex-wrap: wrap;
      flex-wrap: wrap;
  gap: 1.5rem;
}

.about .content .icons-container .icons {
  -webkit-box-flex: 1;
      -ms-flex: 1 1 20rem;
          flex: 1 1 20rem;
  border-radius: .5rem;
  background: #fff;
  -webkit-box-shadow: 0 1rem 1rem rgba(0, 0, 0, 0.05);
          box-shadow: 0 1rem 1rem rgba(0, 0, 0, 0.05);
  display: -webkit-box;
  display: -ms-flexbox;
  display: flex;
  -webkit-box-align: center;
      -ms-flex-align: center;
          align-items: center;
  gap: 2rem;
  padding: 2rem;
}

.about .content .icons-container .icons h3 {
  font-size: 1.7rem;
  color: #130f40;
}

.popular .box-container {
  display: -ms-grid;
  display: grid;
  -ms-grid-columns: (minmax(25rem, 1fr))[auto-fit];
      grid-template-columns: repeat(auto-fit, minmax(25rem, 1fr));
  gap: 1.5rem;
}

.popular .box-container .box {
  border-radius: .5rem;
  position: relative;
  background: #f7f7f7;
  padding: 2rem;
  text-align: center;
}

.popular .box-container .box .fa-heart {
  position: absolute;
  top: 1.5rem;
  right: 1.5rem;
  font-size: 2.5rem;
  color: #666;
  cursor: pointer;
}

.popular .box-container .box .fa-heart:hover {
  color: #27ae60;
}

.popular .box-container .box .image {
  margin: 1rem 0;
}

.popular .box-container .box .image img {
  height: 15rem;
}

.popular .box-container .box .content h3 {
  font-size: 2rem;
  color: #130f40;
}

.popular .box-container .box .content .stars {
  padding: 1rem 0;
  font-size: 1.7rem;
}

.popular .box-container .box .content .stars i {
  color: gold;
}

.popular .box-container .box .content .stars span {
  color: #666;
}

.popular .box-container .box .content .price {
  font-size: 2rem;
  color: #130f40;
}

.popular .box-container .box .content .price span {
  font-size: 1.5rem;
  color: #666;
  text-decoration: line-through;
}


.footer {
  background: #f7f7f7;
}


.footer .box-container {
  display: -ms-grid;
  display: grid;
  -ms-grid-columns: (minmax(25rem, 1fr))[auto-fit];
      grid-template-columns: repeat(auto-fit, minmax(25rem, 1fr));
  gap: 1.5rem;
}

.footer .box-container .box h3 {
  font-size: 2.2rem;
  color: #130f40;
  padding: 1rem 0;
}

.footer .box-container .box p {
  font-size: 1.4rem;
  color: #666;
  padding: 1rem 0;
}

.footer .box-container .box a {
  display: block;
  font-size: 1.4rem;
  color: #666;
  padding: 1rem 0;
}

.footer .box-container .box a:hover {
  color: #27ae60;
}

.footer .box-container .box a:hover i {
  padding-right: 2rem;
}

.footer .box-container .box a i {
  padding-right: .5rem;
  color: #27ae60;
}

.footer .bottom {
  padding-top: 1rem;
  text-align: center;
}

.footer .bottom .share {
  margin: 1.5rem 0;
}

.footer .bottom .share a {
  height: 4.5rem;
  width: 4.5rem;
  line-height: 4.5rem;
  font-size: 2rem;
  border-radius: .5rem;
  margin: 0 .3rem;
  color: #fff;
  background: #27ae60;
}

.footer .bottom .share a:hover {
  background: #130f40;
}

.footer .bottom .credit {
  font-size: 2rem;
  color: #666;
  padding: 1rem;
}

.footer .bottom .credit span {
  color: #27ae60;
}

@media (max-width: 991px) {
  html {
    font-size: 55%;
  }
  .header {
    padding: 2rem;
  }
  section {
    padding: 2rem;
  }
}

@media (max-width: 768px) {
  #menu-btn {
    display: inline-block;
  }
  .header .navbar {
    position: absolute;
    top: 99%;
    left: 0;
    right: 0;
    background: #fff;
    border-top: 0.1rem solid rgba(0, 0, 0, 0.2);
    border-bottom: 0.1rem solid rgba(0, 0, 0, 0.2);
    -webkit-clip-path: polygon(0 0, 100% 0, 100% 0, 0 0);
            clip-path: polygon(0 0, 100% 0, 100% 0, 0 0);
  }
  .header .navbar.active {
    -webkit-clip-path: polygon(0 0, 100% 0, 100% 100%, 0% 100%);
            clip-path: polygon(0 0, 100% 0, 100% 100%, 0% 100%);
  }
  .header .navbar a {
    font-size: 2rem;
    margin: 2rem;
    display: block;
  }
  .home .home-parallax-img {
    top: 0;
    right: 0;
    width: 130%;
  }
  .order form .flex .inputBox {
    width: 100%;
  }
}

@media (max-width: 450px) {
  html {
    font-size: 50%;
  }
  .shopping-cart-container .cart-total .box {
    text-align: center;
  }
  .shopping-cart-container .cart-total .box .btn {
    width: 100%;
  }
  .home .content h3 {
    font-size: 3rem;
  }
  .home .content p {
    font-size: 1.5rem;
  }
}
/*# sourceMappingURL=style.css.map */
