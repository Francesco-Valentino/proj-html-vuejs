<template>
    <section class="sectionWrap">
        <div class="wrapper">
            <p class="littleText text-center text-uppercase">
                Today's
            </p>

            <h2 class="txt-white text-center text-uppercase">
                Our game collection
            </h2>

            <div class="row justify-content-around">
                <div class="col-3 d-flex align-items-center">
                    <img class="teamPngImage" :src="getImagePath(ninjaTeam)" alt="Ninja gaming team logo">
                    <img class="vsPngImage" :src="getImagePath(vsImage)" alt="vs image">
                    <img class="teamPngImage" :src="getImagePath(vikingTeam)" alt="Viking gaming team logo">
                </div>

                <div class="col-3 d-flex align-items-center">
                    <img class="teamPngImage" :src="getImagePath(monkeyTeam)" alt="Ninja gaming team logo">
                    <img class="vsPngImage" :src="getImagePath(vsImage)" alt="vs image">
                    <img class="teamPngImage" :src="getImagePath(frogTeam)" alt="Viking gaming team logo">
                </div>

                <div class="col-3 d-flex align-items-center">
                    <img class="teamPngImage" :src="getImagePath(wolvesTeam)" alt="Ninja gaming team logo">
                    <img class="vsPngImage" :src="getImagePath(vsImage)" alt="vs image">
                    <img class="teamPngImage" :src="getImagePath(dragonsTeam)" alt="Viking gaming team logo">
                </div>
            </div>

            <div class="d-flex justify-content-center my-5">
                <button class="mainScheme">
                    Browse all games
                </button>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "GameCollection",

    methods: {
        getImagePath: function(img){
            return new URL(`../assets/img/${img}`, import.meta.url).href;
        }
    },

    data(){
        return{
            vsImage: "vs.png",
            ninjaTeam: "team-1.png",
            vikingTeam: "team-2.png",
            monkeyTeam: "teamsm-4.png",
            frogTeam: "teamsm-3.png",
            wolvesTeam: "teamsm-2.png",
            dragonsTeam:"teamsm-1.png",
        }
    },
}
</script>

<style lang="scss" scoped>
@use "../styles/partials/variables.scss" as *;

section.sectionWrap{
    background-color: $mainColor;
    padding-top: 6rem;
}

p.littleText{
    color: $accentColor;
}

.vsPngImage{
    width: 45px;
    height: 45px;
}

.teamPngImage{
    width: 100px;
}

.col-3{
    background-color: $boxColor;
    padding: 3rem;
    border-radius: 2px;
}
</style>