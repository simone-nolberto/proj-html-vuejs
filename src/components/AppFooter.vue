<script>

export default {
    name: 'Footer',
    data() {
        return {
            supports: ['Contact Us', 'Online Chat', 'Whatsapp', 'Telegram', 'Snapchat'],
            abouts: ['About Us', 'Blog', 'Career', 'Job', 'In press'],
            faqs: ['Account', 'Order', 'Delivery', 'Payment', 'Return'],
            socialsIcon: ["fa-brands fa-square-facebook", "fa-brands fa-square-pinterest", "<fa-brands fa-square-x-twitter", "fa-brands fa-linkedin", "<fa-brands fa-square-instagram"],


        }
    }
}

</script>

<template>



    <div class="top_footer">
        <div class="newsletter">

            <img src="/src/assets/img/news.png" alt="">

            <div class="news-cta">
                <h3>Subscribe to Our newsletter</h3>
                <input type="email" name="" id="" placeholder="Your Email Here">
            </div>

        </div>

        <div class="container">

            <div class="row">
                <div class="col">
                    <div class="box">
                        <h4>Get in touch</h4>
                        <p>Have a question for us?</p>
                        <p>we'll answer your problem here</p>

                        <ul class="socials">
                            <li v-for="icon in socialsIcon"><i :class="icon"></i></li>
                        </ul>
                    </div>
                </div>
                <div class="col">
                    <h4>Support</h4>

                    <ul>
                        <li v-for="link in supports">{{ link }}</li>
                    </ul>
                </div>
                <div class="col">

                    <h4>About</h4>
                    <ul>
                        <li v-for="link in abouts">{{ link }}</li>
                    </ul>
                </div>
                <div class="col">
                    <h4>Faq</h4>
                    <ul>
                        <li v-for="question in faqs">{{ question }}</li>
                    </ul>
                </div>
                <div class="col">
                    <h4>Contact me</h4>
                    <ul>
                        <li><i class="fa-solid fa-location-arrow"><a href="#">4500 Mercantile plaza, suite 300, fort
                                    worth,
                                    TX, 76137, USA</a></i></li>
                        <li><i class="fa-solid fa-phone"></i><a href="tel:+">1(817)9013377</a></li>
                        <li><i class="fa-solid fa-envelope"></i><a href="mailto:#">info@DogCare.com</a></li>
                    </ul>
                </div>
            </div>

        </div>

    </div>

    <div class="copy">
        Cpyright 2024 by Simone.Nolberto | Boolean Tech Academy | classe 119
    </div>


</template>

<style></style>