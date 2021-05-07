<template>
  <v-content>
    <div class="staticHero">
      <v-img src="../assets/images/396602.jpg">
        <v-row align="end" class="lightbox white--text pa-2 fill-height">
          <v-col>
            <v-container>
              <!-- <div class="headline">About Me</div> -->
            </v-container>
          </v-col>
        </v-row>
      </v-img>
    </div>
    <div class="block">
      <v-container>
        <div class="container">
  <!-- <h1>This is the title of the article</h1> -->
  <div class="aside"><img src="../assets/images/angry.jpg" /></div><div id="blah" class="content">
    <h2>About me</h2>
<p>Bacon ipsum dolor sit amet frankfurter in laborum, biltong beef consectetur proident tri-tip eu laboris.  Esse exercitation beef ball tip salami.  Irure ham hock strip steak turducken beef ribs, shank ham filet mignon fugiat shoulder.  Hamburger eiusmod ea meatball, veniam biltong exercitation eu flank turducken cillum frankfurter officia rump minim.  Pariatur voluptate boudin commodo duis, nostrud mollit beef ribs sirloin pig shank cow.  Prosciutto duis filet mignon est enim bacon deserunt labore ex turkey voluptate spare ribs.  Esse est eu, voluptate culpa tenderloin pork loin in ad flank nostrud consequat laboris bacon ham.</p><p>Dolor chuck voluptate pig.  Jerky corned beef ham, short loin pancetta filet mignon jowl.  Dolore biltong ullamco, chuck adipisicing sausage dolore.  Ut ham hock dolore minim sirloin officia beef aute ground round tempor ad ribeye in irure.  Frankfurter flank dolor, shank mollit filet mignon laborum swine.</p><p>Pastrami velit ea bacon, culpa deserunt in kielbasa labore meatloaf elit dolor.  Et in duis, pancetta qui boudin fugiat ea adipisicing eu meatball.  Sirloin tempor do et salami proident ex cupidatat.  Pork adipisicing culpa enim cow short ribs ex id, bacon corned beef.</p><p>Irure shank beef ribs laborum id ut in shankle tenderloin.  Est anim aute, tail leberkas capicola eu salami ground round.  Non corned beef flank laboris salami hamburger jowl cupidatat irure fatback.  Eu chuck capicola jowl salami frankfurter, spare ribs eiusmod biltong meatball.</p><p>Venison pastrami pancetta esse ground round occaecat shoulder tempor salami ex aliquip.  Quis pork swine jowl meatball, andouille t-bone eu short ribs pork belly.  Prosciutto drumstick quis in.  Beef ribs tri-tip cow spare ribs tail pastrami magna.</p>
</div>

</div>
      </v-container>
    </div>
   
  </v-content>
</template>

<script>
export default {
  
}
</script>

<style lang="scss">

.v-content__wrap .block {
  border-bottom: none;
}

  * { color: white;-moz-box-sizing: border-box; -webkit-box-sizing: border-box; box-sizing: border-box; }

ul, li, p, html, body, h3 {
 padding: 0;
  margin: 0;
}

img {width: 100%;
    max-width: 100%;
}

body {
 font-size: 16px; 
 font-family: helvetica, arial, san-serif;
 background-color: #999;
 color: #333;
}
h1 {
  border-top: 0.3em solid #333;
}
p {
  font-size: 1em;
  line-height:1.6em;
  margin-bottom: 2em;
}

p:first-of-type{
    margin-top: 1.6em;
}

.container {
   width: 100%;
   max-width: 64em;
  margin: 0 auto;
}

.content{

  float:left;
  width: 100%;
  padding: 0 5%;
}

.aside {
  float:left;
  width: 100%;
  color: #f1f1f1;
  height: 300px;
  overflow:hidden;
  margin-bottom: 2em;
}

.footer{
  clear: both;
  background-color: #333333;
  width: 100%;
  height: 5em;
  float: right;
}

.footer a {
  color: #f0f0f0; 
  text-decoration: none; 
  line-height: 5em;
}
.footer a:hover {
  border-bottom: dashed 1px #999;
}


@media screen and (min-width:20em) {
 /*     20.000em /* (320 px)*/ 
   body { 
    background-color: #fff;
  }
}

@media screen and (min-width:30em) {
 /*         30.000em  /* (480 px)*/
 body { 
    background-color: #f1f1f1;
  }
}
  
@media screen and (min-width:31.25em) {
 /*     31.250em  /* (500 px)*/

}  
@media screen and (min-width: 37.5em) {
 /*   	37.500em  /* (600 px)*/
  
}
@media screen and (min-width:48em) {
 /*   	48.000em /*(ackkkkkk, device specific bad)768px*/
  .columns { 
  -webkit-column-count: 2; /* Saf3, Chrome*/
  -webkit-column-gap: 4%; /* Saf3, Chrome*/
  -moz-column-count: 2; /* FF3.5+ */
  -moz-column-gap: 4%; /* FF3.5+ */
  column-count: 2; /* Opera 11+*/
  column-gap: 4%; /* Opera 11+*/
}
}
@media screen and (min-width:50em) {
 /*   	50.000em  /* (800 px)*/
  .content{
  width: 80%;
}
  
 .aside {
   width: 20%; 
  }
  
}
@media screen and (min-width:60em) {
 /*   	60.000em /*(a designers fav)960px */
    .container {
  margin: 5em auto;
}
} 

@media screen and (min-width:64em) {
 /*   	64.000em /* (ackkkkk) 1024px */

} 
@media screen and (min-width:75em) {
 /*   	75.000em  /* (1200 px)*/
  
}  
  
  
@media screen and (min-width:87.5em) {
 /* 	87.500em  /* (1400 px)*/
/*  body {
    font-size: 1.1em;
  }*/
    
}  
  
@media screen and (min-width:100em) {
 /*   		100.000em  /* (1600 px)*/
  body {
    font-size: 1.4em;
  }
}  
  
 @media screen and (max-height:25em) {

  body {background-color: pink;}
  .content {
  -webkit-column-count: 2; /* Saf3, Chrome*/
  -webkit-column-gap: 4%; /* Saf3, Chrome*/
  -moz-column-count: 2; /* FF3.5+ */
  -moz-column-gap: 4%; /* FF3.5+ */
  column-count: 2; /* Opera 11+*/
  column-gap: 4%; /* Opera 11+*/
  }
}       
  


		
		
		
		
		
	
	
</style>