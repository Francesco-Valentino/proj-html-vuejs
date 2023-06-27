<template>
    <div class="heroWrap position-relative">
        
        <img :src="getImagePath(jumboName)" alt="Brand jumbotron">

        <div class="wrapper position-absolute top-0 start-0 txt-white ms-5 ps-4 textWrap">
           <div class="row">
                <div class="col-6 ms-5">
                    <h1 class="text-uppercase">
                    Online game
                    </h1>

                    <h2 class="text-uppercase">
                        Genuine money transaction
                    </h2>

                    <p>
                        Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusantium accusamus eveniet enim. Ipsam.
                    </p>

                    <button class="mainScheme">
                        Join us today <i class="fa-solid fa-circle-play"></i>
                    </button>
                </div>
           </div>

        </div>
    </div>
</template>

<script>
export default{
    name: "AppHero",

    methods: {
        getImagePath: function(img){
            return new URL(`../assets/img/${img}`, import.meta.url).href;
        }
    },

    data(){
        return{
            jumboName: "bg.jpg"
        }
    },
}
    

</script>

<style lang="scss" scoped>
@use "../styles/partials/variables.scss" as *;
    div.heroWrap{
        /* height: 1200px; */

        img{
            width: 100%;
            object-fit: cover;
        }

        .textWrap{
            margin-top: 10rem;

            h1{
                font-size: 5.2rem;
                text-shadow: 2px 2px 2px $accentColor;
            }
        }
    }
</style>