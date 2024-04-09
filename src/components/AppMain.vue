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
            ],

            reasons: [
                {
                    img: 'src/assets/img/w-3.png',
                    name: 'Safety First',
                    text: 'It s a long established fact that a reader will be distructued by the readable content of a page when looking at its layout',

                },
                {
                    img: 'src/assets/img/w-2.png',
                    name: 'Play yards',
                    text: 'It s a long established fact that a reader will be distructued by the readable content of a page when looking at its layout',

                },
                {
                    img: 'src/assets/img/w-1.png',
                    name: 'Monitor your pets',
                    text: 'It s a long established fact that a reader will be distructued by the readable content of a page when looking at its layout',

                },
            ]

        }
    }
}

</script>

<template>

    <div class="welcome">

        <img src="/src/assets/img/b.png" alt="">

        <div class="container">
            <div class="cta_box">

                <h2>Welcome to DogMilo Pets</h2>

                <p>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Aliquid, obcaecati! Aliquid quisquam magni
                    ullam ipsam.
                </p>

                <a href="#">Get started!</a> <a class="play" href="#"><i class="fa-regular fa-circle-play"></i></a>
            </div>

        </div>

    </div>

    <div class="about">

        <div class="container">

            <div>
                <img src="../assets/img/about.png" alt="">
            </div>


            <div class="about-text">
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

        <img class="side-img" src="/src/assets/img/dog-logo.png" alt="">

    </div>

    <div class="services">


        <img class="leftside-img" src="/src/assets/img/dog-left.png" alt="">



        <div class="container">
            <h6>Services</h6>

            <h3>
                DogMilo Pet Care Services For Your Best Friends.
            </h3>

            <div class="service-box">
                <div class="card" v-for="service in services">
                    <img :src="service.img" alt="">
                    <h5>{{ service.name }}</h5>
                    <p>{{ service.text }}</p>
                    <button><i class="fa-solid fa-chevron-right"></i></button>
                </div>
            </div>


        </div>

        <img class="side-img" src="/src/assets/img/dog-logo.png" alt="">

    </div>

    <div class="choose">
        <div>
            <img src="/src/assets/img/why.png" alt="">
        </div>
        <div class="reasons-box">
            <h6>Choose Us</h6>
            <h3>Why Choose Us?</h3>

            <div class="card" v-for="reason in reasons">
                <img :src="reason.img" alt="">
                <div class="card_body">
                    <h5>{{ reason.name }}</h5>
                    <p>{{ reason.text }}</p>
                </div>

            </div>



        </div>
    </div>

    <div class="reviews">

        <div class="container">

            <div class="card">
                <h6>Review & Rating</h6>
                <h3>Over 8000 Customers With 5-Star Review</h3>
                <p>It s a long established fact that a reader will be distructued by the readable content of a page when
                    looking at its layout</p>
                <ul class="vote">
                    <li v-for="star in 5"><i class="fa-solid fa-star"></i></li>
                </ul>
            </div>

            <div class="rev-card">
                <ul class="vote">
                    <li v-for="star in 5"><i class="fa-solid fa-star"></i></li>
                </ul>
                <h4>Great Place</h4>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Laborum pariatur vel voluptate, ad error impedit autem possimus tempore quam laboriosam quia veritatis odio libero. Minus veniam dignissimos dolores debitis quas.</p>

                <div class="user">
                    <img src="/src/assets/img/t1.png" alt="">

                    <div class="user-id">
                        <h4>Tobias May</h4>
                        <p>UI/UX Designer</p>
                    </div>
                </div>
            </div>
            <div class="rev-card">
                <ul class="vote">
                    <li v-for="star in 5"><i class="fa-solid fa-star"></i></li>
                </ul>
                <h4>Great Place</h4>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Laborum pariatur vel voluptate, ad error impedit autem possimus tempore quam laboriosam quia veritatis odio libero. Minus veniam dignissimos dolores debitis quas.</p>

                <div class="user">
                    <img src="/src/assets/img/t1.png" alt="">

                    <div class="user-id">
                        <h4>Tobias May</h4>
                        <p>UI/UX Designer</p>
                    </div>
                </div>
            </div>

        </div>

        <div class="container">
            <div class="carousel-button">
                <button><i class="fa-solid fa-chevron-left"></i></button>
                <button><i class="fa-solid fa-chevron-right"></i></button>

            </div>
        </div>

    </div>
</template>

<style></style>