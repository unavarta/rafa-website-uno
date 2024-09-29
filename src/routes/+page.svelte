<script>
        import Youtube from "svelte-youtube-embed"

   function redirectWhatsapp(){
        window.location.href = 'https://wa.me/5492617680891';
    }
</script>



<section>
    
<div class="container">
    <div class="horizontal-div">
      <img src="src\img\logo.jpeg" alt="">
    </div>
    <div class="horizontal-div">
<div class="yt">
    <p>Dueño y jefe técnico, Rafael, en acción</p>
    <Youtube class="unovideo" id="1x3q4Qb4MBo" width="10px"
    />
</div>
       </div>
    <div class="center-div">
        <div class="inner-container">
            <div class="title-div">HORARIOS</div>
            <div class="content-div">
                <ul>
                    <li> L-V: 09:00hs a 19:00hs</li>
                    <li> SAB: 09:00hs a 17:00hs</li>
                    <li> DOM: 09:00hs a 13:00hs</li>
                </ul>
            </div>
        </div>
        <div class="inner-container">
            <div class="title-div">METODOS DE PAGO</div>
            <div class="content-div">
                <ul>
                    <li>TARJETAS CRÉDITO/DÉBITO</li>
                    <li>MERCADOPAGO</li>
                    <li>TRANSFERENCIAS ELECTRÓNICAS</li>
                </ul>
            </div>
        </div>
        <div class="inner-container">
            <div class="title-div">DIRECCION</div>
            <div class="content-div">  
                <p>CHILE 2636, CIUDAD DE MENDOZA</p>
            </div>
        </div>
        <div class="inner-container">
            <div class="title-div">REPARACIONES</div>
            <div class="content-div">
                <p>Todas las marcas, especializados en Alemanes</p>
            </div>
        </div>
    </div>
    <div class="inner-container">
        <div class="title-div">ATENCIÓN DE EMERGENCIAS</div>
        <div class="content-div">
            <p class="textemergencia">Contamos con una camioneta equipada con herramientas de todo tipo para cualquier emergencia. <br>  ¿Te quedaste tirado? Peganos un llamado.
            </p>
            <p class="textemergencia">
               
            <button on:click={redirectWhatsapp}>Nuestro WhatsApp</button>
        </div>
    </div>
    <p class="derecho">Derechos Reservados. 2019 Navarta Tecnica</p>
</div>
    
</section>


<style>
    .derecho{
        color: white;
    }
    .yt {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        margin-bottom: 10px;
    }
 
  :global(body) {
        background-color: black; /* New light blue background for the body */
        font-family: 'Gill Sans', 'Gill Sans MT', Calibri, 'Trebuchet MS', sans-serif 
    }
    section img {
        width: 800px;
        max-width: 800px;
    }
    section  {
        
        
      margin: 0;
      height: 100vh; /* Full viewport height */
      display: flex;
      justify-content: center; /* Centers the container horizontally */
      align-items: center;     /* Centers the container vertically */
      /* New light gray background for the body */
  }

  button{
    background-color: forestgreen;
    width: 150px;
    height: 50px;
    border: 0px;
    color: white;
    transition: 0.3s background-color, 0.3s color;    
}

  button:hover{
    background-color: grey;
    color: #202020;
  }
  .container {
    
      display: flex; /* Enables flexbox layout */
      flex-direction: column; /* Stacks child divs vertically */
      height: 100%; /* Full height of the viewport */
      max-width: 800px; /* Set a max width for the container */
      width: 100%; /* Allow full width up to max-width */
      margin: 0 auto; /* Center the container horizontally */
  }

  .horizontal-div {
      flex: 1; /* Allows the divs to grow and fill available space */
      background-color: #242424; /* Bootstrap blue color */
      color: white; /* Text color */
      display: flex; /* Center text inside */
      justify-content: center; /* Center text horizontally */
      align-items: center; /* Center text vertically */
      border-radius: 4px; /* Rounded corners for individual divs */
      border: 1px solid #ccc; /* Light gray border */
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2); /* Subtle shadow */
      transition: background-color 0.3s ease; /* Smooth transition */
      border: 0.5px solid black;
  }

 

  .center-div {
    
      flex: 1.5; /* Makes the center div larger */
      display: flex; /* Enable flexbox for inner divs */
      flex-direction: row; /* Align inner divs horizontally */
      align-items: stretch; /* Ensure inner divs are tall */
      background-color: #202020; /* Darker blue for visibility */
      border-radius: 4px; /* Rounded corners */
      padding: 0; /* Remove padding */
      border: 0.5px solid black;
  }

  .inner-container {
    
    border: 0.5px solid black;
      flex: 1; /* Each inner container takes equal space */
      display: flex; /* Enable flexbox for title and content */
      flex-direction: column; /* Stack title and content vertically */
  }

  .title-div {
      flex: 0 0 25%; /* Title takes up 25% of the inner container height */
      background-color: #3d3d3d; /* Darker color for the title */
      color: white; /* Text color */
      display: flex; /* Center text inside */
      justify-content: center; /* Center text horizontally */
      align-items: center; /* Center text vertically */
      font-size: 16px; /* Font size for the title */
      border-radius: 4px 4px 0 0; /* Rounded corners on the top */
  }

  .content-div {
      flex: 1; /* Content takes up remaining space (75%) */
      background-color: #242424; /* Inner div color */
      color: white; /* Text color */
      display: flex; /* Center text inside */
      justify-content: center; /* Center text horizontally */
      align-items: center; /* Center text vertically */
      border-radius: 0 0 4px 4px; /* Rounded corners on the bottom */
        display: flex;
        flex-direction: column;
    }

    .content-div p {
        font-size: 15px;
        line-height: 20px;
        text-align: center;
    }

@media (max-width: 600px) {
    .horizontal-div {
        font-size: 14px; /* Smaller text on small screens */
    }
    .center-div {
        flex: 1; /* Reduce its size on smaller screens */
    }
}
</style>