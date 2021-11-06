
<template>
    <footer>
        <div class="upper-footer container">
            <div class="footer-links-container">
                <ul class="footer-links">
                    <h3 class="footer-links-title">Address</h3>
                    <li class="footer-link">Gihinga 12kG 18st load</li>
                    <li class="footer-link">Mwaro, Nyabihanga</li>
                    <li class="footer-link">amata@domain.com</li>
                    <li class="footer-link">+002 2020 123 020</li>
                </ul>
                <ul class="footer-links">
                    <h3 class="footer-links-title">Product</h3>
                    <li class="footer-link">Benefits</li>
                    <li class="footer-link">How we sell</li>
                    <li class="footer-link">Testimonials</li>
                    <li class="footer-link">Sponsors</li>
                </ul>
                <ul class="footer-links">
                    <h3 class="footer-links-title">Agency</h3>
                    <li class="footer-link">About</li>
                    <li class="footer-link">Contact</li>
                </ul>
            </div>

            <div class="footer-splash-milk">
                <img src="../assets/images/milk.png" alt="milk splash">
            </div>
        </div>

        <div class="middle-footer logo container">ZeMilk</div>

        <div class="lower-footer container">
            <span>Copyright © 2021 ZeMilk</span>

            <div class="author">Developed by <a href="https://thierrymugisha.me" target="_blank">T Mugisha</a></div>

            <div class="privacy-policy">
                <a href="#" class="terms">Terms & Conditions</a>
                <div class="privacy-container">
                    <a href="#" class="privacy">Privacy</a>
                    <a href="#" class="privacy">Policy</a>
                </div>
            </div>
        </div>
    </footer>
</template>

<style scoped>
footer {
    display: flex;
    flex-direction: column;
    background-color: var(--primary-clr);
    padding-bottom: 1rem;
}

/* -- upper footer -- */
@media screen and (min-width: 768px) {
    .footer-links-container {
        display: flex;
        justify-content: space-between;
    }
}
.footer-links {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    margin: 2rem 0;
}
.footer-links-title {
    color: var(--white-clr);
    margin-bottom: .2rem;
}
.footer-link {
    color: var(--gray-clr-alt);
    font-size: .9rem;
    font-weight: 200;
}

.footer-splash-milk {
    display: none;
}

@media screen and (min-width: 1024px) {
    .upper-footer {
        display: flex;
        justify-content: space-between;
    }
    .footer-links-container {
        width: 100%;
    }
    .footer-splash-milk {
        display: block;
        width: 30rem;
        margin-left: 10rem;
    }
}

/* -- middle footer -- */
.middle-footer {
    margin-bottom: 1rem;
}

/* -- lower footer -- */
.lower-footer {
    margin-top: 1rem;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    gap: .5rem;
    position: relative;
    padding-top: 1.5rem;
}
.lower-footer::before {
    content: "";
    background-color: var(--card-clr);
    position: absolute;
    top: 0;
    height: .05rem;
    width: 100%;
}
.privacy-policy {
    display: flex;
    align-items: center;
}
.privacy-policy .terms {
    margin-right: 1.5rem;
}
.privacy-container {
    display: flex;
    align-items: center;
}
.privacy-container a:first-child {
    margin-right: .5rem;
}
.lower-footer span,
.lower-footer .author,
.privacy-policy .terms,
.privacy-container .privacy {
    color: var(--gray-clr);
    font-size: .8rem;
}

.lower-footer
.author 
a {
    color: var(--white-clr);
}
</style>