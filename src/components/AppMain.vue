<script>

export default {
    name: 'Main',
    data() {
        return {

            services: [
                {
                    img: 'src/assets/img/d-1.png',
                    name: 'Pet Sitting',
                    text: 'The readable content of a page when looking as its layout',

                },
                {
                    img: 'src/assets/img/d-3.png',
                    name: 'Puppy Sitting',
                    text: 'The readable content of a page when looking as its layout',

                },
                {
                    img: 'src/assets/img/d-3.png',
                    name: 'Dog Walking',
                    text: 'The readable content of a page when looking as its layout',

                },
                {
                    img: 'src/assets/img/d-4.png',
                    name: 'Night Care',
                    text: 'The readable content of a page when looking as its layout',

                },
                {
                    img: 'src/assets/img/d-5.png',
                    name: 'Pet Sitting',
                    text: 'The readable content of a page when looking as its layout',

                }
            ]

        }
    }
}

</script>

<template>

    <div class="welcome">

        <div class="container">
            <div class="cta_box">

                <h3>Welcome to DogMilo Pets</h3>

                <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Aliquid, obcaecati! Aliquid quisquam magni
                    ullam ipsam.
                </p>

                <a href="#">Get started!</a>
            </div>

        </div>

    </div>


    <div class="about">

        <div class="container">
            <div>
                <img src="../assets/img/about.png" alt="">
            </div>


            <div>
                <h6>About us</h6>

                <h3>Welcome DogMilo Pets</h3>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Expedita nostrum nam magnam sed odio
                    dolorem! Ipsum vel amet delectus laborum et tempora blanditiis, a quos debitis laudantium eveniet,
                    alias id!</p>
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Dolorem blanditiis numquam doloremque,
                    reprehenderit odio totam minima quas distinctio dolores asperiores similique! Facere similique cum,
                    aut nobis tenetur neque distinctio fugit.</p>

            </div>

        </div>

    </div>

    <div class="services">
        <h6>Services</h6>

        <h3>
            DogMilo Pet Care Services For Your Best Friends.
        </h3>

        <div class="container">
            <div class="card" v-for="service in services">
                <img :src="service.img" alt="">
                <h5>{{ service.name }}</h5>
                <p>{{ service.text }}</p>
                <button><i class="fa-solid fa-chevron-right"></i></button>
            </div>

        </div>

    </div>

    <div class="choose">
        <div>
            <img src="/src/assets/img/why.png" alt="">
        </div>
        <div>
            
        </div>
    </div>
</template>

<style></style>