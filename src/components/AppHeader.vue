<script>

export default {
    name: 'Header',
    data() {
        return {
            socialsIcon: ["fa-brands fa-square-facebook", "fa-brands fa-square-pinterest", "<fa-brands fa-square-x-twitter", "fa-brands fa-linkedin", "<fa-brands fa-square-instagram"],

            sections: ['Home', 'About', 'Services', 'Training', 'Blogs'],
        }
    }
}

</script>

<template>

    <div class="top_header">
        <div class="container">

            <ul class="contacts">
                <li><i class="fa-solid fa-envelope"></i><a href="mailto:#">info@DogCare.com</a></li>
                <li><i class="fa-solid fa-phone"></i><a href="tel:+">1(817)9013377</a></li>
            </ul>

            <ul class="socials">
                <li v-for="icon in socialsIcon"><i :class="icon"></i></li>
            </ul>

        </div>

    </div>

    <div class="nav">
        <div class="container">
            <div class="logo">
                <img src="../assets/img/logo.png" alt="">
            </div>
            <div>
                <ul class="menu">
                    <li v-for="section in sections">{{ section }}</li>
                    <a href="#">Contattaci!</a>
                </ul>
            </div>
        </div>

    </div>




</template>

<style></style>