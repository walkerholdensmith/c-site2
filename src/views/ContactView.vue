<template>
    <div class="contact-view">
        <ContactUs/>

        <div class="links">
            <!-- <fab icon="fa-brands fa-facebook" /> -->
            <h5 class="header">Contact Inforamtion</h5>
            <div class="outer-container">
                <div class="icon-vert">
                    <fa icon="phone" class="icon"/> 
                    <fa icon='fa-envelope' class="icon"/> 
                </div>
                <div class="text-vert">
                    <a href="google.com" class="link"> (520)247-4003</a>
                    <a href="facebook.com"  class="link">Tucson Equine Email</a> 
                </div>
            </div>

            <h5 class="header">Find us on Social Media</h5>
            <div class="outer-container">
                <div class="icon-vert">
                    <fa :icon="['fab','facebook']" class="icon"/>
                    <fa :icon="['fab','instagram']" class="icon"/>
                    <fa :icon="['fab','linkedin']" class="icon"/>
                    
                </div>
                <div class="text-vert">
                    <a href="facebook.com" class="link">Tucson Equine Facebook</a> 
                    <a href="facebook.com" class="link">Tucson Equine Instagram</a> 
                    <a href="facebook.com" class="link">Tucson Equine LinkedIn</a> 
                    
                </div>
            </div>
            

                      

            
        </div>
    </div>

</template>

<style scoped>

.contact-view{
    display: flex;
    justify-content: space-evenly;
    align-items: left;
}

.links{
    text-align: left;
    display: flex;
    flex-direction: column;
    margin-top: 5%;
    width: 300px;
    border: 2px solid #219EBC;
    background-color:#219EBC ;
    justify-content: space-evenly;
    padding: 20px;
    border-radius: 10px;



    /* justify-content: space-evenly; */
}    

.link, .phone, .email{
    font-size: 15px;
    color: white;
    text-decoration: none;
    vertical-align: middle;
    font-weight: bold;

    /* padding-bottom: 20px; */

}


.header{
    color: white;
    font-weight: bold;
    font-size: 22px;
    margin-bottom: -10px;
}

.outer-container{
    display: flex;
}


.icon-vert, .text-vert{
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
}

.link-item{
    /* text-align: center; */
}

.icon{
    height: 30px;
    color: white;

}

.icon, .link{
    padding: 10px;
}

@media (max-width: 480px){
    .contact-view{
        display: flex;
        flex-direction: column;
        justify-content: space-evenly;
        align-items: left;
        align-items: center;
    }  
}

</style>

<script>
import ContactUs from "@/components/ContactUs.vue";
export default{
    components: {
        ContactUs
    }
}
</script>