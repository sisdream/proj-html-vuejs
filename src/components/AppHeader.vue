<script>
 export default {
        data () {
            return {
                links: [
                    'HOME',
                    'ABOUT',
                    'SERVICES',
                    'SHOWCASE',
                    'BLOG',
                    'CONTACT'
                ],
                socials:[
                    'FACEBOOK',
                    'INSTAGRAM',
                    'YOUTUBE',
                    'TWITTER'
                ],
                images: [
                    {
                        id: 1,
                        src: "/images/Group-36-2x.png",
                    },
                    {
                        id: 2,
                        src: "/images/Group-35-2x.png",
                    },
                    {
                        id: 3,
                        src: "/images/Group-40-2x.png",
                    },
                ],
                image: {
                    id: 1,
                    src: "/images/Group-36-2x.png",
                }
            }
        },
        methods: {
            switchImage(id){
                this.images.forEach(image => {
                    if (id === image.id) {
                        this.image = image;
                    }
                });       
            }
        }
    }
</script>

<template>
 <header id="top">
    <section class="header-fixed"> 
        <div class="banda-recapiti">
            <div>
                <span>(001) 88451234</span>
                <span class="ms-3">88455438</span>
            </div>
            <div class="d-flex gap-3">
                <i class="fa-brands fa-facebook-f"></i>
                <i class="fa-brands fa-twitter"></i>
                <i class="fa-brands fa-pinterest-p"></i>
            </div>
        </div>
        <div class="banda-dinamica">
            <div class="logo">
                <img src="/images/cropped-Group-39-2x.png" alt="logo">
            </div>
            <ul class="m-0">
                <li v-for="link in links">
                    <a href="#">{{ link }}</a>
                </li>
            </ul>
            <div>
                <button type="button" class="btn btn-grad btn-outline-success">PURCHASE</button>
                <i class="ms-4 fa-solid fa-magnifying-glass"></i>
            </div>
        </div>
    </section>
    <section class="jumbo">
        <div class="left">
            <h6>17 YEARS OF EXPERIENCE</h6>
            <h2>We Are a Web Design <span class="coloring-text">Agency</span></h2>
            <div class="d-flex gap-2">
                <span class="point"></span>
                <hr class="line">
            </div>
            <p>
                Far far away, behind the word mountains, far from the countries Vokalia and Consonantia,
                there live the blind texts.Separated they live in Bookmarksgrove right at the coast of the 
                Semantic, a large language ocean.Separated they live in Bookmarksgrove.
            </p>
            <button type="button" class="btn btn-black btn-outline-secondary">READ MORE</button>
            <div class="mt-5 d-flex gap-5">
                <ul>
                    <li v-for="social in socials">
                        <a href="#">{{ social }}</a>
                    </li>
                </ul>
                <div class="btn-group rounded-pill p-1" role="group" aria-label="Basic example">
                    <button @click="switchImage(1)" type="button" class="btn rounded-pill" :class="image.id === 1 ? 'btn-grad-btn' : ''">01</button>
                    <button @click="switchImage(2)" type="button" class="btn rounded-pill" :class="image.id === 2 ? 'btn-grad-btn' : ''">02</button>
                    <button @click="switchImage(3)" type="button" class="btn rounded-pill" :class="image.id === 3 ? 'btn-grad-btn' : ''">03</button>
                </div>
            </div>
        </div>
        <div class="right">
            <img :src="image.src" alt="group">
        </div>
    </section>
 </header>
</template>

<style lang="scss">
@use '../styles/responsive/responsive.scss' as *;

.header-fixed{
    position: fixed;
    left: 0;
    right: 0;
    top: 0;
    z-index: 9999;
    background-color: #fff;
}

.banda-recapiti{
    display: flex;
    padding: 0 50px;
    justify-content: space-between;
    align-items: center;
    height: 40px;
    background-color: #3b3b3b;
    color: #fff;
}

.banda-dinamica{
    height: 100px;
    display: flex;
    justify-content: space-around;
    align-items: center;

    .logo{
        width: 50px;
        height: 50px;
    }
}

.jumbo{
    display: flex;
    background-color: #fafafa;
    justify-content: space-between;
    margin-top: 100px;
}

h6{
    background: linear-gradient(90deg, rgba(6,217,163,1) 0%, rgba(79,221,129,1) 43%, rgba(147,224,97,1) 100%);
    background-clip: text;
    -webkit-text-fill-color: transparent;
    font-size: 1.3rem;
}

.left{
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    margin: 100px 20px;
    width: 40%;
}

.right{
    width: 900px;
    overflow: hidden;
    position: relative;
    animation-name: mymoves;
    animation-duration: 3s;
    img{
        width: 100%;
        display: block;
        margin-left: 103px;
    }
}

@keyframes mymoves {
    0%   {left: 400px;}
    100% {left: 0px;}
}
</style>
