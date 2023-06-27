<template>

    <header>
        <div class="container d-flex justify-content-between pt-3">
            <div class="d-flex col-6 justify-content-between">
                <p>
                    <i class="fa-solid fa-phone"></i> +800-123-4567 6587
                </p>

                <p class="">
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
        }
   },
}
</script>

<style lang="scss" scoped>
    @use "../styles/partials/variables.scss" as *;

    header{
        background-color: $mainColor;
        color: white;
    }
</style>