
<template>
  <main>
    <!-- section one -->
        <section class="about-section container">
            <div class="zeMilk-abouts">
                <!-- about -->
                <div class="about-one about">
                    <img src="../assets/images/hist1.png" alt="">
                    <div class="zemilk-history-container">
                        <div class="zemilk-years">2009 - 2013</div>
                        <p class="history">
                            Phasellus vestibulum ex non risus ultricies, a ullamcorper velit ultricies. Morbi lacinia ornare est lacinia ornare. In et pulvinar elit. Suspendisse sit amet condimentum libero, quis pretium sem. Nam rhoncus scelerisque porta. Aenean dolor sem
                        </p>
                        <p class="history">
                            Praesent eget efficitur urna. Fusce efficitur, elit et dignissim suscipit, augue enim convallis arcu, a rutrum sapien libero quis ante.
                        </p>
                    </div>
                </div>

                <!-- about -->
                <div class="about-two about">
                    <div class="zemilk-history-container">
                        <div class="zemilk-years">2013 - 2016</div>
                        <p class="history">
                            Donec nisl tellus, blandit nec mauris eget, tincidunt ornare nibh. Donec nunc turpis, elementum vel scelerisque id, tristique eu urna. Morbi lectus leo, maximus ut interdum ac, sagittis sed libero.
                        </p>
                        <p class="history">
                            Duis ultricies tellus non tortor sollicitudin, vitae ultrices neque tempor. Aliquam sodales semper nisl, sit amet rutrum velit consequat
                        </p>
                    </div>
                    <img src="../assets/images/hist2.png" alt="">
                </div>

                <!-- about -->
                <div class="about-three about">
                    <img src="../assets/images/hist3.png" alt="">
                    <div class="zemilk-history-container">
                        <div class="zemilk-years">2016 - 2018</div>
                        <p class="history">
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean efficitur quis eros pulvinar consectetur. Ut ante eros, euismod eget Phasellus posuere sapien in iaculis cursus. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos
                        </p>
                        <p class="history">
                            Curabitur eget dui augue. Suspendisse consequat est in cursus volutpat.
                        </p>
                    </div>
                </div>

                <!-- about -->
                <div class="about-four about">
                    <div class="zemilk-history-container">
                        <div class="zemilk-years">2018 - 2021</div>
                        <p class="history">
                            Maecenas lacinia tristique interdum. Donec eu quam efficitur, ultrices ex sit amet, elementum sapien. Ut nec rhoncus turpis, ac viverra ipsum. Morbi a vestibulum lorem. Fusce ut lacus volutpat, sagittis sapien quis, ultricies tortor.
                        </p>
                        <p class="history">
                            Praesent eget efficitur urna. Fusce efficitur, elit et dignissim suscipit, augue enim convallis arcu, a rutrum sapien libero quis ante.
                        </p>
                    </div>
                    <img src="../assets/images/hist4.png" alt="">
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
  name: 'About',
  components: { Testimonials, MilkTypes }
}
</script>

<style scoped>
.about-section {
    margin-top: .5rem;
}

.about {
    margin-bottom: 2rem;
}

@media screen and (min-width: 900px) {
    .about-section {
        margin-top: 2rem;
    }
    .zeMilk-abouts {
        display: flex;
        flex-direction: column;
        align-items: center;
    }
    .about {
        display: flex;
        margin-bottom: 5rem;
    }
}

.about
img {
    border-radius: 10px 10px 0 0;
}
.about-two img,
.about-four img {
    border-radius: 0 0 10px 10px;
}


@media screen and (min-width: 428px) {
    .about
    img {
        width: 405px;
        height: 290.2px;
    }
}
@media screen and (min-width: 900px) {
    .about
    img {
        border-radius: 50px 0 50px 0;
    }
    .about-two img,
    .about-four img {
        border-radius: 0 50px 0 50px;
    }
}

.zemilk-years {
    font-weight: 400;
    color: var(--white-clr-alt);
    margin-bottom: .3rem 0;
}

@media screen and (min-width: 976px) {
    .zemilk-years {
        font-size: 1.1rem;
        margin-top: 0;
        margin-bottom: .8rem;
    }
}

.history {
    font-weight: 200;
    font-size: 1.1rem;
    max-width: 25rem;
    margin-bottom: 1rem;
}
.about-two .history,
.about-four .history {
    margin-bottom: 1.2rem;
}

@media screen and (min-width: 900px) {
    .zemilk-history-container {
        margin-left: 1.5rem;
    }
    .about-two .zemilk-history-container,
    .about-four .zemilk-history-container {
        text-align: right;
        margin-right: 1.5rem;
    }
    .about-two .history,
    .about-four .history {
        margin-bottom: 1.2rem;
    }
    .about-two .history:last-child,
    .about-four .history:last-child {
        margin-bottom: 0;
    }

    .history {
        max-width: 40rem;
        margin-bottom: 1rem;
        line-height: 2rem;
    }
    .history:last-child {
        margin-bottom: 0;
    }
}
@media screen and (min-width: 976px) {
    .history {
        font-size: 1.2rem;
    }
}
</style>