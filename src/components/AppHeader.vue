<template>

    <header>
        <div class="container pt-3">
            <div class="row d-flex justify-content-between">
                <div class="d-flex col-6 justify-content-between">
                    <p>
                        <i class="fa-solid fa-phone"></i> +800-123-4567 6587
                    </p>

                    <p>
                        <i class="fa-solid fa-location-dot"></i>  Beverley, New York 224 USA 
                    </p>
                </div>

                <div class="d-flex col-2 justify-content-between">
                    <i class="fa-brands fa-facebook-messenger"></i>

                    <i class="fa-brands fa-twitter"></i>

                    <i class="fa-brands fa-vimeo-v"></i>

                    <i class="fa-brands fa-skype"></i>

                    <i class="fa-solid fa-rss"></i>
                </div>
            </div>
            
        </div>

        <div class="container">
            <div class="row d-flex">
                <div class="col-3">
                    <img :src="getImagePath(logoName)" alt="Gamer logo">
                </div>
                
                <nav class="d-flex justify-content-end text-uppercase col-9">
                    <ul class="d-flex justify-content-around">
                        <li v-for="action in headerNavActions">
                            {{ action }}
                        </li>
                    </ul>

                    <div>
                        <button class="text-uppercase logIn">
                            <i class="fa-solid fa-user"></i> Log in
                        </button>

                        <button class="text-uppercase signUp">
                            <i class="fa-solid fa-users"></i> Sign Up
                        </button>
                    </div>
                </nav>
            </div>
        </div>
    </header>
    

    <nav>

    </nav>
</template>

<script>
export default {
    name: "AppHeader",

   data(){
        return{
            headerNavActions: [
                "Home",
                "Features +",
                "Achievement",
                "Blog +",
                "Contact",
            ],

            logoName: "logo.png",
        }
   },

   methods: {
    getImagePath: function(img) {
        return new URL(`../assets/img/${img}`, import.meta.url).href;
    }
   }
}
</script>

<style lang="scss" scoped>
    @use "../styles/partials/variables.scss" as *;

    header{
        background-color: $mainColor;
        color: white;

        button.logIn{
            background-color: white;
            color: $accentColor;
            border-bottom: $accentColor 2px solid;
            padding: .5rem;
        }
    }
</style>