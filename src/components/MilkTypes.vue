
<template>
    <!-- section two -->
        <section class="section milk__type-section container" id="milks-types">
            <h2 class="section-title">
                Curabitur luctus ut dolor sed porttitor. Pellentesque in ipsum congue
            </h2>
            <div class="milk-types-container">
                <!-- Milk type one -->
                <div class="milk-type">
                    <img src="../assets/images/milk1.png" alt="milk type">
                    <div class="milk-type-info-container">
                        <h3>Maecenas lacinia tristique interdum</h3>
                        <p>
                            Fusce ut lacus volutpat, sagittis sapien quis, ultricies tortor.
                            Maecenas lacinia tristique interdum. Donec eu quam efficitur, ultrices ex sit amet
                        </p>
                    </div>
                </div>
                
                <!-- Milk type Two -->
                <div class="milk-type">
                    <img src="../assets/images/milk2.png" alt="milk type">
                    <div class="milk-type-info-container">
                        <h3>Maecenas lacinia tristique interdum</h3>
                        <p>
                            Fusce ut lacus volutpat, sagittis sapien quis, ultricies tortor.
                            Maecenas lacinia tristique interdum. Donec eu quam efficitur, ultrices ex sit amet
                        </p>
                    </div>
                </div>

                <!-- Milk type Three -->
                <div class="milk-type">
                    <img src="../assets/images/milk3.png" alt="milk type">
                    <div class="milk-type-info-container">
                        <h3>Maecenas lacinia tristique interdum</h3>
                        <p>
                            Fusce ut lacus volutpat, sagittis sapien quis, ultricies tortor.
                            Maecenas lacinia tristique interdum. Donec eu quam efficitur, ultrices ex sit amet
                        </p>
                    </div>
                </div>

                <!-- Milk type Four -->
                <div class="milk-type">
                    <img src="../assets/images/milk4.png" alt="milk type">
                    <div class="milk-type-info-container">
                        <h3>Maecenas lacinia tristique interdum</h3>
                        <p>
                            Fusce ut lacus volutpat, sagittis sapien quis, ultricies tortor.
                            Maecenas lacinia tristique interdum. Donec eu quam efficitur, ultrices ex sit amet
                        </p>
                    </div>
                </div>
            </div>
        </section>
</template>

<style scoped>
.milk-types-container {
    display: flex;
    flex-wrap: wrap;
    align-items: flex-start;
    justify-content: space-between;
}
.milk-type {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;
    margin-bottom: 2rem;
}
.milk-type img {
    width: 300px;
    border-radius: 30px 0 30px 0;
}
@media screen and (min-width: 1240px) {
    .milk-type {
        flex-direction: row;
        justify-content: flex-start;
        margin-bottom: 5rem;
    }
    .milk-type-info-container {
        margin-left: 1rem;
    }
    .milk-type img {
        width: 300px;
    }
}
.milk-type-info-container
h3 {
    max-width: 20rem;
    font-size: 1.5rem;
    font-weight: 400;
    margin: .5rem 0;
}
.milk-type-info-container
p {
    max-width: 18rem;
    line-height: 1.5;
}

@media screen  and (min-width: 1024px) {
    .milk-type-info-container
    h3 {
        max-width: 18rem;
        font-size: 1.5rem;
        font-weight: 400;
        margin-top: 0;
    }
    .milk-type-info-container
    p {
        margin-top: .5rem;
        max-width: 18rem;
        line-height: 1.5;
    }
}
</style>