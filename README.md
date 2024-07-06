```
<!DOCTYPE html>
<html>
<head>
<title>Dribbble Clone</title>
<style>
body {
  font-family: sans-serif;
  margin: 0;
}

header {
  background-color: hsl(237, 53%, 58%);
  color: #fff;
  padding: 1em;
}

nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  font-size: 2em;
  font-weight: bold;
  text-decoration: none;
  color: #fff;
}

.nav-links {
  display: flex;
  list-style: none;
  margin: 0;
  padding: 0;
}

.nav-links li {
  margin-right: 1em;
}

.nav-links a {
  color: #fff;
  text-decoration: none;
}

.nav-links a:hover {
  text-decoration: underline;
}

.search-bar {
  display: flex;
  align-items: center;
}

.search-bar input {
  padding: 0.5em;
  border: none;
  border-radius: 5px;
}

.search-bar button {
  padding: 0.5em 1em;
  border: none;
  border-radius: 5px;
  background-color: #fff;
  color:  hsl(237, 53%, 58%);
  cursor: pointer;
}

.hero {
  background-color: #f0f0f0;
  padding: 2em;
  text-align: center;
}

.hero h1 {
  font-size: 2em;
}

.hero p {
  font-size: 1.2em;
  margin-bottom: 1em;
}

.hero button {
  padding: 0.8em 1.5em;
  border: none;
  border-radius: 5px;
  background-color: #333;
  color: #fff;
  cursor: pointer;
}

.content {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  padding: 2em;
}

.card {
  width: 200px;
  margin: 1em;
  background-color: #fff;
  border-radius: 5px;
  overflow: hidden;
  box-shadow: 0 2px 5px  hsl(237, 53%, 58%);
  cursor: pointer;
  position: relative; /* For the overlay */
}

.card img {
  width: 100%;
  height: 150px;
  object-fit: cover;
}

.card-content {
  padding: 1em;
}

.card-title {
  font-weight: bold;
  margin-bottom: 0.5em;
}

.card-stats {
  display: flex;
  justify-content: space-between;
  align-items: center;
  color:  hsl(237, 53%, 58%);
  font-size: 0.8em;
}

.card-stats i {
  margin-right: 0.5em;
}

.overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: hsl(237, 53%, 58%);
  color: #fff;
  display: flex;
  justify-content: center;
  align-items: center;
  opacity: 0;
  transition: opacity 0.3s ease-in-out;
}

.card:hover .overlay {
  opacity: 1;
}

.overlay-text {
  font-size: 1.2em;
  font-weight: bold;
}

.pagination {
  display: flex;
  justify-content: center;
  margin-top: 2em;
}

.pagination button {
  padding: 0.5em 1em;
  border: none;
  border-radius: 5px;
  background-color:  hsl(237, 53%, 58%);
  color: #fff;
  cursor: pointer;
  margin: 0 0.5em;
}

.pagination button.active {
  background-color: #fff;
  color:  hsl(237, 53%, 58%);
}

.footer {
  background-color:  hsl(237, 53%, 58%);
  color: #fff;
  padding: 1em;
  text-align: center;
}
</style>
</head>
<body>

<header>
  <nav>
    <a href="#" class="logo">Dribbble</a>
    <ul class="nav-links">
      <li><a href="#">Shots</a></li>
      <li><a href="#">Designers</a></li>
      <li><a href="#">Teams</a></li>
      <li><a href="#">Community</a></li>
      <li><a href="#">Jobs</a></li>
    </ul>
    <div class="search-bar">
      <input type="text" placeholder="Search">
      <button>Search</button>
    </div>
    <div>
      <button>Sign up</button>
      <button>Sign in</button>
    </div>
  </nav>
</header>

<div class="hero">
  <h1>What are you working on?</h1>
  <p>Dribbble is show and tell for designers.</p>
  <button>Learn more</button>
  <button>Sign up</button>
</div>

<div class="content">
  <div class="card">
    <img src="https://www.blsinternational.com/blog/wp-content/uploads/2024/02/The-Big-Wave-of-Tourism-in-India-20-Feb-24.jpeg">
    <div class="card-content">
      <h2 class="card-title">Famous</h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 4,044
        <i class="fas fa-comments"></i> 14
        <i class="fas fa-heart"></i> 290
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
  <div class="card">
    <img src="https://tse1.mm.bing.net/th?id=OIP._4nLGybPMKowc8wPdjII8gAAAA&pid=Api&P=0&h=180">
    <div class="card-content">
      <h2 class="card-title">Trading</h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 2,404
        <i class="fas fa-comments"></i> 13
        <i class="fas fa-heart"></i> 236
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
  <div class="card">
    <img src="https://tse3.mm.bing.net/th?id=OIP.J7a9cK_gnSTtza7ylXxDWwHaEo&pid=Api&P=0&h=180">
    <div class="card-content">
      <h2 class="card-title">3D Animation Techniques</h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 3,985
        <i class="fas fa-comments"></i> 17
        <i class="fas fa-heart"></i> 264
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
  <div class="card">
    <img src="https://tse2.mm.bing.net/th?id=OIP.0IFjen8S_UDqMfnUYG4aBwHaEK&pid=Api&P=0&h=180">
    <div class="card-content">
      <h2 class="card-title">Software Engineering Division</h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 2,602
        <i class="fas fa-comments"></i> 23
        <i class="fas fa-heart"></i> 186
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
  <div class="card">
    <img src="https://tse2.mm.bing.net/th?id=OIP.gsWsnGPJ6emp4Im2O3wyRQHaEK&pid=Api&P=0&h=180">
    <div class="card-content">
      <h2 class="card-title">Unleashing AI</h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 2,369
        <i class="fas fa-comments"></i> 8
        <i class="fas fa-heart"></i> 178
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
  <div class="card">
    <img src="https://tse4.mm.bing.net/th?id=OIP.jbXDTxEDCffgn-7R9vSOXwHaDm&pid=Api&P=0&h=180">
    <div class="card-content">
      <h2 class="card-title">Android Studio</h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 2,025
        <i class="fas fa-comments"></i> 6
        <i class="fas fa-heart"></i> 160
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
  <div class="card">
    <img src="https://news-cdn.softpedia.com/images/news2/linux-mint-debian-edition-3-cindy-cinnamon-edition-is-out-upgrade-now-522539-2.jpg">
    <div class="card-content">
      <h2 class="card-title">Linux Mint | Debian</h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 1,841
        <i class="fas fa-comments"></i> 6
        <i class="fas fa-heart"></i> 158
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
  <div class="card">
    <img src="https://pbs.twimg.com/media/EaXItBCVAAEUU_f?format=jpg&name=large">
    <div class="card-content">
      <h2 class="card-title">A Studio-JQ A</h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 2,179
        <i class="fas fa-comments"></i> 4
        <i class="fas fa-heart"></i> 158
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
  <div class="card">
    <img src="https://tse2.mm.bing.net/th?id=OIP.WjrBmE8MYrHVBaSiQiP_iwHaEn&pid=Api&P=0&h=180">
    <div class="card-content">
      <h2 class="card-title">Romain Trystram</h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 1,872
        <i class="fas fa-comments"></i> 8
        <i class="fas fa-heart"></i> 148
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
  <div class="card">
    <img src="https://tse4.mm.bing.net/th?id=OIP.D92VanNNtsE7kqEOFnjbwgAAAA&pid=Api&P=0&h=180">
    <div class="card-content">
      <h2 class="card-title">GNOME OS</h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 2,167
        <i class="fas fa-comments"></i> 9
        <i class="fas fa-heart"></i> 134
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
  <div class="card">
    <img src="https://tse4.mm.bing.net/th?id=OIP.q_QkT6vRP0M2qvMqQbOpqQHaEK&pid=Api&P=0&h=180">
    <div class="card-content">
      <h2 class="card-title">FSpace Station</h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 1,371
        <i class="fas fa-comments"></i> 9
        <i class="fas fa-heart"></i> 127
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
  <div class="card">
    <img src="https://wallpaperset.com/w/full/b/3/3/436108.jpg">
    <div class="card-content">
      <h2 class="card-title">Advertise Technologies</h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 728
        <i class="fas fa-comments"></i> 3
        <i class="fas fa-heart"></i> 118
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
  <div class="card">
    <img src="https://cdn.dribbble.com/userupload/15417820/file/original-ec3016842f085f024f3769c55d8f878d.jpg?resize=320x240&vertical=center">
    <div class="card-content">
      <h2 class="card-title"></h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 1,027
        <i class="fas fa-comments"></i> 6
        <i class="fas fa-heart"></i> 129
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
  <div class="card">
    <img src="https://cdn.dribbble.com/userupload/15411410/file/original-805da8f55afce317055cd4b4701cbfdd.jpg?resize=320x240&vertical=center">
    <div class="card-content">
      <h2 class="card-title"></h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 1,553
        <i class="fas fa-comments"></i> 9
        <i class="fas fa-heart"></i> 112
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
  <div class="card">
    <img src="https://cdn.dribbble.com/userupload/15419381/file/original-2940eedfc6203770cdb38969c94a2034.jpg?resize=320x240&vertical=center">
    <div class="card-content">
      <h2 class="card-title"></h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 940
        <i class="fas fa-comments"></i> 9
        <i class="fas fa-heart"></i> 107
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
  <div class="card">
    <img src="https://tse4.mm.bing.net/th?id=OIP.0-nHDLxizFgqOj4fJ-qv5AHaEL&pid=Api&P=0&h=180">
    <div class="card-content">
      <h2 class="card-title"></h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 1,177
        <i class="fas fa-comments"></i> 4
        <i class="fas fa-heart"></i> 102
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
  <div class="card">
    <img src="https://cdn.dribbble.com/userupload/15412492/file/original-3581fa0c1d455273fb12340b0f16995a.png?resize=320x240&vertical=center">
    <div class="card-content">
      <h2 class="card-title"></h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 1,100
        <i class="fas fa-comments"></i> 6
        <i class="fas fa-heart"></i> 93
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
  <div class="card">
    <img src="https://tse1.mm.bing.net/th?id=OIP.iluTdY_2__GZp40TTBfG_AAAAA&pid=Api&P=0&h=180">
    <div class="card-content">
      <h2 class="card-title"></h2>
      <div class="card-stats">
        <i class="fas fa-eye"></i> 1,445
        <i class="fas fa-comments"></i> 5
        <i class="fas fa-heart"></i> 101
      </div>
    </div>
    <div class="overlay">
      <p class="overlay-text">View Project</p>
    </div>
  </div>
</div>

<div class="pagination">
  <button class="active">1</button>
  <button>2</button>
  <button>3</button>
  <button>4</button>
  <button>5</button>
</div>

<footer class="footer">
  <p>&copy; 2023 Dribbble</p>
</footer>

<script src="https://kit.fontawesome.com/your-fontawesome-kit-id.js" crossorigin="anonymous"></script>
</body>
</html>
```
![Screenshot (168)](https://github.com/Saravanan123456789/css-advanced-project/assets/127467412/4b870354-caf3-4b57-b541-ff8234981001)
![Screenshot (169)](https://github.com/Saravanan123456789/css-advanced-project/assets/127467412/5c6d6f04-e262-4377-8d7a-a0e606d0daf1)
