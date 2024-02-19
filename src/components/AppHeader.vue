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
            <button type="button" class="btn btn-grad btn-outline-success">PURCHASE</button>
        </div>
    </section>
    <section class="jumbo">
        <div class="left">
            <h6>17 YEARS OF EXPERIENCE</h6>
            <h1>We Are a <br>
            Web Design Agency</h1>
            <p></p>
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
    margin: 100px auto;
}

.right{
   width: 900px;
    overflow: hidden;

    img{
        width: 100%;
        display: block;
        margin-left: 113px;
    }
}

</style>
