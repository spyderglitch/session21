 @import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;600&family=Poppins:wght@400;600&display=swap');
*{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
    color: white;

}
a{
    font-family: 'Open Sans', sans-serif;
}

.profile{
    height: 650px;
    width: 100%;
    background-image: url(./assets/profile-bg.png);
    background-repeat: no-repeat;
    background-attachment: fixed;
}

.profile>img{
    border-radius: 50%;
}

h1{
    font-size: 54px;
    border-radius: 10px;
    padding: 5px;
    background-color: #7EB38C;
}

p{
    font-size: 18px;
    font-family: 'Poppins', sans-serif;
    text-align: center;
}
.profile>p, .profile>a{
    background-color: #7EB38C;
    padding: 10px;
    font-family: 'Open Sans', sans-serif;
    border-radius: 10px;
}
.profile>a{
    margin-top: 25px;
    border: 1px solid #FFFFFF;
}

.about-me-container>p{
    margin-top:20px ;
}

h2{
    font-family: 'Open Sans', sans-serif;
    font-size: 36px;
}


.progress>progress{
    width: 300px;
}

.work img{
    height: 200px;
    width: 250px;
}

.card{
    margin: 10px;
    text-align: center;
    background-color: white;
    cursor: pointer;
    box-shadow: 2px 4px 3px -2px rgba(255,255,255,0.75);
-webkit-box-shadow: 2px 4px 3px -2px rgba(255,255,255,0.75);
-moz-box-shadow: 2px 4px 3px -2px rgba(255,255,255,0.75);
}
.card:hover{
    transform: scale(1.1);
}
.card>p{
    color: black;
}

.lets-talk{
    height: 300px;
    background-image:url(./assets/footer-final.png) ;
}


.lets-talk a{
    width: 150px;
    background-color: #7EB38C;
    padding: 10px 5px;
    text-decoration: none;
    border-radius: 5px;
}

.lets-talk-container>a:hover{
    font-weight: bold;
    color: black;
}

footer{
    background-color: black;
    text-align: center;
    color: #828282;
    padding: 10px;
}


/*Iteration 1  - Implement flex property to nav Bar */
.flex{
    display: flex;
}
/*Iteration 2 - Use flex property and style the nav bar*/
nav{
    position: fixed;
    height: 70px;
    width: 100%;
    background:#1E1E1E;
    justify-content: space-evenly;
    align-items: center;

}

nav>a{
    font-family: 'Open Sans', sans-serif;
    font-size: 16px;
    padding: 25px;
    text-decoration: none;
}

nav>a:hover{
    font-weight: bold;
    color: #7EB38C;
}
/*Iteration 3  - Implement flex property to about part */
.column{
    flex-direction: column;
    align-items: center;
    justify-content: center;
}
/*Iteration 4 -  Use Justify-content and Align-items to align about-me-container class*/
.about-me-container{
    width: 250px;
    text-align: center;
    justify-content: flex-start;
    align-items: space-evenly;
}
/*Iteration 5 -  Use Justify-content to style about and work div*/
.about, .work{
    min-height: 600px;
    background-color: #1E1E1E;
    justify-content: space-evenly;

}
/*Iteration 6 -  USe justify-content to style work,about-container, .lets-talk-container and skills  div */
.about-container{
    width: 100vw;
    justify-content: space-evenly;
}
.work{
    justify-content: space-evenly;
}
.lets-talk-container{
    height: 200px;
    width: 400px;
    text-align:center ;
    justify-content: space-evenly;
}
.skills{
    height: 600px;
    background-image: url(./assets/skills-bg-final.png);
    justify-content: space-evenly;

}
/*Iteration 7 -  Implement the flex wrapping to work-container*/
.work-container{
    width: 70%;
    justify-content: space-evenly;
    flex-wrap: wrap;
}
/*Iteration 8 -  Make your Website Mobile Responsive using @media query*/

@media only screen and (max-width: 600px){
    /* nav{

    } */
    nav>a{
        font-size: 10px;
        font-weight: 800;
        background-color:#7EB38C ;
        padding: 5px;
        border-radius: 5px;
    }
    nav>a:hover{
        color:black;
    }

    .about-container{
        flex-direction: column;
        align-items: center;
    }

    .about-me-container{
        margin: 7px;
    }
    .about, .work{
        padding: 10px;
    }
} 
