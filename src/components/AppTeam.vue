<template>
    <section class="teamWrap">
        <div class="wrapper txt-white py-5">
            <div class="row">
                <div class="col-6">
                    <img class="leftColIllustration" :src="getImagePath(illustrationName)" alt="team section illustration">
                </div>

                <div class="col-6">
                    <p class="text-uppercase">
                        Who we are
                    </p>

                    <h2 class="text-uppercase">
                        We are professional team esport
                    </h2>

                    <p>
                        Distinctively provide acces mutfuncto users whereas transparent proceses somes ncentivize eficient functionalities rather than an extensible archtectur services and cross
                    </p>

                    <ul>
                        <li>
                            <div class="row">
                                <div class="col-2">
                                    <div class="imageWrap d-flex justify-content-center align-items-center">
                                        <img class="iconImg" :src="getImagePath(joystickIconName)" alt="joystick icon">
                                    </div>
                                </div>

                                <div class="col-10">
                                    <h5>
                                        103k Community Earning
                                    </h5>

                                    <p>
                                        Distinctively provide acces mutfuncto users whereas communicate leveraged services
                                    </p>
                                </div>
                            </div>
                        </li>

                        <li>
                            <div class="row">
                                <div class="col-2">
                                    <div class="imageWrap d-flex justify-content-center align-items-center">
                                        <img class="iconImg" :src="getImagePath(headsetIconName)" alt="joystick icon">
                                    </div>
                                </div>

                                <div class="col-10">
                                    <h5>
                                        34m+ Registered Players
                                    </h5>

                                    <p>
                                        Distinctively provide acces mutfuncto users whereas communicate leveraged services
                                    </p>
                                </div>
                            </div>
                        </li>

                        <li>
                            <div class="row">
                                <div class="col-2">
                                    <div class="imageWrap d-flex justify-content-center align-items-center">
                                        <img class="iconImg" :src="getImagePath(gamepadIconName)" alt="joystick icon">
                                    </div>
                                </div>

                                <div class="col-10">
                                    <h5>
                                        240k Streams Complete
                                    </h5>

                                    <p>
                                        Distinctively provide acces mutfuncto users whereas communicate leveraged services
                                    </p>
                                </div>
                            </div>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "AppTeam",

    data(){
        return{
            illustrationName: "01.png",
            joystickIconName: "icon-1.png",
            headsetIconName: "icon-2.png",
            gamepadIconName: "icon-3.png",
        }
    },

    methods: {
        getImagePath: function(img){
            return new URL(`../assets/img/${img}`, import.meta.url).href;
        }
    },
}
</script>

<style lang="scss" scoped>
    @use "../styles/partials/variables.scss" as *;

    section.teamWrap{
        background-color: $mainColor;
    }

    img.leftColIllustration{
        width: 550px;
    }

    p.text-uppercase{
        color: $accentColor;
    }

    div.imageWrap{
            width: 70px;
            height: 70px;
            border-radius: 50%;
            background-color: $accentColor;
        }
</style>