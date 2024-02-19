<script>
</script>

<template>
<main>
    <section class="website">
        <div class="website-left">
            <h2>We Are Here To Make Your Website Look More Elegant And Stylish</h2>
            <button type="button" class="btn btn-grad btn-outline-success">VIEW ALL</button>
        </div>

        <div class="website-right">
            <div class="card web-card">
                <div class="icon mt-3 mb-4">
                    <i class="fa-solid fa-gauge-high"></i>
                </div>
                <h4 class="mb-4">Speed Optimization</h4>
                <p>Far far away,bhehind the word mountains, far from the countries Vokalia Separated...</p>
            </div>

            <div class="card web-card">
                <div class="icon mt-3 mb-4">
                    <i class="fa-solid fa-cloud"></i>
                </div>
                <h4 class="mb-4">Cloud Solution</h4>
                <p>Far far away,bhehind the word mountains, far from the countries Vokalia Separated...</p>
            </div>

            <div class="card web-card">
                <div class="icon mt-3 mb-4">
                    <i class="fa-solid fa-tablet-screen-button"></i>
                </div>
                <h4 class="mb-4">Website Design</h4>
                <p>Far far away,bhehind the word mountains, far from the countries Vokalia Separated...</p>
            </div>

            <div class="card web-card">
                <div class="icon mt-3 mb-4">
                    <i class="fa-solid fa-stopwatch"></i>
                </div>
                <h4 class="mb-4">Online Marketing</h4>
                <p>Far far away,bhehind the word mountains, far from the countries Vokalia Separated...</p>
            </div>
        </div>
    </section>
    <section class="missions">
        <div class="mission-left">
            <div class="architect">
                <img src="/images/busy-architect-PYVKWM4-1024x872.jpg" alt="">
                <div class="arc-color"></div>
                <div class="businesswoman">
                    <img src="/images/businesswoman-analysing-document-P8WSNMC-1024x820.jpg" alt="">
                </div>
            </div>
        </div>

        <div class="mission-right">
            <h2>Learn more about our missions</h2>
            <p>
                Far far away, behind the word mountains, far from the countries Vokalia and Consonantia,
                there live the blind texts.Separated they live in Bookmarksgrove right at the coast of the 
                Semantic, a large language ocean.Separated they live in Bookmarksgrove.
            </p>
            <div>
                <button type="button" class="btn btn-grad btn-outline-success">READ MORE</button>
            </div>
        </div>
    </section>
    <section class="project">
        <div class="project-top">
            <h2>Our recent web designs &#38; some examples of past projects </h2>
            <p class="pro-p">
                Far far away, behind the word mountains, far from the countries Vokalia and Consonantia,
                there live the blind texts.Separated they live in Bookmarksgrove right at the coast of the 
                Semantic, a large language ocean.Separated they live in Bookmarksgrove.Separated they live in Bookmarksgrove 
                right at the coast of the Semantic, a large language ocean.
            </p>
        </div>
        <div class="project-bottom">
            <div class="cube">
                <img src="/images/ina-soulis-227104-unsplash-1024x1024.jpg" alt="fiori">
            </div>
            <div class="cube">
                <img src="/images/sunisa-misa-531163-unsplash-1024x1024.jpg" alt="ruota panoramica">
            </div>
            <div class="cube">
                <img src="/images/355H-1024x1024.jpg" alt="scarpe gialle">
            </div>
            <div class="cube">
                <img src="/images/photo-1448932252197-d19750584e56-1024x1024.jpg" alt="lavoro">
            </div>
            <div class="cube">
                <img src="/images/business-competition-PB366D8-1024x1024.jpg" alt="origami">
            </div>
            <div class="cube">
                <img src="/images/cozy-sofa-in-living-room-PQR5AB9-1024x1024.jpg" alt="divano">
            </div>
            <div class="cube">
                <img src="/images/aa9a4539-PQGJ7HU-1024x1024.jpg" alt="mongolfiere">
            </div>
            <div class="cube">
                <img src="/images/cody-davis-253928-unsplash-1024x1024.jpg" alt="agrume blu">
            </div>
        </div>
        <div class="d-flex justify-content-center mt-5 mb-5">
            <button type="button" class="btn btn-grad btn-outline-success">READ MORE</button>
        </div>
    </section>
    <section class="client"></section>
    <section class="blog"></section>
    <section class="work"></section>
</main>
</template>

<style>
.website{
    display: flex;
    margin-top: 30px;
}

.website-left{
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    width: 40%;
}

.icon i{
    font-size: 3rem;
}

.website-right{
    display: flex;
    gap: 4rem;
    width: 60%;
    flex-wrap: wrap;
}

.missions{
    display: flex;
    margin-top: 50px;
    background-color: #f9f9f9;
    .mission-left{
        width: 60%;
        margin: 100px 0;
    }
}

.mission-right{
    width: 40%;
    display: flex;
    flex-direction: column;
    justify-content: center;
    margin: 100px 0;
}

.architect{
    width: 520px;
    position: relative;
    img{
        width: 100%;
        border-radius: 20px;
    }
}
.arc-color{
    width: 520px;
    background-color: #38d99b;
    opacity: 0.9;
    height: 450px;
    position: absolute;
    top: 0;
    z-index: 1;
    border-radius: 20px;
}
   
.businesswoman{
    width: 500px;
    position: absolute;
    z-index: 2;
    left: 7rem;
    top: 4rem;
    img{
        width: 100%;
        border-radius: 20px;
    }
}

.project-top{
    display: flex;
    gap: 5rem;
    margin: 20px 30px;
    .pro-p{
        width: 60%;
        margin-top: 3rem;
    }
}

.project-bottom{
    display: flex;
    flex-wrap: wrap;
    margin: 0 10px;
}

.cube{
    margin: 4px;
    width: calc(100% / 4 - 10px);
    height: calc(100vw/ 4 - 20px);
    
    img{
        width: 100%;
        border-radius: 20px;
    }
}
</style>