# Usando-Flexbox-Posiciones
*Practicando los usos básicos de Flexbox y posiciones
```javascript
.header-sitio {
    
    background-color: #03A9F4;
    padding: 0 20px;
    /* Flex aqui*/
    display: flex;  
    flex-direction: column;      
}
@media screen and (min-width:768px) {
    .header-sitio {
        /* Flex aqui*/
        flex-direction: row;
        justify-content: space-between;
    }
}
.header-sitio h1 {
    color:white;
}

nav {
    /* Flex aqui*/
    align-self: center;
}
nav a {
    color: white; 
    font-family: 'IBM Plex Serif', serif;
    text-decoration: none;
}

.contenedor {
    background-color: rgb(60, 67, 105);
    min-height: calc( 100vh - 20px );
    max-width: 1000px;
    margin: 0 auto;
    padding: 20px 30px 0 30px;
}
h1, h2 {
    text-align: center;
    font-family: 'IBM Plex Serif', serif;
}
h2 {
    color:white;
}

.contenedor-flex {
    margin-top: 20px;
    /* Flex aqui*/
    display: flex;
    flex-direction: column;
}
@media screen and (min-width:768px) { 
    .contenedor-flex {
       /* Flex aqui*/
       flex-direction: row;
    }
}

.principal {
    /* Flex aqui*/
    order: 2;
}
aside {
    /* flex aqui*/
    margin-bottom: 1rem;/*Celular. Separacion entre el blog y servicios*/
}

aside {
    background-color: #03A9F4;
}
@media screen and (min-width:768px) {
    .principal {
        /* Flex aqui*/ 
        flex: 0 1 60%; 
        margin-right: 1rem; /*Para separar SErvicios de nuestro blog*/
        order: -1;/* Nos garantiza que es el primer elemento que se verá*/
    }
    aside {
        /* Flex aqui*/
        flex: 1; /* tomará el espacio restante del 60%*/
    }
}

.servicios .servicio {
    /* Flex aqui*/
    
}
@media screen and (min-width:768px) {
    .servicios {
        /* Flex aqui*/
        display: flex;
        
    }
    .servicios .servicio {
        /* Flex aqui*/
        /* flex-grow: 1; */
         flex: 1;
    }
}

.servicio {
    padding: 5px;
    background-color: #E53935;
}


.servicio:nth-child(2) {
    background-color: #8E24AA;
}

.servicio:nth-child(3) {
    background-color: #3F51B5;
}

footer {
    height: 100px;
    background-color: #8E24AA;
    margin-top: 20px;    
    /* Flex aqui*/
    display: flex;
    justify-content: center;
    align-items: center;
}
footer p {
    color: white;
}
.ul-centrar {
    margin-left: 30px;
}
```
