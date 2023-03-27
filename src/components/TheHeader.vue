<script>
export default {
    name: 'TheHeader',
    data() {
        return {
            navBar: [
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
                {
                    text: 'News'

                },
                {
                    text: 'Shop'

                },


            ]

        }
    }
};
</script>



<template>
    <div class="navbar">
        <div class="nav-logo">
            <img src="../assets/dc-logo.png" alt=" Dc logo">
        </div>
        <div class="link-nav">
            <ul class="list">
                <li v-for="(link, index) in navBar" class="item" key="index">{{ link.text }}</li>

            </ul>
        </div>
    </div>
</template>




<style scoped></style>