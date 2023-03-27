<script>
export default {
    name: 'TheFooter',
    data() {
        return {
            menuLinks: [
                {
                    text: 'Characters'

                },
                {
                    text: 'Comics'

                },
                {
                    text: 'Movies'

                },
                {
                    text: 'Tv'

                },
                {
                    text: 'Games'

                },
                {
                    text: 'Còllectibles'

                },
                {
                    text: 'Video'

                },
                {
                    text: 'Fans'

                },

            ],

            shopComics: [
                {
                    text: 'Shop DC'

                },

                {
                    text: 'Shop DC Collectibles'

                },

            ],

            shopBars: [
                {
                    text: 'Term of use'
                },
                {
                    text: 'Privacy policy(New)'
                },
                {
                    text: 'Ad Choices'
                },
                {
                    text: 'Advertising'
                },
                {
                    text: 'jobs'
                },
                {
                    text: 'Substractions'
                },
                {
                    text: 'Talent Workshops'
                },
                {
                    text: 'CPSC Certificates'
                },
                {
                    text: 'Ratings'
                },
                {
                    text: 'Sjop Help'
                },
                {
                    text: 'Conctact Us'
                },
            ],

            sitesLink: [
                {
                    text: 'DC'
                },
                {
                    text: 'MAD Magazine'
                },
                {
                    text: 'DC Kids'
                },
                {
                    text: 'DC Universe'
                },
                {
                    text: 'DC Power Visa'
                },


            ],
            imageName: [
                {
                    img: 'footer-facebook.png'

                },
                {
                    img: 'footer-twitter.png'

                },

                {
                    img: 'footer-youtube.png'

                },
                {
                    img: 'footer-pinterest.png'

                },
                {
                    img: 'footer-periscope.png'

                },


            ],


        }

    },
    methods: {
        getImagePath: function (img) {
            console.log(img)
            return new URL(`../assets/${img}`, import.meta.url).href;

        }
    }
};
</script>



<template>
    <div class="container-footer">
        <div class="container-text">
            <div class="mini-text">
                <h3 class="text">DC COMICS</h3>
                <p v-for="(link, index) in menuLinks" key="index">{{ link.text }}</p>

                <h2 class="text">Shop</h2>
                <p v-for="(link, index) in shopComics " key="index">{{ link.text }}</p>

            </div>


            <div class="mini-text container2">
                <h2 class="text">DC</h2>
                <p v-for="(link, index) in shopBars" key="index">{{ link.text }}</p>

            </div>


            <div class="mini-text container3">
                <h2 class="text">SITES</h2>
                <p v-for="(link, index) in sitesLink " key="index">{{ link.text }}</p>

            </div>

            <div class="bg-logo">
                <img src="../assets/dc-logo-bg.png" alt="DC LOGO">
            </div>
        </div>
    </div>
    <div class="container-bottom">
        <div class="text-footer">
            <button>SIGN-UP NOW!</button>


            <div class="follow">
                <h1>Follow Us</h1>
                <img v-for="(img, index) in imageName " key="index" :src="getImagePath(img.img)" alt="Logo Facebook">



            </div>

        </div>


    </div>
</template>



<style scoped></style>