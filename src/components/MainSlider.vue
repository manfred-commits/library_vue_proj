<template>
    <main>
        <div id="carouselExampleCaptions" class="carousel slide" data-bs-ride="false">
            <div class="carousel-indicators">
                <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="0" class="active"
                    aria-current="true" aria-label="Slide 1"></button>
                <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="1"
                    aria-label="Slide 2"></button>
                <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="2"
                    aria-label="Slide 3"></button>
            </div>
            <!-- carousel image slider content-->
            <div class="carousel-inner">
                <div :class="['carousel-item', (index==0?'active':'')]" v-for="(slider_image, index) in slider_images" v-bind:key = "slider_image+index">
                    <img :src="slider_image" class="d-block w-100" alt="">
                    <div class="carousel-caption d-none d-md-block">
                        <h5>{{slider_text_label[index]}}</h5>
                        <p>{{slider_text_description[index]}}</p>
                    </div>
                </div>
            </div>
            <!-- carousel image slider content-->

            <!-- carousel directional buttons -->
            <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleCaptions"
                data-bs-slide="prev">
                <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                <span class="visually-hidden">Previous</span>
            </button>
            <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleCaptions"
                data-bs-slide="next">
                <span class="carousel-control-next-icon" aria-hidden="true"></span>
                <span class="visually-hidden">Next</span>
            </button>
            <!-- carousel directional buttons -->

        </div>
        
    </main>
</template>

<script>

export default {
    name: 'MainSlider',
    components: {
    },
    data() {
        return {
            slider_images: [
                    "https://wallpaperaccess.com/full/5487841.jpg",
                    "https://wallpaperaccess.com/full/5487841.jpg",
                    "https://wallpaperaccess.com/full/5487841.jpg",
                    ],
            slider_text_label: [
                "Slide 1",
                "Slide 2",
                "Slide 3",
            ],
            slider_text_description: [
                "Slide 1 description",
                "Slide 2 description",
                "Slide 3 description",
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
main {
    width: 80%;
    margin: auto;
    padding-top: 5%;
    color: white;

    #carouselExampleCaptions {
        img {
            height: 500px;
            object-fit: cover;
        }
    }

    .card_container {
        width: 100%;
        padding: 1rem 0 1rem;

        img {
            height: 300px;
            object-fit: cover;
        }
    }
    .card{
        background-color: rgb(20, 20, 20) !important;
    }
    .card-body{
        background-color: rgb(20, 20, 20) !important;
        border: 0;
    }

}
</style>