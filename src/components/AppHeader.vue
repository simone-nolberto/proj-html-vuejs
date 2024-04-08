<script>

export default {
    name: 'Header',
    data() {
        return {
            socialsIcon: ["fa-brands fa-square-facebook", "fa-brands fa-square-pinterest", "<fa-brands fa-square-x-twitter", "fa-brands fa-linkedin", "<fa-brands fa-square-instagram"],

            sections: [],
        }
    }
}

</script>

<template>

    <div class="top_header">
        <div class="contacts">
            <ul>
                <li><i class="fa-solid fa-envelope"></i><a href="mailto:#">info@DogCare.com</a></li>
                <li><i class="fa-solid fa-phone"></i><a href="tel:+">1(817)9013377</a></li>
            </ul>
        </div>
        <div class="socials">
            <ul>
                <li v-for="icon in socialsIcon"><i :class="icon"></i></li>
            </ul>
        </div>
    </div>

    <div class="nav">
        <div class="logo"></div>
        <div class="menu"></div>
    </div>


</template>

<style></style>