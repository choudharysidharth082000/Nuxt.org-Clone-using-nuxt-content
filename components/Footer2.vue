<template>
    <div class="containorfooter">
        <div class="firstone">

            <div class="header"><h4>DISCOVER</h4></div>
            <div class="links">
                <a href="#">Our Team</a>
            <a href="#">Design Kit</a>
            <a href="#">Contact Us</a>

            </div>
        </div>
        <div class="secondone">
            <div class="header"><h4>HELP</h4></div>
            <div class="links">
                <a href="#">Resources</a>
            <a href="#">Chat with us</a>
            <a href="#">Contribution guide</a>
            </div>
            

        </div>
        <div class="thirdone">
            <div class="header"><h4>SUPPORT</h4></div>
            <div class="links">
                <a href="#">Our Goodies Store</a>
            <a href="#">Sponsoring & Donations</a>
            <a href="#">Training & Consultancy</a>
            </div>
        </div>

    </div>
</template>
<script>
export default {
    name: 'Footer2'
}
</script>
<style scoped>
*
{
    margin: 0;
    padding: 0;
    box-sizing: border-box ;
    font-family: Verdana, Geneva, Tahoma, sans-serif;
    transition: all 0.4 ease;
}
.containorfooter 
{
    height: 100%;
    width: 100%;

    display: flex;
    flex-direction: row;
}
.firstone
{
    flex: 1;
    background-color: white;
    
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
}
.header
{
    margin: 25px;
    font-family: Arial, Helvetica, sans-serif;
    color: #2f495e;
    font-size: 0.7rem;
}
.header, .links 
{
    margin-top: -20px;

}
.links 
{
    height: 100px;
    width: 200px;
    display: flex;
    flex-direction: column;
    
    justify-content: center;
    align-items: center;
}
.links a
{
    color: #607187;
    text-decoration: #607187;
    font-size: 1rem;
    padding: 3px;
}
.links a:hover 
{
    color:#35bb80 ;
}
.secondone 
{
    flex: 1;
     background-color: white;
    
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    
}
.thirdone 
{
    flex: 1;
     background-color: white;
    
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
}
@media screen and (max-width: 1400px){

  .containorfooter{
    flex-direction:column ;
  }
  
}

</style>