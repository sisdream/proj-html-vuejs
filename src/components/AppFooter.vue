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
                <ul class="p-0 d-flex flex-column">
                    <li v-for="link in links">
                        <a href="#">{{ link }}</a>
                    </li>
                </ul>
            </div>
            <div class="col">
                <h4>CONTACT</h4>
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
                <div class="map">
                    <img src="/images/map.png" alt="map">
                </div>
            </div>
        </div>
    </section>
    <section class="copy"></section>
</footer>
</template>

<style>
.info{
    padding: 100px;
}

.copy{
    background: rgb(2,0,36);
    background: linear-gradient(90deg, rgba(2,0,36,1) 0%, rgba(115,115,115,1) 0%, rgba(24,24,24,1) 27%); 
    height: 100px;
}
</style>