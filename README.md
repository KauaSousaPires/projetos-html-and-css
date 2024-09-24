# projetos-html-and-css
 Projetos feitos usando linguagem html e CSS

 BLOG SEMANTICO 
 *HTML*
 
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" Content="IE=edge">
    <title> Blog Semântico </title>
    <link rel="stylesheet" href="css/style.css">

</head>
<body>
   
    <header>  <!-- sessão inicial -->
        <nav id="navbar"> <!-- barra de navegação -->
            <div  id="navbar-inner"> <!-- div nesse blog tem propósito apenas para o css -->
                <h2> Blog </h2>
                <ul id="nav-links"> 
                    <li> <a href="a"> Home </a> </li>
                    <li> <a href="a"> Categorias </a> </li>
                    <li> <a href="a"> Contato </a> </li>

                </ul>

            </div>
        </nav>
    </header>
    <div class="container">
        <main id="post-container"> 
            <article class="post">
                <img src="img/f1.jpg" alt="Passeio de barco">
                <h3 class="title"><a href="a"> Algum título </a> </h3>
                <p class="description"> Lorem ipsum, dolor sit amet consectetur adipisicing elit. Alias libero unde in. Incidunt nam laudantium 
                    rerum vel voluptatibus, nihil exercitationem. Perferendis, laudantium incidunt molestias sed error accusamus sapiente est 
                    officiis? </p>
                    <p class="author"> Por: Kauã Sousa Pires</p>
                    <a href="a"> Ler mais </a>
            </article>

            <article class="post">
                <img src="img/f2.jpg" alt="Cachoeira">
                <h3 class="title"><a href="a"> Outro título </a> </h3>
                <p class="description"> Lorem ipsum, dolor sit amet consectetur adipisicing elit. Alias libero unde in. Incidunt nam laudantium 
                    rerum vel voluptatibus, nihil exercitationem. Perferendis, laudantium incidunt molestias sed error accusamus sapiente est 
                    officiis? </p>
                    <p class="author"> Por: Kauã Sousa Pires</p>
                    <a href="a"> Ler mais </a>
            </article>

            <article class="post">
                <img src="img/f3.jpg" alt="Balões ao ar">
                <h3 class="title"><a href="a"> Mais um post blog  </a> </h3>
                <p class="description"> Lorem ipsum, dolor sit amet consectetur adipisicing elit. Alias libero unde in. Incidunt nam laudantium 
                    rerum vel voluptatibus, nihil exercitationem. Perferendis, laudantium incidunt molestias sed error accusamus sapiente est 
                    officiis? </p>
                    <p class="author"> Por: Kauã Sousa Pires</p>
                    <a href="a"> Ler mais </a>
            </article>
        </main>
        <aside id="sidebar">
            <section id="search-bar">
                <h4> Busca </h4>
                <form> 
                    <input type="text" placeholder="Pesquise no blog">
                    <input type="submit" value="Buscar">
                </form>
            </section>
            <section id="categories">
                <h4> Categorias </h4>
                <nav> 
                    <ul> 
                        <li> <a href="a"> Paisagens </a></li>
                        <li> <a href="a"> Aventuras </a></li>
                        <li> <a href="a"> Naturezas </a></li>
                        <li> <a href="a"> Viagens longas  </a></li>
                        <li> <a href="a"> Cachoeiras </a></li>
                        <li> <a href="a"> Diversão </a></li>
                    </ul>
                </nav>
            </section>
            <section id="tags"> 
                <h4> Tags </h4>
                <div id="tags-container"> 
                    <a href="a"> Lifestyle </a>
                    <a href="a"> Viagem </a>
                    <a href="a"> Barco </a>
                    <a href="a"> Trilha </a>
                    <a href="a"> Tirolesa </a>
                    <a href="a"> Rafting </a>
                    <a href="a"> Parapente </a>
                    <a href="a"> Escaladas </a>
                    <a href="a"> Florestas </a>
                    
                    


                </div>
            </section>
        </aside>
    </div>
    <footer id="footer"> 
        <h2> Blog </h2>
        <p> Os melhores registros de aventuras </p>
        <P> 2024 &copy; GANDALFxl</P>

    </footer>
</body>
</html>

*CSS*
/* Geral */
* {
    padding: 0;
    font-family: Georgia, 'Times New Roman', Times, serif;
    margin: 0;
}

ul{
    list-style: none;
}

a{
    text-decoration: none;
    color: #444;
    transition: 0.4s;
}

a:hover{
    color: #37a1f7;
}

/* navbar */
#navbar{
    padding: 1.5rem 2.5rem;
    border-bottom: 2px solid #ddd;

}

#navbar-inner{
    max-width: 1200px;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

#nav-links{
    display: flex;
    gap: 1rem;
}

/* conteúdo principal */
.container{
    max-width: 1200px;
    margin: 0 auto;
    display: flex;
    gap: 3rem; /*afastar um do outro */
    padding: 2rem 2.5rem;
}

#posts-container{
    flex: 3 1 0;
}

.post{
    margin-bottom: 2.5rem;
}

.post img{
    width: 100%;
    margin-bottom: 1rem;

}

.title,
.description,
.author{
    margin-bottom: 1rem;
}

.title{
    font-size: 2rem;
}

.author{
    color: #333;
    font-weight: bold;
}

/* barra lateral */
#sidebar{
    flex: 1 1 0;

}

#search-bar, 
#categories,
#tags {
    padding: 1.5rem;
    border: 1px solid #DDD;
    margin-bottom: 1rem ;
}

#search-bar h4,
#categories h4,
#tags h4{
    margin-bottom: 1.5rem;
    font-size: 1.6rem;
    
}

#search-bar form{
    display: flex;
}

#search-bar input{
    padding: .5rem 1rem;
    border: 1px solid #ddd;
}

#search-bar input[type="submit"]{
    cursor: pointer;
    background-color: #37a1f7;
    color: #FFF;
    border: none;
}

#categories li{
    margin-bottom: 1rem;
    
   
}

#tags-container{
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem;
}

#tags-container a{
    background-color: #DDD;
    padding: 0.5.rem 0.7.rem;
    border-radius: 0.3rem;
}

/* rodapé */ 
#footer{
    padding: 3rem;
    text-align: center;
    border-top: 2px solid #DDD;
}

#footer h2, 
#footer p{
    margin-bottom: 1rem;
}

/* responsivo */ 
@media(max-width: 450px){
    .container {
        flex-wrap: wrap;
    }
}
