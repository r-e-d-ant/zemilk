
<template>
<main>
    <!-- section one -->
        <section class="hook-section container">
            <div class="section-contact-hook-container">
                <div class="hook-text">
                    <p>Maecenas lacinia tristique interdum. Donec eu quam efficitur, ultrices ex sit amet, elementum sapien. Ut nec rhoncus turpis, ac viverra ipsum. Morbi a vestibulum lorem. Fusce ut lacus volutpat, sagittis sapien quis, ultricies tortor. Nunc ut quam in elit feugiat vehicula.</p>
                    <p>Praesent eget efficitur urna. Fusce efficitur, elit et dignissim suscipit, augue enim convallis arcu, a rutrum sapien libero quis ante.</p>
                </div>
                <img src="../assets/images/milk.png" alt="">
            </div>
        </section>

        <!-- section two -->
        <section class="section form-contact-section container">
            <div class="form-container">
                <form>
                    <div class="upper-forms">
                        <div class="left-upper-forms">
                            <div class="input-div">
                                <label for="firstName" class="input-label">First name</label>
                                <input type="text" id="firstName" class="input-regular">
                            </div>
                            <div class="input-div">
                                <label for="lastName" class="input-label">Last name</label>
                                <input type="text" id="lastName" class="input-regular">
                            </div>
                        </div>

                        <!-- right -->
                        <div class="right-upper-forms">
                            <div class="input-div">
                                <label for="emailAddress" class="input-label">Email address</label>
                                <input type="text" id="emailAddress" class="input-regular">
                            </div>
                            <div class="input-div">
                                <label for="phoneNumber" class="input-label">Phone number</label>
                                <input type="text" id="phoneNumber" class="input-regular">
                            </div>
                        </div>
                    </div>
                    <div class="lower-input">
                        <label for="textInput" class="input-label">Message</label>
                        <textarea id="textInput" class="contact-message-input" cols="30" rows="10"></textarea>
                    </div>

                    <button type="submit" class="contact-btn">SEND</button>
                </form>
            </div>
            <div class="info-container">
                <h2>Our Contact</h2>
                <ul class="info-lists">
                    <!-- info list one -->
                    <li class="info-list-container">
                        <i class="bx bx-map"></i>
                        <div class="info-list">
                            <h3>Gihinga 12kG 18st load</h3>
                            <h3>Mwaro, Nyabihanga</h3>
                        </div>
                    </li>
                    <!-- info list two -->
                    <li class="info-list-container">
                        <i class="bx bx-mail-send"></i>
                        <div class="info-list">
                            <h3>amata@domain.com</h3>
                            <h3>amata@domain.com</h3>
                        </div>
                    </li>
                    <!-- info list three -->
                    <li class="info-list-container">
                        <i class="bx bx-phone-call"></i>
                        <div class="info-list">
                            <h3>+002 2020 123 020</h3>
                            <h3>+003 92120 921 020</h3>
                        </div>
                    </li>
                </ul>

                <div class="boule-deco"></div>
            </div>
        </section>
</main>
</template>

<style scoped>
.hook-section {
    background-color: var(--hook-bg-clr);
}
.section-contact-hook-container {
    display: flex;
    align-items: center;
    justify-content: space-between;
}
@media screen and (min-width: 984px) {
    .section-contact-hook-container {
        padding: 0 2rem;
    }
}
.section-contact-hook-container img {
    width: 280px;
    height: 280px;
    display: none;
}

.hook-text p {
    font-size: 1.1rem;
    max-width: 45rem;
    margin-bottom: 1rem;
}
.hook-text p:last-child {
    margin-bottom: 0;
}

@media screen and (min-width: 900px) {
    .hook-text p {
        font-size: 1rem;
        line-height: 2;
    }
    .section-contact-hook-container img {
        display: block;
    }
}


/* -- form section -- */
@media screen and (min-width: 984px) {
    .form-contact-section {
        display: flex;
        justify-content: space-around;
    }
}

.form-contact-section {
    margin: 2rem 0;
}
.upper-forms {
    display: flex;
    flex-direction: column;
}
.input-div {
    display: flex;
    flex-direction: column;
}
.input-label {
    font-size: 1.1rem;
    margin-bottom: .5rem;
}
.input-regular, .contact-message-input {
    color: var(--primary-clr);
    font-size: 1.2rem;
    height: 2.5rem;
    border: thin solid var(--input-border-clr);
    border-radius: 5px;
    outline: none;
    padding: 0 .5rem;
    margin-bottom: 1.5rem;
    transition: 150ms box-shadow;
}
.input-regular:focus, .contact-message-input:focus {
    box-shadow: 0 0 5px 1px #475d645b;
}

@media screen and (min-width: 984px) {
    .form-container {
        margin-right: 3rem;
    }
    .upper-forms {
        display: flex;
        flex-direction: row;
    }
    .left-upper-forms {
        margin-right: 3rem;
    }
    .input-label {
        font-size: 1rem;
    }
    .input-regular {
        width: 20rem;
    }
    .input-regular, .contact-message-input {
        height: 3rem;
    }
}

/* -- lower input -- */
.lower-input {
    display: flex;
    flex-direction: column;
}
.contact-message-input {
    height: auto;
    padding-top: 1rem;
}
.contact-btn {
    cursor: pointer;
    border: none;
    color: var(--white-clr);
    background-color: var(--primary-clr);
    font-size: 1.1rem;
    height: 3rem;
    width: 10rem;
    border-radius: 5px;
    letter-spacing: .1rem;
    transition: background-color 150ms;
}
.contact-btn:hover {
    background-color: var(--white-clr-alt);
}

/* -- contact information part -- */
.info-container {
    background-color: var(--card-clr);
    margin-top: 2rem;
    height: 511px;
    border-radius: 5px;
    padding: 0 1rem;
    position: relative;
    overflow: hidden;
}
@media screen and (min-width: 984px) {
    .info-container {
        height: 28.5rem;
        width: 25rem;
    }
}
.boule-deco {
    background-color: var(--gray-clr);
    width: 200px;
    height: 200px;
    border-radius: 50%;
    position: absolute;
    bottom:-5rem;
    left: -5rem;
}
.info-container h2 {
    font-size: 1.4rem;
    font-weight: 400;
    margin-bottom: 1.2rem;
    margin-top: 3rem;
}
@media screen and (min-width: 768px) {
    .info-container h2 {
        font-size: 1.3rem;
        font-weight: 400;
        margin-bottom: 1.5rem;
        margin-top: 1rem;
    }
}
.info-list-container {
    display: flex;
    align-items: flex-start;
    margin-bottom: 2rem;
}
.info-list-container
.bx {
    font-size: 1.5rem;
    opacity: .8;
}
.info-list-container
.info-list {
    margin-left: .8rem;
}
.info-list-container
.info-list
h3 {
   font-size: 1rem;
   font-weight: 400;
}
@media screen and (min-width: 768px) {
    .info-list-container
    .info-list
    h3 {
        font-size: .99rem;
        font-weight: 200;
    }
    .info-list-container
    .bx {
        font-size: 1.4rem;
    }
}
</style>