<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <link rel="stylesheet" href="style.css">
        <title>Navigation Dropdown</title>
    </head>
    <body style="background-color: orange;">
        <div class="nav__bars">
        <ul>
            <li>
            </li>
        </ul>
        </div>
        <div class="nav__bar">
        <ul>
            <li><a href="#">Home</a></li>
            <li>
                <a href="#">Tutorials <i class="fas fa-caret-down"></i></a>
                     <div class="dropdown__nav">
           <ul>
             <li><a href="#">Photoshop </a></li>
             <li><a href="#">Illustrator</a></li>          <li>
                 <a href="#">Web Design</a> <i class="fas fa-caret-down"></i></a>
             <div class="dropdown__nav-1">
                 <ul>
                     <li><a href="#">HTML</a></li>
                     <li><a href="#">CSS</a></li>
                            </ul>
                        </div>
                    <div>
                     </li>
                    
                    </ul>
                </div>  
                    
            </li>    

            <li><a href="#">Articles</a></li>
            <li><a href="#">Inspiration</a></li>
        </ul>

        </div>

        <br>
        <br>
        <br>
    </body>



</html>

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: sans-serif;
}
.nav__bars {
    background-color: orange;
}

.nav__bar {
    background: linear-gradient(rgb(66, 66, 66), #373737);
    border: 10px;
    height: 80px;
    width: 100%;
    display: flex;
    align-items: center;
}

.nav__bar ul{
    margin-left: 10px;
    list-style: none;
    display: flex;
}

.nav__bar ul li {
    background-color: lightgray;
    border-radius: 5px;
    margin-right: 30px;
    padding: 10px 20px;
    word-spacing: normal;

}

.nav__bar ul li:hover {
    background-color: rgb(255, 106, 52)
}

.nav__bar ul li a {
    color: black;
    text-decoration: none;
    font-size: 20px;


    
}

.nav__bar ul li a:hover {
    color: white;

}

.dropdown__nav {
    display: none;
}

.dropdown__nav ul li:hover {
    background-color: blue;
    border-style: solid;
    border-color: blue;
    border-width: 5px 50px 5px 5px;
    border-right: orangered;
}

.nav__bar ul li:hover .dropdown__nav {
    display: block;
    position: absolute;
    left: 135px;
    top: 8%;
    background-color: blue;
}

.nav__bar ul li .dropdown__nav ul {
    display: block;
    margin: 10px;
}

.nav__bar ul li .dropdown__nav ul li {
    width: 150px;
    padding: 10px;
}

.fas {
    float: right;
    margin-left: 10px;
    padding-top: 3px;
}

.dropdown__nav-1{
    display: none;
}

.dropdown__nav ul li:hover .dropdown__nav-1 {
    display: block;
    position: absolute;
    top: 0;
    left: 200px;
    background-color: violet;
    border-color: violet;
}
