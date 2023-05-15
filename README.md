# projetodia15
Projeto alcides para o dia 15/05/2023

exemplo aula 10

@media only screen and (max-width: 767px){

    header{ display: block; }

    nav ul{ padding: 0; }

    nav ul li a span {display: none;}

    h1{font-size: 30px;}

    .imagem-lado { flex-direction: column; }

    .imagem-lado div { width: 100%; }

    .imagem-lado:nth-child(1){ margin-right: 0; }

    #item1 p, #item1 h3 {text-align: center;}
    
    .imagem-lado p {  text-align: center; }

    .imagem-lado h3 {text-align: center; }
    
    iframe { max-width: 100%;}
}

/*Dentro do header Mobile (header-collapse):*/
@media only screen and (max-width: 780px) {
    .header-mobile {
        width: 100%;
        position: fixed;
    }

    .header-collapse {
        background-color: #fff;
        box-shadow: 1px 1px 4px 0 rgba(0, 0, 0, .1);
        position: fixed;
        margin-top: 7em;
        width: 100%;
        display: block;
        z-index: 3;
    }

    .header-collapse ul {
        margin: 0;
        padding: 0;
        list-style: none;
        overflow: hidden;
        background-color: #fff;
    }

    .header-collapse li a {
        color: #000;
        padding: 8px;
        display: block;
        border-right: 1px solid #f4f4f4;
        text-decoration: none;
    }

    .header-collapse li a:hover,
    .header-collapse .menu-btn:hover {
        background-color: #f4f4f4;
    }

    .header-collapse .menu {
        clear: both;
        max-height: 0;
        transition: max-height .2s ease-out;
    }

    .header-collapse .menu-icon {
        cursor: pointer;
        display: inline-block;
        padding: 28px 20px;
        position: relative;
        user-select: none;
    }

    .header-collapse .menu-icon .navicon {
        background: #333;
        display: block;
        height: 2px;
        position: relative;
        transition: background .2s ease-out;
        width: 18px;
    }

    .header-collapse .menu-icon .navicon:before,
    .header-collapse .menu-icon .navicon:after {
        background: #333;
        content: '';
        display: block;
        height: 100%;
        position: absolute;
        transition: all .2s ease-out;
        width: 100%;
    }

    .header-collapse .menu-icon .navicon:before {
        top: 5px;
    }

    .header-collapse .menu-icon .navicon:after {
        top: -5px;
    }

    .header-collapse .menu-btn {
        display: none;
    }

    .header-collapse .menu-btn:checked~.menu {
        max-height: 240px;
    }

    .header-collapse .menu-btn:checked~.menu-icon .navicon {
        background: transparent;
    }

    .header-collapse .menu-btn:checked~.menu-icon .navicon:before {
        transform: rotate(-45deg);
    }

    .header-collapse .menu-btn:checked~.menu-icon .navicon:after {
        transform: rotate(45deg);
    }

    .header-collapse .menu-btn:checked~.menu-icon:not(.steps) .navicon:before,
    .header-collapse .menu-btn:checked~.menu-icon:not(.steps) .navicon:after {
        top: 0;
    }
}
/*Dentro do Header Mobile:*/
@media (min-width: 48em) {
    .header-collapse li {
        float: left;
    }

    .header-collapse li a {
        padding: 20px 30px;
    }

    .header-collapse .menu {
        clear: none;
        max-height: none;
    }

    .header-collapse .menu-icon {
        display: none;
    }
}