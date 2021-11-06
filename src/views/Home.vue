
<template>
  <main>
    <!-- section one -->
        <section class="section hero-section">
            <div class="hero-hook__container">
                <div class="hook-container">
                    <h1 class="hero-title">Why drink unhealthy, when you have milk</h1>
                    <h2 class="hero-sub__title">Maecenas lacinia tristique interdum. donec eu quam efficitur ultrices ex sit amet elementum sapien.</h2>
                    <router-link :to="{ name: 'Contact' }">Become Client</router-link>
                </div>
            </div>
            <div class="benefits-section">
                <div class="benefit-one benefit">
                    <span class="no">01</span>
                    <h2 class="benefit-title">Yummy milk</h2>
                    <p class="benefit-desc">Donec nisl tellus, blandit nec mauris eget, tincidunt ornare nibh. Donec nunc turpis, elementum vel</p>
                </div>
                <div class="benefit-two benefit">
                    <span class="no">02</span>
                    <h2 class="benefit-title">No Additive</h2>
                    <p class="benefit-desc">Phasellus vestibulum ex non risus ultricies, a ullamcorper velit ultricies. Morbi lacinia ornare est lacinia</p>
                </div>
                <div class="benefit-three benefit">
                    <span class="no">03</span>
                    <h2 class="benefit-title">Rich in protein</h2>
                    <p class="benefit-desc">consectetur adipiscing elit. Aenean est ex, suscipit id felis amet, tincidunt lacinia metus. Nulla congue</p>
                </div>
            </div>
        </section>
        <MilkTypes/>
        <Testimonials/>
  </main>
</template>

<script>
import Testimonials from '../components/Testimonials.vue'
import MilkTypes from '../components/MilkTypes.vue'

export default {
  name: 'Home',
  components: { Testimonials, MilkTypes }
}
</script>

<style scoped>
.hero-section {
    position: relative;
}

/* -- hero section sylings -- */
.hero-hook__container {
    padding: .5rem;
    background-image: url(../assets/images/cows.png);
    background-color: var(--white-clr-alt);
    height: 80vh;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    overflow: hidden;
}
.hook-container {
    padding-top: 0rem;
}
@media screen and (min-width: 700px) {
    .hero-hook__container {
        padding: 0 1rem;
    }
    .hook-container {
        padding-top: 5rem;
    }
}
@media screen and (min-width: 1024px) {
    .hero-hook__container {
        padding: 0 1rem;
    }
    .hook-container {
        padding-top: 7rem;
    }
}
.hero-title {
    color: var(--white-clr);
    font-family: 'Fruktur', cursive;
    font-size: 2.9rem;
    font-weight: 800;
    max-width: 35rem;
    letter-spacing: .2rem;
}
.hero-sub__title {
    color: var(--white-clr);
    font-family: 'Open Sans Condensed', sans-serif;
    font-size: 1rem;
    font-weight: 600;
    max-width: 28rem;
    margin-top: .8rem;
    margin-bottom: 2rem;
}
.hook-container a {
    background-color: var(--white-clr);
    color: var(--primary-clr);
    text-decoration: none;
    font-size: 1.3rem;
    font-weight: 500;
    padding: 1rem 2rem;
    border-radius: 45px;
    transition: background-color 150ms;
}
.hook-container a:hover {
    background-color: var(--input-border-clr);
}

@media screen and (min-width: 700px) {
    .hero-title {
        font-size: 3.5rem;
    }
    .hero-sub__title {
        font-size: 1.5rem;
        font-weight: 400;
        margin-top: 1.2rem;
        margin-bottom: 4rem;
        max-width: 50rem;
    }
    .hook-container a {
        padding: 1rem 4rem;
    }
}
@media screen and (min-width: 1024px) {
    .hero-title {
        font-size: 5rem;
        font-weight: 800;
        line-height: 6rem;
        max-width: 60rem;
    }
    .hero-sub__title {
        font-size: 1.6rem;
        max-width: 40rem;
    }
}

/* -- benefits sylings -- */
.benefits-section {
    padding: 0 .5rem;
    margin: .1rem 0 3rem 0;
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: space-between;
}
@media screen and (min-width: 768px) {
    /* -- benefits sylings -- */
    .benefits-section {
        padding: 0 1rem;
        margin: 1.2rem 0 3rem 0;
    }
}
.benefit {
    margin: .5rem 0;
    background-color: var(--card-clr);
    padding: 2rem;
    width: 19.5rem;
    height: 15rem;
    position: relative;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;
}
.benefit
.no {
    position: absolute;
    top: 1rem;
    left: .5rem;
    font-size: 1.2rem;
    font-weight: 600;
    color: var(--gray-clr);
    opacity: .5;
}
.benefit
.benefit-title {
    font-size: 1.5rem;
    font-weight: 400;
    margin-bottom: .5rem;
    margin-top: 1rem;
}
.benefit
.benefit-desc {
    font-size: 1.1rem;
    line-height: 1.6;
    font-weight: 200;
}
</style>
