<script>
  import '../styles.scss'
  import { onMount } from 'svelte';
  import spacedeb1 from '$lib/images/slides/spacedeb1.webp';
  import spacedeb2 from '$lib/images/slides/spacedeb2.webp';
  import spacedeb3 from '$lib/images/slides/spacedeb3.webp';
  import theft1 from '$lib/images/slides/theft1.webp';
  import theft2 from '$lib/images/slides/theft2.webp';
  import theft3 from '$lib/images/slides/theft3.webp';
  import { book, open_book, arrow, emoji, artist, gear, school, brain, oldsites, boring, habitual, morado, postcards, github, instagram, twitter, discord } from '$lib/images/images';
  
</script>
<nav class="navbar">
  <a href="#" id="title">
    <h2><span>W</span><span>i</span><span>l</span><span>l</span><span>i</span><span>a</span><span>m</span> <span>J</span><span>o</span><span>J</span><span>a</span><span>r</span><span>t</span><span>h</span></h2>
  </a>
  <div id="socials">
    <a href="https://github.com/wjojarth23" target="_blank" rel="noreferrer" aria-label="Go to William's Github"><img src={github} alt="github logo"/></a>
    <a href="https://discord.com/users/801117219945578516" target="_blank" rel="noreferrer" aria-label="Go to William's Discord"><img src={discord} alt="discord logo"/></a>
  </div>
</nav>
<br/>
<div class="body">
<h1 class="line">I use </h1><div class="figmabox"><img class= "figmalogo"src="src/lib/images/icons/figma.svg"/>Figma</div><h1 class="line">    a next generation design tool to create stunning visual effects</h1>

<br/>
<span>Get started with Figma for Education, and copy one of the decks below!</span>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>

<div class="presgrid">
<a class="set" href="https://www.figma.com/slides/1EcpzU2zz7mZxmoLrw4uML/AP-Seminar-TMP?node-id=137-159&t=zzW8H72RgUWRY7gA-1">
<div class="deck">
<img class="deckimg bot" src={spacedeb1}/>
<img class="deckimg mid" src={spacedeb2}/>
<img class="deckimg top" src={spacedeb3}/>

</div>
<h1>Black and Colorful</h1>
</a>
<a class="set" href="https://www.figma.com/slides/3YjFDb0VuYROF3HflRxOfs/Untitled?node-id=1-25&t=CE57cjrIMdz5HLiC-1">
<div class="deck">
<img class="deckimg bot" src={theft1}/>
<img class="deckimg mid" src={theft2}/>
<img class="deckimg top" src={theft3}/>

</div>
<h1>Black Impact</h1>
</a>
</div>
<div class="bottombar">More Coming Soon! <div class="centertext"> Want a deck made just for you? <a href= "mailto:100034323@mvla.net">Reach out to me!</a></div></div>
</div>
<style>
@mixin fade-up($duration, $delay) {
  animation-name: fade-up;
  animation-duration: $duration;
  animation-delay: $delay;
  animation-timing-function: cubic-bezier(0.33, 1, 0.68, 1);
  animation-fill-mode: forwards;
  transform: translateY(1em);
  opacity: 0;
}
@keyframes fade-up {
  from {
    transform: translateY(1em);
    opacity: 0;
  }
  to {
    transform: translateY(0);
    opacity: 1;
  }
}
.presgrid{
  display: flex;
}
h1{
  font-family: articulat-cf, sans-serif;
  font-size:40px;
  display:inline-block;
  
}

.bottombar{
  background:#ffffff;
  border: 1px solid #000000;
  padding:60px;
  width:1400px;
  border-radius:25px;
  text-align:center;
  margin-top:100px;
}
.mid{
  opacity:80%;
}
a{
  color:black;
}
.top{
  opacity:100%;
}
.bot{
  opacity:40%;
}
.deckimg{
  width:500px;
  border-radius:25px;
  display:inline-block;
  margin-left:-460px;
  transform:translate(460px,0px);
  transition: 2s;
  border: 1px solid #000000;
}
.deckimg:hover{
  width:500px;
  border-radius:25px;
  display:inline-block;
  margin-left:-400px;
  transform:translate(400px,0px);
  opacity:100% !important;
}
.body{
  margin-top:6rem;
  margin-left:6rem;
  margin-right:6rem;
  @include fade-up(1.5s, 2.5s);
}
.deck{
width:800px;
}
.figmalogo{
  height:40px;
  transform: translate(0px, 5px);
  margin-right:10px;
  @include fade-up(1.5s, 2.5s);
  transition: 0.2s ease-in-out;
}
.figmabox{
  background:#E0E0E0;
  padding:6px;
  margin-left:10px;
  margin-right:10px;
  font-weight:700;
  font-size:40px;
  border-radius: 10px;
  width:170px;
  display:inline-block;
}
</style>