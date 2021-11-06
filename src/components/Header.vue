
<template>
    <header>
        <div class="logo">ZeMilk</div>
        <nav class="navbar" ref="navBar">
            <ul class="nav-lists">
                <li class="nav-item"><router-link :to="{ name: 'Home' }" class="nav-link">Home</router-link></li>
                <li v-show="$route.name !== 'Contact' " class="nav-item"><a href="#milks-types" class="nav-link">How We Sell</a></li>
                <li class="nav-item"><router-link :to="{ name: 'About' }" class="nav-link">About</router-link></li>
                <li class="nav-item"><router-link :to="{ name: 'Contact' }" class="nav-link">Contact</router-link></li>
            </ul>
        </nav>
        <div class="nav-menus">
            <i class='bx bx-menu' ref="menuOpenIcon" @click="openMenu"></i>
            <i class="bx bx-x" ref="menuCloseIcon" @click="closeMenu"></i>
        </div>
    </header>
</template>

<script>
import { ref } from 'vue'

export default {
    setup() {
        const navBar = ref(null)
        const menuOpenIcon = ref(null)
        const menuCloseIcon = ref(null)

        // Open Menu Function
        const openMenu = () => {
            /*
            check if showMenu class in not in navbar
            If not show it
            */
            if(!navBar.value.classList.contains('showMenu')) {
                navBar.value.classList.toggle('showMenu')
                menuOpenIcon.value.classList.toggle('hide')
                menuCloseIcon.value.classList.toggle('showClose')
            }
        }

        // Close Menu Function
        const closeMenu = () => {
            /*
            check if showMenu class is in navbar
            If true remove it
            */
            if(navBar.value.classList.contains('showMenu')) {
                navBar.value.classList.remove('showMenu')
                menuOpenIcon.value.classList.remove('hide')
                menuCloseIcon.value.classList.remove('showClose')
            }
        }

        return { navBar, menuOpenIcon, menuCloseIcon, openMenu, closeMenu }
    }
}
</script>

<style scoped>
header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    background-color: var(--primary-clr);
    padding: 1rem 1.5rem;
}
@media screen and (max-width: 768px) {
    header {
        padding: 1rem .5rem;
    }
}
/* nav items */
.navbar
.nav-lists {
    display: flex;
}
/* nav item */
.nav-lists
.nav-item {
    margin: 0 1rem;
}
.nav-lists
.nav-item
.nav-link {
    color: var(--white-clr);
    font-size: 1.05rem;
    font-weight: 500;
    text-decoration: none;
    position: relative;
}
.nav-link {
    position: relative;
}
.nav-link::before {
    content: "";
    background-color: var(--white-clr);
    position: absolute;
    bottom: 0;
    width: 100%;
    height: .14rem;
    transform: scaleX(0);
    transform-origin: right;
    transition: transform 300ms;
}
.nav-link:hover::before {
    transform: scaleX(1);
    transform-origin: left;
}
.router-link-exact-active {
    position: relative;
}
.router-link-exact-active::before {
    content: "";
    background-color: var(--white-clr);
    position: absolute;
    bottom: 0;
    width: 100%;
    height: .14rem;
    transform: scaleX(1);
    transform-origin: right;
    transition: transform 300ms;
}
.nav-menus {
    display: none;
}

@media screen and (min-width: 768px) {
    /* remove margin right to the last item */
    .nav-lists
    .nav-item:last-child {
        margin: 0;
    }
}
@media screen and (max-width: 768px) {
    .nav-menus {
        display: block;
        display: flex;
        align-items: center;
        justify-content: center;
    }
    .bx-menu,
    .bx-x {
        cursor: pointer;
        color: var(--white-clr);
        font-size: 2.5rem;
    }
    .bx-x {
        display: none;
    }
    .showClose {
        display: block;
    }
    /* navbar */
    .navbar {
        z-index: 1;
        background-color: var(--primary-clr);
        position: absolute;
        top: 4.2rem;
        right: 0;
        border-bottom-left-radius: .2rem;
        transform: scaleY(0);
        transform-origin: top;
        transition: 300ms transform;
    }
    .showMenu {
        transform: scaleY(1);
    }
    /* nav items */
    .navbar
    .nav-lists {
        flex-direction: column;
        padding: .8rem 2rem;
    }
    /* nav item */
    .nav-lists
    .nav-item {
        margin: 1rem 0;
    }
}
</style>