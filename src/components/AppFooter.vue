<template>
    <section>
        <div class="upperFooter">
            <div class="wrapper">
                <div class="row pt-5">
                    <div class="col-4 d-flex justify-content-center">
                        <img class="me-3" :src="getImagePath(contactImage)" alt="contact illustration">

                        <p class="txt-white mt-1">
                            Phone Number : +88012 345 678 912 
                        </p>
                    </div>

                    <div class="col-4 d-flex justify-content-center">
                        <img class="me-3" :src="getImagePath(contactImage)" alt="contact illustration">

                        <p class="txt-white mt-1">
                            Email : youremail@gmail.com                        </p>
                    </div>

                    <div class="col-4 d-flex justify-content-center">
                        <img class="me-3" :src="getImagePath(contactImage)" alt="contact illustration">

                        <p class="txt-white mt-1">
                            Address : 30 North West New York 240                         </p>
                    </div>
                </div>
            </div>
        </div>

        <div class="lowerFooter">
            <p class="py-5 txt-white text-center">
                ©2022 Gamer - eSpost And Gameing HTML Template.
            </p>
        </div>
    </section>
</template>

<script>
export default {
    name: "AppFooter",

    methods: {
        getImagePath: function(img){
            return new URL(`../assets/img/${img}`, import.meta.url).href;
        }
    },

    data(){
        return{
            contactImage: "01 (4).png"
        }
    },
}
</script>

<style lang="scss" scoped>
    @use "../styles/partials/variables.scss" as *;

    div.upperFooter{
        background-image: url("../assets/img/bg\ \(3\).jpg");
    }

    div.lowerFooter{
        background-color: $boxColor;
    }
</style>