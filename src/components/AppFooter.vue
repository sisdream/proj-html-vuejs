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
                <i class="fa-solid fa-arrow-up"></i>
            </span>
            <span class="comment">
                <i class="fa-regular fa-comment"></i>
            </span>
        </div>
    </section>
</footer>
</template>

<style>
.info{
    padding: 100px;
}

.info li,
.info li a{
    color: #7e7e7e;
    
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
    display: flex;
    align-items: center;
    justify-content: center;
    width: 30px;
    height: 30px;
    border-radius: 50%;
    background-color: #fff;
    color: #7e7e7e;
    cursor: pointer;
}

.comment{
    display: flex;
    align-items: center;
    justify-content: center;
    width: 50px;
    height: 50px;
    border-radius: 50%;
    background-color: #527ceb;
    cursor: pointer;
}
</style>