
<template>
    <!-- section three -->
        <section class="section testimonials-section container">
            <h2 class="section-title">
                Curabitur luctus ut dolor sed porttitor.
                Pellentesque in ipsum congue
            </h2>
            <div class="testimonials-n-sponsors-container">
                <div class="testimonials-container">
                    <!-- testimony one -->
                    <div class="testimony-container">
                        <p>Maecenas lacinia tristique interdum. Donec eu quam efficitur, ultrices ex sit amet, elementum sapien.</p>
                        <h3>Maecenas lacinia</h3>
                    </div>
                    <!-- testimony two -->
                    <div class="testimony-container">
                        <p>Maecenas lacinia tristique interdum. Donec eu quam efficitur, ultrices ex sit amet, elementum sapien.</p>
                        <h3>Maecenas lacinia</h3>
                    </div>
    
                    <!-- testimony three -->
                    <div class="testimony-container">
                        <p>Maecenas lacinia tristique interdum. Donec eu quam efficitur, ultrices ex sit amet, elementum sapien.</p>
                        <h3>Maecenas lacinia</h3>
                    </div>
                </div>

                <div class="sponsors container"></div>
                <div class="middle-call-to-action">
                    <h2>
                        Curabitur luctus ut dolor sed porttitor.
                        Pellentesque in ipsum congue
                    </h2>
                    <a class="call-action" href="#">Become Client</a>
                </div>
            </div>
        </section>
</template>
<style scoped>
/* section three */
.testimonials-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    gap: 1rem;
}
.testimony-container {
    background-color: var(--card-clr);
    border-radius: 10px;
    width: 22rem;
    padding: 2rem 0 2rem 2.2rem;
}
.testimony-container p {
    max-width: 18rem;
    font-size: 1.1rem;
    font-weight: 200;
}
.testimony-container h3 {
    max-width: 15rem;
    font-size: 1rem;
    margin-top: 1.2rem;
    font-weight: 600;
}

/* -- call to action part */

.middle-call-to-action {
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: space-between;
    gap: 2rem;
    margin: 5rem 0;
}
.middle-call-to-action h2 {
    max-width: 30rem;
    font-weight: 400;
}
.middle-call-to-action h2 {
    max-width: 30rem;
    font-weight: 400;
}
.call-action {
    background-color: var(--card-clr);
    border-radius: 0;
    padding: 1.3rem 3rem;
}
.call-action:hover {
    background-color: var(--input-border-clr);
}
</style>