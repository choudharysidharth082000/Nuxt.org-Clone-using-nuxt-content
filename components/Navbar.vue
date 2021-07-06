<template>
<div class="containor_nav">

    <div class="containor_nav_items">

        <div id="containor_nav_logo" class="containor_nav_logo">
            <img src="https://tse3.mm.bing.net/th?id=OIP.O6ItV8jHybw34TIjE2T6qQHaD4&pid=Api&P=0&w=316&h=167" alt="logo">
        </div>
        <div class="links">
            <ul>
                <li>
                    <a href="https://nuxtjs.org/docs/2.x/get-started/installation">DOCS</a>
                    <a href="https://nuxtjs.org/examples">EXAMPLE</a>
                    <a href="https://nuxtjs.org/resources">RESOURCES</a>
                    <a href="https://nuxtjs.org/blog">BLOG</a>
                    <a href="https://masteringnuxt.com/?utm_source=nuxt&utm_medium=link&utm_campaign=navbar_link">VIDEO COURSES</a>
                    
                </li>
            </ul>
        </div>

        <div class="containor_nav_searchbar">

            <form action="submit">
                <input id="input" type="text" placeholder="Search ('/' to focus)">
            </form>
        </div>

        <div @click="clicked" class="hamburger">
            <svg @click="clicked" xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
</svg>
        </div>

    </div>

    <div id="sidebarmenu" class="sidebarmenu">
        <div class="crossbutton">
            <a @click="closeside" id="close" class="crossbutton" href="#">Close</a>
        </div>


        <div class="contents">

            <div id="sidebarcontent" class="sidebarcontent">

                <h3>ROUTING</h3>
                
                <a href="#">Hello World</a><br>
                <a href="/Activelink">Nuxt helpers</a><br>
                <a href="#">Dynamic Pages</a><br>
                <a href="#">Nested Pages</a><br><br>
               
                <h3>Data Fetching</h3>
                
                <a href="#">asyncData Hook</a><br>
                <a href="#">fetch Hook</a><br><br>
                
                <h3>Asset Management</h3>
                
                <a href="#">webpack Assets</a><br>
                <a href="#">Pre-processors</a><br><br>
               
                <h3>Transitions</h3>
                
                <a href="#">Nuxt transitions</a><br><br>
                
                <h3>SEO</h3>
                
                <a href="#">SEO HTML Head</a><br>
                <a href="#">SEO Twitter and Open Graph</a><br><br>
                
                <h3>Miscelenous</h3>
                
                <a href="#">Layouts</a><br>
                <a href="#">Lazy Loading Components</a><br>
                <a href="#">Vuex store</a><br>
                <a href="#">Nuxt Helpers</a><br><br>
               
                <h3>MiddleWare</h3>
                
                <a href="#">Router Middleware</a><br>
                <a href="#">Named Middleware</a><br>
                <a href="#">Anonymous Middleware</a><br><br>

                <h3>plugins</h3>
                
                <a href="#">Vue Plugins</a><br>
                <a href="#">Client only Plugins</a><br>
                <a href="#">External Packages Plugin</a><br>
                <a href="#">Custom Plugins</a><br>
               
                <h3>Modules</h3>
                
                <a href="#">Local Module</a><br>
                <a href="#">Axios Module</a><br><br>



            </div>


            
            

        </div>
    

    </div>


</div>
    
</template>
<script>
export default {
    name: 'Navbar',
    methods:
    {
        clicked(){
            var sidebar = document.getElementById('sidebarmenu');
            var sidebarcontent = document.getElementById('sidebarcontent');
            var anchor = document.getElementById('close');
            sidebar.style.width= '100%';
            sidebar.style.height= '100vh';
            sidebar.style.height= '100vh';
            anchor.style.display ='flex';
            sidebarcontent.style.display='block';
            
            

        
        },
        closeside()
        {
            var sidebar = document.getElementById('sidebarmenu');
            var sidebarcontent = document.getElementById('sidebarcontent');
            var anchor = document.getElementById('close');
            console.log('button clicked');
            sidebar.style.width = '0';
            sidebar.style.height = '0';
            anchor.style.display = 'none';
            sidebarcontent.style.display = 'none';


        }
    }
    
}
</script>
<style scoped>
*
{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Verdana, Geneva, Tahoma, sans-serif;
    transition: 0.4s ease;
}.crossbutton
{
    width: 100%;
    height: 70px;
    background-color: #f8fafc;
    display: flex;
    justify-content: flex-end;
    align-items: center;
    padding-right: 20px;

}a

{
    padding-left: 40px;
    
    font-size: 1.1rem;
    
}
.sidebarcontent 
{
    display: none;
    height: 100%;
    
    flex-direction: column;
    overflow-y: scroll;
    
    
}
.sidebarcontent h3
{
    color: #a4b2c3;
    font-size: 1.3rem;
    padding: 20px;
    text-transform: uppercase;

}
.sidebarcontent a
{
    color: #4e6476da ;
    text-decoration: #4e6476;

}
.sidebarcontent a:hover

{
    color:#4db687 ;
}

.crossbutton a
{
    color: #4db687;
    text-decoration: #4db687;  
    display: none;


}
    
    

.containor_nav
{
    width: 100%;
    height: auto;
    
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
   

}
.contents
{
    width: 100%;
    height: 500px;
    background-color: #f8fafc;
}
.sidebarmenu
{
    height: 100vh;
    width: 100%;
    
    background-color: #f8fafc;
    margin-right:-70px;
    width: 0;
    height: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    
    
    

    
}

.activeborder
{
     border-bottom: 1px solid rgba(0, 0, 0, 0.24);
}
.containor_nav_items 
{
    width: 80%;
    height: 150px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    
}
.containor_nav_logo
{
    
    height: 80%;
    width: 250px;
    object-fit: contain;
    
    
}
.hamburger
{
    height: 60px;
    width: 60px;
    
    display: flex;
    justify-content: center;
    align-items: center;
    display: none;
}
.containor_nav_logo img
{
    height: 100%;
    width: 250px;
    object-fit: contain;
}
.links 
{
    height: 80%;
    width: 600px;

    display: flex;
    justify-content: center;
    align-items: center;
}
.links ul

{
    list-style: none;

}
.links ul li a 
{
    text-decoration: white;
    color: rgba(0, 0, 0, 0.747);
    font-size: 1.1rem;
    padding: 10px;


}
.links ul li a:hover
{
    color: #35bb80;
}
.containor_nav_searchbar 
{
    height: 80%;
    width: 300px;
    display: flex;
    justify-content: center;
    align-items: center;
}
#input
{
    background-color: #d8d8e41f;
    border: none ;
    height: 40px;
    width: auto;
    border-radius: 20px;
    outline: none;
    

}
input[type = "text"]
{
    padding-left: 20px;
    font-size: 1.1rem;
}
::placeholder {
  color: rgba(2, 23, 24, 0.295);
  padding: 20px;
  font-size: 1.1rem;
  
  
}
@media screen and (max-width: 1400px){

  .links ul li a 
  {
display: none ;
  }
  .hamburger
  {
      display: block;
      margin-top: 50px;
      margin-left: -10px;
      cursor: pointer;
      margin-left: 3px;
  }
  .containor_nav_searchbar
  {
      margin-left: -60px;
  }
  


  
}
</style>