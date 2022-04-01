<template>
  <div style="width: 960px; margin: 0 auto; padding-top: 80px; padding-bottom: 80px;"> 
<h1>Testimonials</h1>
    
    <div class="testimonial-quote group">
        <img src="https://i.postimg.cc/0NzN80k9/craig.jpg">
        <div class="quote-container">
            <blockquote>
                <p>Tursha is an extremely observant and intelligent person, and has an innate ability paired with  well developed social skills to quickly learn her environment and adapt to it. Not only that but she knows how to get along with many people from different walks of life which makes her the perfect candidate to incorporate into any work environment.</p>
            </blockquote>  
            <cite><span>Craig Braaf</span><br>
                Frontend Web Developer<br>
                
            </cite>
        </div>
    </div>    
        
    <hr style="margin: 60px auto; opacity: .5;">
  
            
    <div class="testimonial-quote group right">
        <img src="https://i.postimg.cc/wMj5tc9F/alex.jpg">
        <div class="quote-container">
            <div>
                <blockquote>
                    <p>Tursha is a hard worker and thrives to produce quality work.”</p>
                </blockquote>  
                <cite><span>Alex Sexwale</span><br>
                    Lecturer<br>
                    
                </cite>
            </div>
        </div>
    </div>     

    <hr style="margin: 60px auto; opacity: .5;">

           
    <div class="testimonial-quote group">
        <img src="https://i.postimg.cc/vHPqvTjc/haniah.jpg">
        <div class="quote-container">
            <div>
                <blockquote>
                    <p>Overall, fantastic! I'd recommend them to anyone looking for a creative, thoughtful, and professional team.”</p>
                </blockquote>  
                <cite><span>Haniah Jardien</span><br>
                    Full-stack web developer<br>
                    
                </cite>
            </div>
        </div>
    </div>   
      
    <hr style="margin: 60px auto; opacity: .5;">
    
    
    <div class="testimonial-quote group right">
        <img src="https://i.postimg.cc/jjvLWVC0/20211109-111026.jpg">
        <div class="quote-container">
            <blockquote>
                <p>Overall, fantastic! I'd recommend them to anyone looking for a creative,<br> thoughtful, and professional team.”</p>
            </blockquote>  
            <cite><span>Enosh Elliott</span><br>
                Full-stack web developer<br>
                
            </cite>
        </div> 
    </div>

    <hr style="margin: 60px auto; opacity: .5;">

<div class="testimonial-quote group">
        <img src="https://i.postimg.cc/xTDGmyh0/Muneeb-min.jpg">
        <div class="quote-container">
            <blockquote>
                <p>Tursha is good at critical thinking as well as using her time well enough to complete the given task.”</p>
            </blockquote>  
            <cite><span>Mugammad Muneeb Davids</span><br>
                Full-stack web developer<br>
                
            </cite>
        </div>
    </div>    
        
    <hr style="margin: 60px auto; opacity: .5;">
  
            
    <div class="testimonial-quote group right">
        <img src="https://i.postimg.cc/X7vxX3J3/tony.jpg">
        <div class="quote-container">
            <div>
                <blockquote>
                    <p>Overall, fantastic! I'd recommend them to anyone looking for a creative, thoughtful, and professional team.”</p>
                </blockquote>  
                <cite><span>Ndiphiwe Ngxola</span><br>
                    Full-stack web developer<br>
                    
                </cite>
            </div>
        </div>
    </div>     

    

</div>
</template>

<script>
export default {};
</script>
<style scoped>
h1 {
  padding-top: 40px;
}
html {
  background: #fff;
}

h1 {
  font-size: 45px;
  text-align: center;
  margin-bottom: 40px;
}

.testimonial-quote {
  font-size: 16px;
}

.testimonial-quote blockquote {
  /* Negate theme styles */
  border: 0;
  margin: 0;
  padding: 0;
  background: none;
  color: black;
  font-family:"Helvetica Neue",Helvetica,Arial,sans-serif;
  font-size: 1.5em;
  font-style: italic;
  line-height: 1.4 !important;
  margin: 0;
  position: relative;
  text-shadow: 0 1px white;
  z-index: 600;
}

.testimonial-quote blockquote * {
  box-sizing: border-box;
}

.testimonial-quote blockquote p {
  color: #000;
  line-height: 1.4 !important;
}

.testimonial-quote blockquote p:first-child:before {
  content: '\201C';
  color: gray;
  font-size: 7.5em;
  font-weight: 700;
  opacity: .3;
  position: absolute;
  top: -.4em;
  left: -.2em;
  text-shadow: none;
  z-index: -300;
}

.testimonial-quote img {
  border: 3px solid #000;
  border-radius: 50%;
  display: block;
  width: 120px;
  height: 120px;
  position: absolute;
  top: -.2em;
  left: 0;
}

.testimonial-quote cite {
  color: red;
  display: block;
  font-size: .8em;
}

.testimonial-quote cite span {
  color: blue;
  font-size: 1em;
  font-style: normal;
  font-weight: 700;
  letter-spacing: 1px;
  text-transform: uppercase;
  text-shadow: 0 1px white;
}

.testimonial-quote {
  position: relative;
}
.testimonial-quote cite  {
  text-align: left;
}

.testimonial-quote .quote-container {
  padding-left: 160px;
}

.testimonial-quote.right .quote-container {
  padding-left: 0;
  padding-right: 160px;
}

.testimonial-quote.right img {
  left: auto;
  right: 0;
}

.testimonial-quote.right cite {
  text-align: right;
}

</style>
