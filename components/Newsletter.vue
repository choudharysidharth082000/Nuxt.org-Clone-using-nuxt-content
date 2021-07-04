<template>
<div class="containor_newsletter">
    <div class="newslettercontent">
               <h1>NUXT<span>JS</span> Newsletter</h1>
               <blockquote>Get the latest Nuxt news to your inbox, curated by the NuxtJS team.</blockquote>

               <form id="form" action="submit">
                   <input type="text" placeholder="Email" >
                   <button id="button">SUBSCRIBE</button>
               </form>
               
    </div>
</div>
    
</template>
<script>
export default {
    name: 'Newsletter',

    
}
</script>
<style scoped>
*
{
    margin: 0;
    padding:0 ;
    box-sizing: border-box ;
    font-family: Verdana, Geneva, Tahoma, sans-serif;
}
.containor_newsletter 
{
    padding: 30px;
    
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    background-color: #f8fafc;
}
.newslettercontent h1

{
    color: #2f495e;
}
.newslettercontent span
{
    color: #00c58e;
}
.newslettercontent blockquote
{
    margin-top: 30px;
    color: #917a7b;
}
input
{
    background-color: #d8d8e41f;
    border:1px solid #917a7b8e ;
    height: 50px;
    width: auto;
    
    outline: none;
    

}
input[type = "text"]
{
    background-color: white;
    
    padding-left: 10px;
    font-size: 1rem;
}
::placeholder {
  color: rgba(2, 23, 24, 0.295);
  padding: 20px;
  font-size: 1.1rem;
  
  
}
#button
{
    height: 50px;
    width: auto;
    padding: 10px 20px 10px 20px;
    background-color: #00c58e ;
    color: white;
    border: none ;
    margin-left: 30px;
    
}
#form
{
    margin-top: 40px;

}

</style>