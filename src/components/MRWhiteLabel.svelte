<script>
    import { createEventDispatcher } from 'svelte';
    import Button from "../shared/Button.svelte";
 </script>

 <section><br>
      <h3 class="blue">Andrew Weatherall, la quintaesencia de la electrónica</h3><br>
      (MRWL_02)<br>
      <img src="/img/Andrew.jpg" alt="portada Andrew Weatherall" class="andy"><br>
 </section>
      <p>Andrew Weatherall (1963-2020): The Guv´nor. Lord Sabre. The Chairman.<br><br>
        Boy´s Own. The Sabres Of Paradise. Two Lone Swordsmen.<br>
        Acid. Post-Punk. Spacy Disco.<br>
        Cosmic. House. Techno.<br>
        Electro. Ambient. Dub.<br>
        Remixer. Productor. DJ.<br>
        Screamadelica. Dexter. Weekender.<br>
        The Asphodells. The Woodleigh Research Facility. Dayglo Maradona.<br>
        Lino Squares. Lords Of Afford. Rude Solo.<br>
        Wrong Meeting. A Love From Outer Space. Turntables & Machines.<br>
        The Haywire Sessions. 6 Mix. Music´s Not For Everyone.<br>
        Bohemio. Agudo. Sarcástico.<br>
        100 bpms. 120 bpms. 140 bpms.<br>
        La quintaesencia de la electrónica: Andrew Weatherall.<br><br>
        «Andrew no seguía las modas. Pinchaba lo que quería pinchar, hacía lo que quería hacer 
        y producía con la gente con la que quería producir. 
        Creo que esa es la razón por la que era tan respetado» -Paul Oakenfold-.</p><br>

        <section><br>
            <h3 class="blue">R&S Records, el Ferrari de doce pulgadas</h3><br>
            (MRWL_01)<br>
            <img src="/img/r&s.jpg" alt="portada R&S Records" class="ferrari"><br>
        </section>
       <p>A finales de los 80, unos misteriosos y fantásticos doce pulgadas estampados 
        con el logo de la marca de automóviles Ferrari comienzan a poblar las estanterías 
        de las mejores tiendas de discos de importación.<br><br>
        R&S Records se convertirá en el sello favorito de miles de ravers europeos, 
        y la leyenda del sello belga no hará más que crecer y crecer: 
        Public Relation, Aphex Twin, Cisco Ferreira, Derrick May, Jaydee, Capricorn, 
        Model 500, Kenny Larkin, Carl Craig, Joey Beltram... 
        El cénit de la electrónica mundial.</p><br> 
<style>
  .andy, .ferrari {
      border-radius: 5px;
      transition: width 0.1s, height 0.1s;
      display: block;
      margin: 0px auto;
      width: 200px;
  }
  .andy:hover, .ferrari:hover {
      border-radius: 5px;
      transition: width 0.1s, height 0.1s;
      display: block;
      margin: 0px auto;
      width: 220px;
  }
  @media screen and (max-width: 650px) {
  .andy, .ferrari {
      width: 70vw;
  }
  }
</style>


 