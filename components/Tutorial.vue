<!-- Please remove this file from your project -->
<template>
  <div class="containor_sidebar">

    <h4>version <span>2.15.2</span></h4>
    <div class="sidebar_containor">
      <h5 class="sideheader">ROUTING</h5>
      <a href="#">Hello World</a>
      <a href="/activelink">Active Link Class</a>
      <a href="#">Dynamic Pages </a>
      <a href="#">Nested Pages</a>
      
      
    </div>
    
    
    <div class="sidebar_containor">
      <h5 class="sideheader">DATA FETCHING</h5>
      <a href="#">Asyncdata Hook</a>
      <a href="#">fetch Hook</a>
      
      
    </div>
    
    <div class="sidebar_containor">
      <h5 class="sideheader">ASSET MANAGEMENT</h5>
      <a href="#">webpack Assets</a>
      <a href="#">Pre-processors</a>
      
      
    </div>
    
    
    <div class="sidebar_containor">
      <h5 class="sideheader">TRANSITIONS</h5>
      <a href="#">Nuxt transitions</a>
      
      
      
    </div>
    
    <div class="sidebar_containor">
      <h5 class="sideheader">SEO</h5>
      <a href="#">SEO HTML Head</a>
      <a href="#">SEO Twitter and Open Grapgh</a>
      
      
    </div>
    
    <div class="sidebar_containor">
      <h5 class="sideheader">LOADING</h5>
      <a href="#">Customize Nuxt Loading</a>
      <a href="#">Customized Nuxt Loading Indicator</a>
      <a href="#">Custom Loading Component</a>
      
      
    </div>
    
    <div class="sidebar_containor">
      <h5 class="sideheader">MISCELLANEOUS</h5>
      <a href="#">Layouts</a>
      <a href="#">Lazy Loading Components</a>
      <a href="#">Vuex Store</a>
      <a href="#">Nuxt Helpers</a>
      
      
    </div>
    
    <div class="sidebar_containor">
      <h5 class="sideheader">MIDDLEWARE</h5>
      <a href="#">Router Middleware</a>
      <a href="#">Named Middleware</a>
      <a href="#">Anonymous Middleware</a>
      
      
    </div>
    
    <div class="sidebar_containor">
      <h5 class="sideheader">PLUGINS</h5>
      <a  href="#">Vue Plugins</a>
      <a href="#">Client Only Plugins</a>
      <a href="#">External Packages Plugin</a>
      <a href="#">Custom Plugins</a>
      
      
    </div>
    
    <div class="sidebar_containor">
      <h5 class="sideheader">MODULES</h5>
      <a href="#">Local Modules</a>
      <a href="#">Axios Usage</a>
      
      
    </div>
    
    

  </div>
</template>
<script>
export default {
  
}
</script>
<style scoped>
*
{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  transition: all 0.4s ease;
  /* display: none; */
}
.containor_sidebar 
{
  height: 100%;
  width: 100%;
  background-color: white;
  display: flex;
  flex-direction: column;
  overflow-y: scroll ;
  display: flex;

}

.sidebar_containor
{
  
  width: 100%;
  height: auto;
  margin-bottom: 20px;
  
}

h4
{
  padding: 10px;
  color: rgba(0, 0, 0, 0.651);
  font-size: 1.1rem;
  font-weight: 500;
  margin-bottom: 20px;
}
.sideheader
{
  padding: 10px;
  color: rgba(0, 0, 0, 0.568);
  font-size: 1.09rem;
  font-weight: 500;
  margin-bottom: 20px;
  
}
span
{
  color: #35bb80;
  font-weight: 500;
  font-size: 1.05rem;
  font-weight: bold;
  font-family: sans-serif;
}
.sidebar_containor 
{
  display: flex;
  justify-content: center;
  flex-direction: column;
  


}
.sidebar_containor a
{
  padding-left:30px;
  padding-bottom: 10px;
  color: rgba(0, 0, 0, 0.63);
  font-size: 17px;
  text-decoration: rgba(0, 0, 0, 0.658);

}
.sidebar_containor a:hover
{
  color: #35bb80;
}
.active

{
  color: green;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 128, 0, 0.466);
  display: flex;
  
  align-items: center;
}

</style>
