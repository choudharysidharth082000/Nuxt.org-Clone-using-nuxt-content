<template>
<div class="containor">
  <div class="navbarcontainor">
    <Navbar />
  </div> 
  

  <Mobileviewsidebar />
  
  

 
  <div class="containor_items">

    <div class="sidebar">

      <Tutorial />

    </div>
    <div class="maincontent">

      <h1>{{page.title}}</h1>
      
      <p><nuxt-content :document="page" /></p>

      <div class="csbfilecontainor">
          <iframe :src="page.csb_link"
     style="width:100%; height:500px; border:0; border-radius: 4px; overflow:hidden;"
     title="vigilant-leavitt-3264r"
     allow="accelerometer; ambient-light-sensor; camera; encrypted-media; geolocation; gyroscope; hid; microphone; midi; payment; usb; vr; xr-spatial-tracking"
     sandbox="allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
   ></iframe>

      </div>

    
    </div>



  </div>

  <div class="newsletter">
    <Newsletter/>
  </div>
  
    <div class="footer1">
      <Footer2 />
    </div>

   
  
  
  
  
  </div>  
 
</template>

<script>

import Newsletter from '../components/Newsletter.vue'
import Navbar from '../components/Navbar.vue'
import Tutorial from '../components/Tutorial.vue'
import Footer2 from '../components/Footer2.vue'
import Mobileviewsidebar from '../components/Mobileviewsidebar.vue'
export default {
  components:
  {
    Navbar,
    Tutorial,
    Newsletter,
    
    Footer2,
    Mobileviewsidebar

  },
  async asyncData ({ $content }) {
    const page = await $content('hello-world').fetch()

    return {
      page
    }
  },
 
}
</script>
<style scoped>

*
{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  
}
.footer1
{
  height: 300px;
  width: 100%;
  
}
.mobileviewsidebar
{
  height: 100vh;
  width: 100%;
  
  display: flex;
  flex-direction: row;
  
  
}
.leftview 
{
  height: 100%;
  width: 100%;
  background-color: #f8fafc;


}
.newsletter 
{
  margin-top: 240px;
  width: 100%;
  height: 300px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.containor
{
  display: flex;
  flex-direction: column;
  height: 100%;
  width: 100%;
  justify-content: center;
  align-items: center;
  

}
.navbarcontainor
{
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-left: -70px;
  
}


.containor_items 
{
  
  height: 100vh;
  width: 80%;
  display: flex;

  

}
.sidebar 
{
  height: 80vh;
  

  flex: 0.7;
  
  

}
.maincontent
{
  flex: 2;
  padding: 30px;
  
}
.csbfilecontainor{
  width: 100%;
  height: auto;
  object-fit: contain;
 
  
}
h1
{
  
  color: #2f495ecb;
  margin-bottom: 20px;

}
.Learncontainor
{
  margin-top: 20px;
  margin-bottom: 20px;
  padding-top: 13px;
  padding-left: 20px;
  display: flex;
  justify-content: flex-start;
  align-items: center;
  
  height: 4rem;
  width: 100%;
  background-color: #f7fafc;
  border-left: 5px solid #cbd5e0;
}
.Learncontainor a
{
    color: #35bb80;
  
}
svg
{
  height: 60%;
  width: auto;
  padding-right: 20px;
  padding-top: -60px;
  margin-top: -14px;
  color: rgba(0, 0, 0, 0.541);
}
.h-6
{

  display: flex;
  justify-content: center;
  align-items: center;
}

@media screen and (max-width: 1400px){

  /* .sidebar{
    display: none;
  } */
  .maincontent
  {
    flex: 1;
  }
  .footer1
  {
    height: 600px;
  }
  
}
@media screen and (max-width : 1200px) {
  .sidebar 
  {
    display: none;
  }
  
}
</style>
