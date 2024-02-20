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
                <p>
                    While the lovely valley teems whit vapour around me, 
                    and the meridian sun strikes the upper surface of the 
                    impenetrable foliage of my trees.while the lovely valley
                    teems with vapour around me.
                </p>
            </div>
            <div class="col">
                <h4>QUICK LINKS</h4>
                <ul class="d-block ">
                    <li v-for="link in links">
                        <a href="#">{{ link }}</a>
                    </li>
                </ul>

            </div>
            <div class="col"></div>
            <div class="col"></div>
        </div>
    </section>
    <section class="copy"></section>
</footer>
</template>

<style>
.info{
    height: 700px;
}
</style>