<template>
<div class="containor_nav `${(window.scrolly > 300) ? 'activeborder' : ''}`">

    <div class="containor_nav_items">

        <div class="containor_nav_logo">
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

    </div>


</div>
    
</template>
<script>
export default {
    name: 'Navbar'
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
}
.containor_nav
{
    width: 100%;
    height: 130px;
    
    display: flex;
    justify-content: center;
    align-items: center;
   

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
</style>