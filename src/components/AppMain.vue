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
    <section class="project"></section>
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
</style>