<template>
    <div id="screen">
        <header>
            <div id="logoContainer">
                 <Link href="/">
                        <fa icon="users-line" />
                        <span> まなび </span>
                    </Link>
            </div>

            <nav>
                <div class="links">
                    <Link href="/">
                        <fa icon="users-line" />
                        <span> Custom </span>
                    </Link>
                </div>
                <div class="links">
                    <Link href="/">
                        <fa icon="users-line" />
                        <span> Rank </span>
                    </Link>
                </div>
                <div class="links">
                    <Link href="/">
                        <fa icon="users-line" />
                        <span> Titul </span>
                    </Link>
                </div>
                
            </nav>
            <div id="profile">
                <div>
                    Profil
                </div>
            </div>
        </header>

        <article>
            <slot />
        </article>
    </div>
</template>

<script>
import { Link } from "@inertiajs/vue3";
import axios from "axios";

export default {
    components: {
        Link,
    },
    
    methods: {
    },
};
</script>

<style>
html, body {
    padding: 0;
    margin: 0;
}
header {
    width: 100%;
    height: 80px;
    background-color: #228B22;
    display: flex;
}

#logoContainer {
    color: white;
    padding: 10px;
    font-size: 42px;
    flex: 40%;
}

nav{
    padding: 10px;
    flex: 50%;
    display: flex;
    align-items: center;
}
.links span{
    padding: 16px;
    font-size: 24px;
 }
 a {
    color: white;
    text-decoration: none;
 }

 a:active {
   color: rgba(255, 255, 255, 0.6);
 }
 #profile {
    flex: 10%;
    display: flex;
    align-items: center;
 }
 #profile div{
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: #D9D9D9;
    width: 50px;
    height: 50px;
    border-radius: 50%;
    user-select: none;
 }

  #profile div:active{
    transform: scale(0.9);
 }
</style>
