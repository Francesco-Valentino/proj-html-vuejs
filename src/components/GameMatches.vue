<template>
    <section class="matchesWrap">
        <p class="text-uppercase text-center">
            Anywhere, anytime
        </p>
        
        <h1 class="text-uppercase txt-white text-center">
            All matches schedule
        </h1>
        
        <div class="wrapper">
            <div class="row">
                <div class="col-12 mb-5">
                    <div class="upperBox txt-white d-flex justify-content-between align-items-center pt-3 px-3">
                        <p>
                            <span class="text-uppercase">2 group</span> <span class="text-uppercase fw-bold">32 Players</span>
                        </p>

                        <p>
                            <span class="text-uppercase">Prize pool</span> <span class="text-uppercase fw-bold">$3200</span>
                        </p>
                    </div>

                    <div class="lowerBox d-flex justify-content-between align-items-center py-4 px-3">
                        <div>
                            <h5 class="text-uppercase">
                                Battlefield-4 torunament
                            </h5>

                            <p>
                                30 April 2022 Time: 08:30PM 
                            </p>
                        </div>

                        <div>
                            <img :src="getImagePath(lionsName)" alt="team logo">
                            
                            <img class="mx-5" :src="getImagePath(vsImageName)" alt="vs image">
                            
                            <img :src="getImagePath(jesterName)" alt="team logo">
                        </div>

                        <div>
                            <img :src="getImagePath(vimeoName)" alt="vimeo logo">
                            
                            <img :src="getImagePath(youtubeName)" alt="youtube logo">
                            
                            <img :src="getImagePath(twitchName)" alt="twitch logo">

                            <button class="offScheme ms-5">
                                Watch now <i class="fa-solid fa-circle-play"></i>
                            </button>
                        </div>
                    </div>
                </div>
            </div>

            <div class="colWrap d-flex justify-content-between">
                <div class="column">
                    <div class="row">
                        <div class="col-12">
                            <h2 class="txt-white text-center text-uppercase">
                                Upcoming matches
                            </h2>

                            <div class="matchCard">
                                <div class="upperBox txt-white d-flex justify-content-between align-items-center pt-3 px-3">
                                    <p>
                                        <span class="text-uppercase">2 group</span> <span class="text-uppercase fw-bold">32 Players</span>
                                    </p>

                                    <p>
                                        <span class="text-uppercase">Prize pool</span> <span class="text-uppercase fw-bold">$3200</span>
                                    </p>
                                </div>

                                <div class="lowerBox d-flex justify-content-between align-items-center py-4 px-3">
                                    <img :src="getImagePath(dragonsName)" alt="team thumbnail">

                                    <div>
                                        <p class="text-uppercase text-center txt-normal">
                                            Call of duty tournament 30 April 2022 Time: 08:30PM
                                        </p>
                                    
                                        <div>
                                            <img :src="getImagePath(vimeoName)" alt="vimeo logo">
                                            
                                            <img :src="getImagePath(youtubeName)" alt="youtube logo">
                                            
                                            <img :src="getImagePath(twitchName)" alt="twitch logo">
                                        </div>
                                    </div>

                                    <img :src="getImagePath(wolvesName)" alt="team thumbnail">
                                </div>
                            </div>

                            <div class="matchCard">
                                <div class="upperBox txt-white d-flex justify-content-between align-items-center pt-3 px-3">
                                    <p>
                                        <span class="text-uppercase">2 group</span> <span class="text-uppercase fw-bold">32 Players</span>
                                    </p>

                                    <p>
                                        <span class="text-uppercase">Prize pool</span> <span class="text-uppercase fw-bold">$3200</span>
                                    </p>
                                </div>

                                <div class="lowerBox d-flex justify-content-between align-items-center py-4 px-3">
                                    <img :src="getImagePath(frogName)" alt="team thumbnail">

                                    <div>
                                        <p class="text-uppercase text-center txt-normal">
                                            Call of duty tournament 30 April 2022 Time: 08:30PM
                                        </p>
                                    
                                        <div>
                                            <img :src="getImagePath(vimeoName)" alt="vimeo logo">
                                            
                                            <img :src="getImagePath(youtubeName)" alt="youtube logo">
                                            
                                            <img :src="getImagePath(twitchName)" alt="twitch logo">
                                        </div>
                                    </div>

                                    <img :src="getImagePath(monkeyName)" alt="team thumbnail">
                                </div>
                            </div>

                            <div class="matchCard">
                                <div class="upperBox txt-white d-flex justify-content-between align-items-center pt-3 px-3">
                                    <p>
                                        <span class="text-uppercase">2 group</span> <span class="text-uppercase fw-bold">32 Players</span>
                                    </p>

                                    <p>
                                        <span class="text-uppercase">Prize pool</span> <span class="text-uppercase fw-bold">$3200</span>
                                    </p>
                                </div>

                                <div class="lowerBox d-flex justify-content-between align-items-center py-4 px-3">
                                    <img :src="getImagePath(sharkName)" alt="team thumbnail">

                                    <div>
                                        <p class="text-uppercase text-center txt-normal">
                                            Call of duty tournament 30 April 2022 Time: 08:30PM
                                        </p>
                                    
                                        <div>
                                            <img :src="getImagePath(vimeoName)" alt="vimeo logo">
                                            
                                            <img :src="getImagePath(youtubeName)" alt="youtube logo">
                                            
                                            <img :src="getImagePath(twitchName)" alt="twitch logo">
                                        </div>
                                    </div>

                                    <img :src="getImagePath(lionsName)" alt="team thumbnail">
                                </div>
                            </div>
                        </div>
                    </div>
                </div>

                <div class="column">
                    <div class="row">
                        <div class="col-12">
                            <h2 class="txt-white text-center text-uppercase">
                                Previous matches
                            </h2>

                            <div class="matchCard">
                                <div class="upperBox txt-white d-flex justify-content-between align-items-center pt-3 px-3">
                                    <p>
                                        <span class="text-uppercase">2 group</span> <span class="text-uppercase fw-bold">32 Players</span>
                                    </p>

                                    <p>
                                        <span class="text-uppercase">Prize pool</span> <span class="text-uppercase fw-bold">$3200</span>
                                    </p>
                                </div>

                                <div class="lowerBox d-flex justify-content-between align-items-center py-4 px-3">
                                    <img :src="getImagePath(robotName)" alt="team thumbnail">

                                    <div>
                                        <p class="text-uppercase text-center txt-normal">
                                            Call of duty tournament 30 April 2022 Time: 08:30PM
                                        </p>
                                    
                                        <div>
                                            <img :src="getImagePath(vimeoName)" alt="vimeo logo">
                                            
                                            <img :src="getImagePath(youtubeName)" alt="youtube logo">
                                            
                                            <img :src="getImagePath(twitchName)" alt="twitch logo">
                                        </div>
                                    </div>

                                    <img :src="getImagePath(witchName)" alt="team thumbnail">
                                </div>
                            </div>

                            <div class="matchCard">
                                <div class="upperBox txt-white d-flex justify-content-between align-items-center pt-3 px-3">
                                    <p>
                                        <span class="text-uppercase">2 group</span> <span class="text-uppercase fw-bold">32 Players</span>
                                    </p>

                                    <p>
                                        <span class="text-uppercase">Prize pool</span> <span class="text-uppercase fw-bold">$3200</span>
                                    </p>
                                </div>

                                <div class="lowerBox d-flex justify-content-between align-items-center py-4 px-3">
                                    <img :src="getImagePath(jesterName)" alt="team thumbnail">

                                    <div>
                                        <p class="text-uppercase text-center txt-normal">
                                            Call of duty tournament 30 April 2022 Time: 08:30PM
                                        </p>
                                    
                                        <div>
                                            <img :src="getImagePath(vimeoName)" alt="vimeo logo">
                                            
                                            <img :src="getImagePath(youtubeName)" alt="youtube logo">
                                            
                                            <img :src="getImagePath(twitchName)" alt="twitch logo">
                                        </div>
                                    </div>

                                    <img :src="getImagePath(kitsuneName)" alt="team thumbnail">
                                </div>
                            </div>

                            <div class="matchCard">
                                <div class="upperBox txt-white d-flex justify-content-between align-items-center pt-3 px-3">
                                    <p>
                                        <span class="text-uppercase">2 group</span> <span class="text-uppercase fw-bold">32 Players</span>
                                    </p>

                                    <p>
                                        <span class="text-uppercase">Prize pool</span> <span class="text-uppercase fw-bold">$3200</span>
                                    </p>
                                </div>

                                <div class="lowerBox d-flex justify-content-between align-items-center py-4 px-3">
                                    <img :src="getImagePath(dragon2Name)" alt="team thumbnail">

                                    <div>
                                        <p class="text-uppercase text-center txt-normal">
                                            Call of duty tournament 30 April 2022 Time: 08:30PM
                                        </p>
                                    
                                        <div>
                                            <img :src="getImagePath(vimeoName)" alt="vimeo logo">
                                            
                                            <img :src="getImagePath(youtubeName)" alt="youtube logo">
                                            
                                            <img :src="getImagePath(twitchName)" alt="twitch logo">
                                        </div>
                                    </div>

                                    <img :src="getImagePath(monkey2Name)" alt="team thumbnail">
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <div class="d-flex justify-content-center py-5">
                <button class="mainScheme">
                    Browse all matches <i class="fa-solid fa-circle-chevron-right"></i>
                </button>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "GameMatches",

    methods: {
        getImagePath: function(img){
            return new URL(`../assets/img/${img}`, import.meta.url).href;
        }
    },

    data(){
        return{
            vsImageName: "vs.png",
            vimeoName: "social-1.png",
            youtubeName: "social-2.png",
            twitchName: "social-3.png",
            lionsName: "teamsm-6.png",
            jesterName: "teamsm-9.png",
            dragonsName: "teamsm-1.png",
            wolvesName: "teamsm-2.png",
            robotName: "teamsm-7.png",
            witchName: "teamsm-8.png",
            frogName: "teamsm-3.png",
            monkeyName: "teamsm-4.png",
            kitsuneName: "teamsm-10.png",
            sharkName: "teamsm-5.png",
            dragon2Name: "teamsm-11.png",
            monkey2Name: "teamsm-12.png",
        }
    },  
}
</script>

<style lang="scss" scoped>
    @use "../styles/partials/variables.scss" as *;

    section.matchesWrap{
        background-image: url("../assets/img/bg\ \(1\).jpg");
        background-position: center;
/*         height: 1000px;
 */    }

    p.text-uppercase.text-center{
        color: $accentColor;
    }
    p.text-uppercase.text-center.txt-normal{
        color: black;
    }

    div.column{
        width: 550px;
    }

    div.upperBox{
        background-color: $accentColor;
    }

    div.lowerBox{
        background-color: white;
    }

    div.matchCard{
        margin-bottom: 2rem;
    }
</style>