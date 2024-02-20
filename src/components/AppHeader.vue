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
                ]
            }
        },
    }
</script>

<template>
 <header>
    <section class="header-fixed">
        <div class="banda-recapiti"></div>
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
            <hr class="line">
            <p>
                Far far away, behind the word mountains, far from the countries Vokalia and Consonantia,
                there live the blind texts.Separated they live in Bookmarksgrove right at the coast of the 
                Semantic, a large language ocean.Separated they live in Bookmarksgrove.
            </p>
            <button type="button" class="btn btn-black btn-outline-secondary">READ MORE</button>
            <div class="mt-5">
                <ul>
                    <li v-for="social in socials">
                        <a href="#">{{ social }}</a>
                    </li>
                </ul>
            </div>
        </div>
        <div class="right">
            <img src="/images/Group-36-2x.png" alt="group">
        </div>
    </section>
 </header>
</template>

<style lang="scss">
.header-fixed{
    position: fixed;
    left: 0;
    right: 0;
    top: 0;
    z-index: 9999;
    background-color: #fff;
}

.banda-recapiti{
    height: 40px;
    background-color: #3b3b3b;
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
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    font-size: 300;
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

    img{
        width: 100%;
        display: block;
        margin-left: 103px;
    }
}

</style>
