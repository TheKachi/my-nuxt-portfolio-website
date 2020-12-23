<template>
     <section class="section hero">
        
        <div class="tagline">
      
            <h1>Onyedikachi Nze-Ben</h1>
            <p>Front end web developer based in Lagos, Nigeria</p>
            
            <div class="sm-links">
                <i class="fa fa-github"></i>
                <i class="fa fa-linkedin"></i>
                <i class="fa fa-twitter"></i>
            </div>
        </div>
        <div class="hero-img">   
          <img  src="../assets/kachi.png" alt="A picture of me">
            
        </div>
  </section>
</template>

<style lang='scss' scoped>
    .hero {
        position: relative;
        display: flex;
        justify-content: space-around;
        height: 90vh;
        p {
            font-size: 1.5rem;
        }
        
    }

    .hero-img {
        align-self:center;
    }
#left {
     position: absolute;
     top: 20%;
     right: 0;
     z-index: 1;
 } 
    .tagline {
        align-self: center;
    }
    .sm-links {
        display: inline-block;
       justify-content: space-evenly;

        // justify-content: space-between;
    }
</style>
