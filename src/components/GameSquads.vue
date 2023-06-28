<template>
    <section class="squadsSectionWrapper pt-5">
        <p class="smallText text-uppercase text-center">
            Meet our players
        </p>

        <h1 class="txt-white text-uppercase text-center">
            Meet our squad players
        </h1>

        <div class="wrapper py-5">
            <div class="row">
                <div class="col-3 vikings d-flex flex-column align-items-center">
                    <img :src="getImagePath(vikingsName)" alt="team logo">
                </div>

                <div class="col-3 dragons d-flex flex-column align-items-center">
                    <img :src="getImagePath(dragonsName)" alt="team logo">
                </div>

                <div class="col-3 frogs d-flex flex-column align-items-center">
                    <img :src="getImagePath(vikingsName)" alt="team logo">
                </div>

                <div class="col-3 tigers d-flex flex-column align-items-center">
                    <img :src="getImagePath(dragonsName)" alt="team logo">
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "GameSquads",

    methods: {
        getImagePath: function(img){
            return new URL(`../assets/img/${img}`, import.meta.url).href;
        }
    },

    data(){
        return{
            vimeoName: 'social-1.png',
            youtubeName: 'social-2.png',
            twitchName: 'social-3.png',
            vikingsName: "5.png",
            dragonsName: "1.png",
            /* frogsName: "teamsm-3.png",
            tigersName: "teamsm-6.png", */
        }
    },
}
</script>

<style lang="scss" scoped>
    @use "../styles/partials/variables.scss" as *;
    
    section.squadsSectionWrapper{
        background-color: $mainColor;
        height: 1000px;
    }

    p.smallText{
        color: $accentColor;
    }

    div.col-3{
        height: 500px;
        border: solid 3px $boxColor;
        padding: 0 .3rem 0 .3rem;

        img{
            width: 220px;
        }
    }

    div.vikings{
        background-image: url("../assets/img/5.jpg");
    }

    div.dragons{
        background-image: url("../assets/img/1.jpg");
    }

    div.frogs{
        background-image: url("../assets/img/1.jpg");
        filter: sepia(100%);
    }

    div.tigers{
        background-image: url("../assets/img/5.jpg");
        filter: brightness(.7);
    }
</style>