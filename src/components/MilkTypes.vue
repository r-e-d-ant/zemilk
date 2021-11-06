
<template>
    <!-- section two -->
        <section class="section milk__type-section container" id="milks-types">
            <h2 class="section-title">
                ZeMilk have tremendous different kind of milk which satisfy everyone
            </h2>
            <div class="milk-types-container">
                <!-- Milk type one -->
                <div class="milk-type">
                    <img src="../assets/images/milk1.png" alt="milk type">
                    <div class="milk-type-info-container">
                        <h3>Delicious milk to drink at place</h3>
                        <p>
                            Etiam lacus ex, volutpat at massa at, laoreet mollis ipsum. Sed
                            eu efficitur augue. Mauris vel cursus mi Cras ac molestie
                        </p>
                    </div>
                </div>
                
                <!-- Milk type Two -->
                <div class="milk-type">
                    <img src="../assets/images/milk2.png" alt="milk type">
                    <div class="milk-type-info-container">
                        <h3>Yummy and soft milk for take away</h3>
                        <p>
                            Nam tincidunt vehicula lectus, at maximus lorem suscipit vitae.
                            Nam mattis massa at diam facilisis, sit amet aliquet
                        </p>
                    </div>
                </div>

                <!-- Milk type Three -->
                <div class="milk-type">
                    <img src="../assets/images/milk3.png" alt="milk type">
                    <div class="milk-type-info-container">
                        <h3>Yummy milk which last long days</h3>
                        <p>
                            Proin eleifend, sapien et ullamcorper aliquet, enim nisl auctor ex,
                            ut convallis massa nisl nec metus. Curabitur
                        </p>
                    </div>
                </div>

                <!-- Milk type Four -->
                <div class="milk-type">
                    <img src="../assets/images/milk4.png" alt="milk type">
                    <div class="milk-type-info-container">
                        <h3>Milk to take miles away and stay soft</h3>
                        <p>
                            Fusce ut lacus volutpat, sagittis sapien quis, ultricies tortor.
                            Maecenas lacinia tristique interdum. Donec eu quam
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
    font-weight: 200;
    font-size: 1.15rem;
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