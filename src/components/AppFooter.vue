<script>
export default {
    data () {
        return {
            links: [
                'Careers',
                'News',
                'Terms of use',
                'Privacy Projects',
                'About',
                'Contact'
            ],
        }
    },
}
</script>

<template>
<footer>
    <div class="demo">
        <div class="demo-contain">
            <div class="demo-btn">
                <i class="fa-solid fa-table-cells-large me-1"></i>
                <span>Browse Demos</span>
            </div>

            <div class="demo-btn">
                <i class="fa-solid fa-bag-shopping me-1"></i>
                <span>Buy Now!</span>
            </div>

            <div class="demo-btn">
                <i class="fa-solid fa-right-from-bracket me-1"></i>
                <span>Export Section</span>
            </div>
        </div>
    </div>
    <section class="info">
        <div class="row">
            <div class="col">
                <div class="logo">
                    <img src="/images/cropped-Group-39-2x.png" alt="logo">
                </div>
                <p class="mt-3">
                    While the lovely valley teems whit vapour around me, 
                    and the meridian sun strikes the upper surface of the 
                    impenetrable foliage of my trees.while the lovely valley
                    teems with vapour around me.
                </p>
            </div>
            <div class="col">
                <h4>QUICK LINKS</h4>
                <div class="d-flex gap-2">
                    <span class="point"></span>
                    <hr class="line">
                </div>
                <ul class="p-0 d-flex flex-column">
                    <li v-for="link in links">
                        <a href="#">{{ link }}</a>
                    </li>
                </ul>
            </div>
            <div class="col">
                <h4>CONTACT</h4>
                <div class="d-flex gap-2">
                    <span class="point"></span>
                    <hr class="line">
                </div>
                <ul class="p-0 d-flex flex-column">
                    <li>
                        Patricia C. Amedee 4401 Waldeck Street
                        Grapevine Nashville, TX 76051
                    </li>
                    <li><a href="#">info@yourdomain.com</a></li>
                    <li>+99 (0) 101 0000 888</li>
                </ul>
            </div>
            <div class="col">
                <h4>LOCATION ON MAP</h4>
                <div class="d-flex gap-2">
                    <span class="point"></span>
                    <hr class="line">
                </div>
                <div class="map">
                    <img src="/images/map.png" alt="map">
                </div>
            </div>
        </div>
    </section>
    <section class="copy">
        <p>
            <i class="fa-regular fa-copyright"></i>
            2020 PHLOXBUSINESS THEME
        </p>
        <div class="d-flex gap-3 align-items-center">
            <span class="arrow">
                <a href="#top"><i class="fa-solid fa-arrow-up"></i></a>
            </span>
            <span class="comment">
                <i class="fa-regular fa-comment"></i>
            </span>
        </div>
    </section>
</footer>
</template>

<style lang="scss">
@use '../styles/responsive/responsive.scss' as *;

.demo{
    position: fixed;
    right: 0px;
    top: 50%;
    z-index: 9999;
    transform: translate(20px,-50%);
}

.demo-contain{
    display: flex;
    flex-direction: column;
    gap: 0.4rem;
}

.demo-btn{
    width: 200px;
    position: relative;
    right: -30px;
    color: #fff;
    background-color: #858585;
    border-radius: 5px;
    padding: 5px 10px;
    transition: ease-in-out .3s;
    cursor: pointer;
    &:hover{
        background-color: #527ceb;
        right: 0;
    }
}


.info{
    padding: 100px;
}

.info li,
.info li a{
    color: #7e7e7e;
    
}

.map{
    cursor: grab;
}

.copy{
    background: linear-gradient(90deg, rgba(2,0,36,1) 0%, rgba(64,64,64,1) 0%, rgba(5,5,5,1) 100%);
    height: 100px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0 50px;
}

.arrow{
    position: fixed;
    right: 100px;
    bottom: 5%;
    z-index: 80;
    display: flex;
    align-items: center;
    justify-content: center;
    width: 30px;
    height: 30px;
    border-radius: 50%;
    background-color: #fff;
    border: 1px solid #7e7e7e;
    color: #7e7e7e;
    cursor: pointer;
    &:hover{
        border-color: #fff;
        background-color: #7e7e7e;
    }
    &:hover i{
        color: #fff;
    }
}

.comment{
    position: fixed;
    right: 30px;
    bottom: 5%;
    z-index: 80;
    display: flex;
    align-items: center;
    justify-content: center;
    width: 50px;
    height: 50px;
    border-radius: 50%;
    background-color: #527ceb;
    color: #fff;
    cursor: pointer;
    &:hover{
        filter: brightness(1.2);
    }
}
</style>