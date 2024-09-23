# dicoding_landing_page
# index.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8"/>
    <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
    <title>Landing Page</title>
    <link rel="stylesheet" href="css/app.css"/>

    <!--SOCIAL MEDIA-->
    <link
    rel="stylesheet"
    href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css"
    integrity="sha512-1ycn6IcaQQ40/MKBW2W4Rhis/DbILU74C1vSrLJxCq57o941Ym01SwNsOMqvEBFlcgUa6xLiPY/NS5R+E6ztJQ=="
    crossorigin="anonymous"
    referrerpolicy="no-referrer"
  >

    <!--FONT-->
        <link rel="preconnect" href="https://fonts.googleapis.com">
        <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
        <link href="https://fonts.googleapis.com/css2?family=Quicksand:wght@300..700&display=swap" rel="stylesheet">
</head>

<body>
    <header class="navbar-container">
        <div class="logo">
            <img src="img/dicoding-header-logo.png" alt="Dicoding Indonesia">
        </div> 
        <nav class="nav-list">
            <ul>
                <li><a href="#">Beranda</a></li>
                <li><a href="#">Menu</a></li>
                <li><a href="#">Apa yang Baru?</a></li>
                <li><a href="#">Kontak</a></li>
            </ul>
        </nav>
    </header>
    <main> 
        <div class="content">
            <div class="content-description">
                <h1 class="title">DICODING INDONESIA</h1>
                <p> Kami yakin pendidikan teknologi adalah fondasi bagi setiap bangsa agar menjadi yang
                    terdepan dalam menghadapi dunia digital. Dicoding hadir sebagai platform pendidikan
                    teknologi yang membantu menghasilkan talenta digital berstandar global. Semua demi
                    mengakselerasi Indonesia agar menjadi yang terdepan.
                </p> 

                <button>Lebih Lanjut</button>

            </div>
            <div class="content-image">
                <img src="img/circle-g.jpg"/>
            </div>
        </div>

        <aside>
            <div class="social-media">
                <ul>
                    <li><a href="#"><i class="fab fa-instagram"></i></a></li>
                    <li><a href="#"><i class="fab fa-linkedin"></i></a></li>
                    <li><a href="#"><i class="fab fa-twitter"></i></a></li>
                    <li><a href="#"><i class="fab fa-facebook"></i></a></li>
                </ul>
            </div>
        </aside>
    </main>
</body>
</html>


# CSS
*,
*::before,
*::after {
  box-sizing: border-box;
}

body{
    font-family: 'Quicksand',sans-serif;
    height: 100vb;
    margin: 0;
    display: flex;
    flex-direction: column;
}

header.navbar-container {
    width: 100%;
    max-width: 1200px;
    padding-block: 1rem;
    margin-inline: auto;

    display: flex;
    justify-content: space-around;
    align-items: center;
    z-index: 9999;
}

header.navbar-container .logo img {
    width: 150px;
}

header.navbar-container .nav-list ul {
    padding-left: 0%;
    display: flex;
    justify-content: center;
    gap: 2rem 1rem;
}

header.navbar-container .nav-list li {
    list-style-type: none;
}

header.navbar-container .nav-list li a {
    padding: 0.5rem 1.5rem;
    border-radius: 999px;
    text-decoration: none;
    font-size: 1.05rem;
    font-weight: 500;
    color: black;
    transition: all 0.2s ease-in-out;
}

header.navbar-container .nav-list li:hover a {
    background-color: #425c77;
    color: white;
}

main {
    flex: 1;
    width: 100%;
    max-width: 1200px;
    margin-inline: auto;
    padding: 2rem 4rem;
    display: flex ;
    align-items: center;
}

main .content{
    flex: 1;
    display: flex;
    align-items: center;
}

main .content .content-description{
    flex: 1 1;
}

main .content .content-description .title{
    margin-block: 1rem;
    font-size: 3.5rem;
}

main .content .content-description p {
    font-size: 1.2rem;
    line-height: 1.7rem;
}

main .content .content-description button {
    padding: 0.8rem 2.5rem;
    border: 3px solid transparent;
    border-radius: 999px;
    margin-block-start: 1rem;
    background-color: #2d3e50;
    font-family: 'Quicksand',sans-serif;
    text-transform: uppercase;
    font-size: 1rem;
    font-weight: 700;
    color: white;
    cursor: pointer;
    transition: all 0.15 ease-in;
}

main .content-description button:hover {
    border: 3px solid #2d3e50;
    background-color: transparent;
    color: #2d3e50;
}

main .content .content-image {
    flex: 1;
    display: flex;
}

main .content .content-image img {
    width: 300px;
    min-width: 250px;
    margin: auto;
}

main aside {
    position: fixed;
    inset-block: 0;
    inset-inline-end: 0;
}

main aside .social-media {
    height: 100%;
    display: flex;
}

main aside .social-media ul {
    padding: 1.5rem 1rem;
    border-top-left-radius: 12px;
    border-bottom-left-radius: 12px;
    margin: auto;
    background-color: #2d3e50;

    display: flex;
    flex-flow: column nowrap;
    align-items: center;
    justify-content: center;
    gap: 1.5rem;
}

main aside .social-media li {
    list-style-type: none;
}

main aside .social-media li a {
    text-decoration: none;
    font-size: 1.5rem;
    color: white;
    transition: all 0.1s ease-in-out;
}

main aside .social-media li a:hover {
    color: #89b0d9;
}
@media screen and (max-width: 768px){
    header.navbar-container {
        flex-direction: column;
    }
}
header.navbar-container .nav-list ul {
    flex-wrap: wrap;
    column-gap: 0.5rem;
}

main {
    padding: 1rem 3rem;
}

main .content {
    flex-direction: column;
    gap: 2rem
}


main .content .content-description .title {
    font-size: 3rem;
}

main .content-description p {
   font-size: 1rem;
}

main .content .content-image{
    order: -1;
}

