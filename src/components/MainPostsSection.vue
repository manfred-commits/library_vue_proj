<template>
  <div class="card_container">
        <div class="row row-cols-1 row-cols-md-2 g-4">
            <div class="col">
            <!-- <div class="col" v-for="" v-bind=""> -->
                <div class="card ">
                    <img src="https://wallpaperaccess.com/full/5487841.jpg" class="card-img-top" alt="">
                    <div class="card-body">
                        <h5 class="card-title">Card title</h5>
                        <p class="card-text ">This is a longer card with supporting text below as a natural lead-in
                            to additional content. This content is a little bit longer.</p>
                    </div>
                </div>
            </div>
            <div class="col">
                <div class="card">
                    <img src="https://wallpaperaccess.com/full/5487841.jpg" class="card-img-top" alt="">
                    <div class="card-body">
                        <h5 class="card-title">Card title</h5>
                        <p class="card-text">This is a longer card with supporting text below as a natural lead-in
                            to additional content. This content is a little bit longer.</p>
                    </div>
                </div>
            </div>
            <div class="col">
                <div class="card">
                    <img src="https://wallpaperaccess.com/full/5487841.jpg" class="card-img-top" alt="">
                    <div class="card-body">
                        <h5 class="card-title">Card title</h5>
                        <p class="card-text">This is a longer card with supporting text below as a natural lead-in
                            to additional content.</p>
                    </div>
                </div>
            </div>
            <div class="col">
                <div class="card">
                    <img src="https://wallpaperaccess.com/full/5487841.jpg" class="card-img-top" alt="">
                    <div class="card-body">
                        <h5 class="card-title">Card title</h5>
                        <p class="card-text">This is a longer card with supporting text below as a natural lead-in
                            to additional content. This content is a little bit longer.</p>
                    </div>
                </div>
            </div>
        </div>

    </div>
</template>

<script>
export default {
  name: 'MainPostsSection',
  props: {
    msg: String
  }
}
</script>

<style lang="scss" scoped>

</style>