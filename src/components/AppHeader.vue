<script>

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
                <li><a href="#">HOME</a></li>
                <li><a href="#">ABOUT</a></li>
                <li><a href="#">SERVICES</a></li>
                <li><a href="#">SHOWCASE</a></li>
                <li><a href="#">BLOG</a></li>
                <li><a href="#">CONTACT</a></li>
            </ul>
            <button type="button" class="btn btn-grad btn-outline-success">PURCHASE</button>
        </div>
    </section>
    <section class="jumbo">
        <div class="left">
            <h6>17 YEARS OF EXPERIENCE</h6>
            <h1>We Are a <br>
            Web Design Agency</h1>
            <p>
                Far far away, behind the word mountains, far from the countries Vokalia and Consonantia,
                there live the blind texts.Separated they live in Bookmarksgrove right at the coast of the 
                Semantic, a large language ocean.Separated they live in Bookmarksgrove.
            </p>
            <button type="button" class="btn btn-black btn-outline-secondary">READ MORE</button>
            <div class="mt-5">
                <ul>
                    <li><a href="#">FACEBOOK</a></li>
                    <li><a href="#">INSTAGRAM</a></li>
                    <li><a href="#">YOUTUBE</a></li>
                    <li><a href="#">TWITTER</a></li>
                </ul>
            </div>
        </div>
        <div class="right">
            <img src="/images/Group-36-2x.png" alt="">
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
    color: #72e190;
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
