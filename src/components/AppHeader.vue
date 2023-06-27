<template>

    <header>
        <div>
            <div class="d-flex">
                <p>
                    <i class="fa-solid fa-phone"></i> +800-123-4567 6587
                </p>

                <p>
                    <i class="fa-solid fa-location-dot"></i>  Beverley, New York 224 USA 
                </p>
            </div>

            <div>

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
</style>