<template>
    <div>
        <div>
            <!-- Cigarette Butts -->
            <section class="section__1">

                <div class="section__1--title">
                    OpenLitterMap data is <span class="section__1--title1">Open Data</span>
                </div>


            </section>
        </div>

        <section class="section-about">
            <div class="row">

                <div class="col-1-of-2">
                    <p class="paragraph paragraph-bold">The problem</p>
                    <p class="paragraph">
                        Every year, millions of tonnes of plastic makes its way from land to sea.
                        Where it becomes significantly more damaging, more difficult, & more expensive to remove.
                    </p>
                    <p class="paragraph paragraph-bold">The result</p>
                    <p class="paragraph">
                        Massive amounts of nicotine and other toxic chemicals get released.
                        These toxic chemicals bio-accumulate in various plants and animals. Some of which we eat.
                        An environmental emergency is at our fingertips.
                    </p>
                </div>

                <div class="col-1-of-2">
                    <div class="composition">
                        <img src="/assets/butts.jpg" alt="Photo 1" class="composition__photo composition__photo--p1">
                        <img src="/assets/can_litter.jpg" alt="Photo 2"
                             class="composition__photo composition__photo--p2">
                        <img src="/assets/plastic_bottles.jpg" alt="Photo 3"
                             class="composition__photo composition__photo--p3">
                    </div>
                </div>

            </div>
        </section>

        <!-- Call to action -->
        <section class="hero is-success">
            <div class="hero-body">
                <div class="container has-text-centered">
                    <h1 class="title">
                        <strong>
                            {{ $t('home.about.about7') }}
                        </strong>
                    </h1>
                    <!-- subtitle removed -->
                </div>
                <div class="has-text-centered">
                    <router-link to="/signup">
                        <button class="btn btn--white btn--animated">{{ $t('home.about.about9') }}</button>
                    </router-link>
                </div>
            </div>
        </section>

        <section class="take__action">
            <!-- 1. Just take a photo -->
            <div class="take__action-1 has-text-centered pt3">
                <h1 class="title">1. {{ $t('home.about.about9a') }}</h1>

                <img src="/assets/about/take_a_photo.PNG"/>
            </div>

            <!-- 2. Tag it with our app -->
            <div class="take__action-1 has-text-centered pt3">
                <h1 class="title">2. {{ $t('home.about.about9b') }}</h1>

                <img src="/assets/about/facemask-tag.PNG"/>
            </div>

            <!-- 3. Upload it -->
            <div class="take__action-1 has-text-centered pt3">
                <h1 class="title">3. {{ $t('home.about.about9c') }}</h1>

                <img src="/assets/about/facemask-map.PNG"/>
            </div>
        </section>

        <!-- Download app icons -->
        <div class="download flex jc pt3">
            <img
                src="/assets/icons/ios.png"
                class="app-icon"
                style="margin-right: 1em;"
                @click="ios"
            />
            <img
                src="/assets/icons/android.png"
                class="app-icon"
                @click="android"
            />
        </div>


        <!-- The illusion of urban cleaning -->

        <div class="hero-body">
            <div class="container">
                <h1 class="title is-1">
                    {{ $t('home.about.about12') }}
                    {{ $t('home.about.about13') }}
                    {{ $t('home.about.about31') }}
                </h1>
            </div>
        </div>

        <!-- More info -->
        <div class="hero-body">
            <div class="container">
                <div class="tile is-ancestor">
                    <div class="tile is-vertical is-8">
                        <div class="tile">
                            <div class="tile is-parent is-vertical">
                                <article class="tile is-child notification is-primary">
                                    <p style="color: black;" class="title">{{ $t('home.about.about14') }} <b
                                        style="color: white;">{{ $t('home.about.about14a') }}</b></p>
                                    <p class="title" style="padding-bottom: 1em;">{{ $t('home.about.about14b') }}</p>
                                    <p class="subtitle" style="text-align: right; color: red;"><strong>{{
                                        $t('home.about.about15') }}</strong></p>
                                </article>
                                <article class="tile is-child notification is-warning">
                                    <p class="title" style="padding-bottom: 1em;">{{ $t('home.about.about16') }}</p>
                                    <p class="subtitle" style="text-align: right; color: red; padding-bottom: 1em;"><b>{{
                                        $t('home.about.about17') }}</b></p>
                                </article>
                            </div>
                            <div class="tile is-parent">
                                <article class="tile is-child notification is-info">
                                    <p class="title">{{ $t('home.about.about17a') }}</p>
                                    <p class="subtitle">{{ $t('home.about.about17b') }}</p>
                                    <!-- <figure class="image is-4by3"> -->
                                    <a href="https://openlittermap.com/maps/The%20Netherlands/Zuid-Holland/Wassenaar/map">https://openlittermap.com/maps/The%20Netherlands/Zuid-Holland/Wassenaar/map</a>
                                    <br>
                                    <br>
                                    <img src="/assets/nlbrands.png">
                                    <!-- </figure> -->
                                    <br>
                                    <br>
                                    <p class="subtitle">{{ $t('home.about.about17c') }}</p>
                                    <a href="https://openlittermap.com/maps/The%20Netherlands/Zuid-Holland/Wassenaar/download">https://openlittermap.com/maps/The%20Netherlands/Zuid-Holland/Wassenaar/download</a>
                                    <br>
                                </article>
                            </div>
                        </div>
                        <div class="tile is-parent">
                            <article class="tile is-child notification is-danger">
                                <p class="title">{{ $t('home.about.about18') }}</p>
                                <p class="subtitle">{{ $t('home.about.about19') }}<strong>{{ $t('home.about.about20')
                                    }}</strong> {{ $t('home.about.about21') }}</p>
                                <div class="content">
                                    <!-- Content -->
                                </div>
                            </article>
                        </div>
                    </div>
                    <div class="tile is-parent is-5">
                        <article class="tile is-child is-10 notification is-success">
                            <div class="content">
                                <p class="title">{{ $t('home.about.about22') }}</p>
                                <div class="content">
                                    <ul class="list">
                                        <li>{{ $t('home.about.about24') }}</li>
                                        <li>{{ $t('home.about.about25') }}</li>
                                        <li>{{ $t('home.about.about26') }}</li>
                                        <li>{{ $t('home.about.about27') }}</li>
                                        <li>{{ $t('home.about.about28') }}</li>
                                        <li>{{ $t('home.about.about29') }}</li>
                                        <li>{{ $t('home.about.about29a') }}</li>
                                    </ul>
                                </div>
                            </div>
                        </article>
                    </div>
                </div>
            </div>
        </div>

        <div class="container">
            <h1 class="title is-1 has-text-left">
                {{ $t('home.about.about33') }}
            </h1>
        </div>
        <br>
        <br>
        <div class="container">
            <h1 class="title is-1 has-text-left">
                {{ $t('home.about.about34') }}
            </h1>
            <br>
            <div class="has-text-centered" style="padding-top: 2em;">
                <form action="/signup">
                    <button class="btn btn--green btn--animated">{{ $t('home.about.about35') }}</button>
                </form>
            </div>
            <br>
            <br>
        </div>

        <footer class="footer">
            <div class="container">
                <div class="content has-text-centered">
                    <div class="info">
                        OpenLitterMap by <a href="https://ie.linkedin.com/in/seanlynchgis">Seán Lynch, M.Sc, M.Sc.,
                        B.A.</a>
                    </div>
                    <br>
                    <div class="info">info@openlittermap.com</div>
                </div>
            </div>
        </footer>








        <!-- Cigarette Butts -->
        <section style="margin-top: 1000px" class="section">
            <div class="columns">
                <div class="column is-one-third is-offset-1" style="text-align: center;">
                    <img src="/assets/butts.jpg"/>
                </div>

                <div class="column cig-2">
                    <h2 id="butts1txt" class="title is-2" style="color: red; text-align: center;">
                        <strong>{{ $t('home.about.about2') }}</strong>
                    </h2>
                </div>
            </div>
            <br>
            <br>
            <div class="columns">
                <div class="column is-one-third is-offset-1">
                    <h1 class="title is-1" style="text-align: center;"><strong>{{ $t('home.about.about3') }}</strong>
                    </h1>
                    <br>
                    <h1 class="subtitle is-3">{{ $t('home.about.about4') }}</h1>
                    <br>
                    <h1 class="subtitle is-3">{{ $t('home.about.about5') }}</h1>
                    <br>
                    <p class="subtitle is-3">{{ $t('home.about.about6') }}</p>
                </div>

                <div class="column is-offset-1 butts-img">
                    <img src="/assets/cigbutts_jar.jpg" style="height: 600px;">
                </div>
            </div>
        </section>

        <!-- Call to action -->
        <section class="hero is-success">
            <div class="hero-body">
                <div class="container has-text-centered">
                    <h1 class="title">
                        <strong>
                            {{ $t('home.about.about7') }}
                        </strong>
                    </h1>
                    <!-- subtitle removed -->
                </div>
                <div class="has-text-centered" style="padding-top: 2em;">
                    <router-link to="/signup">
                        <button class="button is-large is-info hov">{{ $t('home.about.about9') }}</button>
                    </router-link>
                </div>
            </div>
        </section>

        <!-- 1. Just take a photo -->
        <div class="has-text-centered pt3">
            <h1 class="title is-1">1. {{ $t('home.about.about9a') }}</h1>

            <img src="/assets/about/iphone.PNG"/>
        </div>

        <!-- 2. Tag it with our app -->
        <div class="has-text-centered pt3">
            <h1 class="title is-1">2. {{ $t('home.about.about9b') }}</h1>

            <img src="/assets/about/facemask-tag.PNG"/>
        </div>

        <!-- 3. Upload it -->
        <div class="has-text-centered pt3">
            <h1 class="title is-1">3. {{ $t('home.about.about9c') }}</h1>

            <img src="/assets/about/facemask-map.PNG"/>
        </div>

        <!-- Download app icons -->
        <div class="flex jc pt3">
            <img
                src="/assets/icons/ios.png"
                class="app-icon"
                style="margin-right: 1em;"
                @click="ios"
            />
            <img
                src="/assets/icons/android.png"
                class="app-icon"
                @click="android"
            />
        </div>

        <!-- Plastic from land to sea -->
        <section>
            <div class="columns" style="padding-top: 4em; padding-bottom: 4em;">
                <div class="column is-one-third is-offset-1" style="padding-left: 2em; margin:auto;">
                    <h1 class="title is-2" style="text-align: center;"><strong style="color: red;">{{
                        $t('home.about.about10') }}</strong></h1>
                    <br>
                    <h1 class="title is-2" style="text-align: center;"><strong style="color: red;">{{
                        $t('home.about.about11') }}</strong></h1>
                </div>

                <div class="column is-one-third is-offset-1"
                     style="padding-top: 4em; padding-bottom: 4em; margin:auto;">
                    <img src="/assets/plastic_bottles.jpg" style="">
                </div>
            </div>
        </section>

        <!-- The illusion of urban cleaning -->
        <section class="hero is-warning">
            <div class="hero-body">
                <div class="container">
                    <h1 class="title is-1">
                        {{ $t('home.about.about12') }}
                    </h1>

                    <img src="/assets/cigbutts.jpg">

                    <h1 class="title is-1 has-text-right">
                        {{ $t('home.about.about13') }}
                    </h1>
                </div>
            </div>
        </section>

        <!-- More info -->
        <div class="hero-body">
            <div class="container">
                <div class="tile is-ancestor">
                    <div class="tile is-vertical is-8">
                        <div class="tile">
                            <div class="tile is-parent is-vertical">
                                <article class="tile is-child notification is-primary">
                                    <p class="title">{{ $t('home.about.about14') }} <b style="color: black;">{{
                                        $t('home.about.about14a') }}</b></p>
                                    <p class="title" style="padding-bottom: 1em;">{{ $t('home.about.about14b') }}</p>
                                    <p class="subtitle" style="text-align: right; color: red;"><strong>{{
                                        $t('home.about.about15') }}</strong></p>
                                </article>
                                <article class="tile is-child notification is-warning">
                                    <p class="title" style="padding-bottom: 1em;">{{ $t('home.about.about16') }}</p>
                                    <p class="subtitle" style="text-align: right; color: red; padding-bottom: 1em;"><b>{{
                                        $t('home.about.about17') }}</b></p>
                                </article>
                            </div>
                            <div class="tile is-parent">
                                <article class="tile is-child notification is-info">
                                    <p class="title">{{ $t('home.about.about17a') }}</p>
                                    <p class="subtitle">{{ $t('home.about.about17b') }}</p>
                                    <!-- <figure class="image is-4by3"> -->
                                    <a href="https://openlittermap.com/maps/The%20Netherlands/Zuid-Holland/Wassenaar/map">https://openlittermap.com/maps/The%20Netherlands/Zuid-Holland/Wassenaar/map</a>
                                    <br>
                                    <br>
                                    <img src="/assets/nlbrands.png">
                                    <!-- </figure> -->
                                    <br>
                                    <br>
                                    <p class="subtitle">{{ $t('home.about.about17c') }}</p>
                                    <a href="https://openlittermap.com/maps/The%20Netherlands/Zuid-Holland/Wassenaar/download">https://openlittermap.com/maps/The%20Netherlands/Zuid-Holland/Wassenaar/download</a>
                                    <br>
                                </article>
                            </div>
                        </div>
                        <div class="tile is-parent">
                            <article class="tile is-child notification is-danger">
                                <p class="title">{{ $t('home.about.about18') }}</p>
                                <p class="subtitle">{{ $t('home.about.about19') }}<strong>{{ $t('home.about.about20')
                                    }}</strong> {{ $t('home.about.about21') }}</p>
                                <div class="content">
                                    <!-- Content -->
                                </div>
                            </article>
                        </div>
                    </div>
                    <div class="tile is-parent is-5">
                        <article class="tile is-child is-10 notification is-success">
                            <div class="content">
                                <p class="title">{{ $t('home.about.about22') }}</p>
                                <div class="content">
                                    <ul>
                                        <li>{{ $t('home.about.about24') }}</li>
                                        <li>{{ $t('home.about.about25') }}</li>
                                        <li>{{ $t('home.about.about26') }}</li>
                                        <li>{{ $t('home.about.about27') }}</li>
                                        <li>{{ $t('home.about.about28') }}</li>
                                        <li>{{ $t('home.about.about29') }}</li>
                                        <li>{{ $t('home.about.about29a') }}</li>
                                    </ul>
                                </div>
                            </div>
                        </article>
                    </div>
                </div>
            </div>
        </div>

        <div>
            <br>
            <h1 class="title is-1" style="color: black; text-align: center;"><strong>{{ $t('home.about.about30')
                }}</strong> <strong style="color: red;">{{ $t('home.about.about301') }}</strong></h1>
            <br>
        </div>

        <div class="container" style="padding-bottom:5em; text-align: center;">
            <img src="/assets/marinelitter.jpg"/>
            <p style="padding-bottom: 3em;">Dublin, Ireland.</p>
            <h1 class="title is-1" style="color: black; text-align: center;">
                <strong style="color: red;">{{ $t('home.about.about302') }}</strong>
            </h1>
            <img src="/assets/microplastics_oranmore.JPG"/>
            <p>Microplastics in Oranmore, Co. Galway.</p>
        </div>

        <div class="container">
            <h1 class="title is-1">
                {{ $t('home.about.about31') }}
            </h1>
            <br>
            <br>
        </div>

        <img src="/assets/urban.JPG" style="padding-bottom: 1em;">
        <p style="padding-bottom: 5em; text-align: center;">Penrose Wharf, Cork City, Ireland (above)</p>

        <div style="text-align: center;">
            <img src="/assets/IMG_0554.JPG" style="padding-bottom: 2em;">
            <p style="padding-bottom: 5em; text-align: center;">Accra, Capital of Ghana, North-Western Coast of Africa
                <a href="https://www.facebook.com/nshorena/posts/1652239435009949">more photos on facebook</a></p>
            <img src="/assets/IMG_0556.JPG" style="padding-bottom: 2em;">
            <p style="padding-bottom: 5em;">{{ $t('home.about.about32') }}</p>
        </div>

        <div class="container">
            <h1 class="title is-1 has-text-left">
                {{ $t('home.about.about33') }}
            </h1>
        </div>
        <br>
        <br>
        <div class="container">
            <h1 class="title is-1 has-text-left">
                {{ $t('home.about.about34') }}
            </h1>
            <br>
            <div class="has-text-centered" style="padding-top: 2em;">
                <form action="/signup">
                    <button class="button is-large is-primary hov">{{ $t('home.about.about35') }}</button>
                </form>
            </div>
            <br>
            <br>
        </div>

        <footer class="footer">
            <div class="container">

                <div class="content has-text-centered">
                    <p>
                        <strong>OpenLitterMap</strong> by <a href="https://ie.linkedin.com/in/seanlynchgis">Seán Lynch,
                        M.Sc, M.Sc., B.A.</a>
                        <br>
                    <p>info@openlittermap.com</p>
                </div>
            </div>
        </footer>
    </div>
</template>

<script>
export default {
    name: 'About',
    methods: {
        /**
         * Open Google Play store download page
         */
        android() {
            window.open('https://play.google.com/store/apps/details?id=com.geotech.openlittermap', '_blank');
        },

        /**
         * Open App Store download page
         */
        ios() {
            window.open('https://apps.apple.com/us/app/openlittermap/id1475982147', '_blank');
        }
    }
}
</script>

<style scoped>

.section__1 {
    height: 95vh;
    background-image: url("/assets/IMG_0001.PNG");
    background-size: cover;
    background-position: top;
    position: relative;
}

.section__1--title {
    font-size: 50px;
    font-weight: 700;
    line-height: 1.5rem;
    letter-spacing: 0.1em;
    position: absolute;
    top: 20%;
    left: 50%;
    transform: translate(-50%, -50%);
    text-align: center;
}

.section__1--title1 {
    font-size: 50px;
    font-weight: 700;
    color: white;
}

.section__1--text {
    font-size: 24px;
    font-weight: 400;
    position: absolute;
    top: 30%;
    left: 50%;
    transform: translate(-50%, -50%);
    text-align: center;
}

.section-about {
    background-color: #f7f7f7;
    padding: 10rem 8rem 15rem;
}

.paragraph {
    font-size: 1.5rem;
    font-weight: 400;
    line-height: 1.7;
    color: #777;
    margin-bottom: 1.5rem;
}

.paragraph-bold {
    font-size: 2rem;
    font-weight: 600;
    color: #777;

}

.row {
    max-width: 114rem;
    margin: 0 auto;
}

.row:not(:last-child) {
    margin-bottom: 8rem;
}

.row::after {
    content: "";
    display: table;
    clear: both;
}

.row [class^="col-"] {
    float: left;
}

.row [class^="col-"]:not(:last-child) {
    margin-right: 6rem;
}

.row .col-1-of-2 {
    width: calc((100% - 6rem) / 2);
}


.composition {
    position: relative;
}

.composition__photo {
    width: 70%;
    box-shadow: 0 1.5rem 4rem rgba(0, 0, 0, 0.4);
    position: absolute;
    z-index: 10;
    transition: all .2s;
    outline-offset: 2rem;
}

@media (max-width: 56.25em) {
    .composition__photo {
        float: left;
        position: relative;
        width: 33.3333%;
        box-shadow: 0 1.5rem 3rem rgba(0, 0, 0, 0.2);
    }
}

.composition__photo--p1 {
    left: 0;
    top: -3rem;
}

@media (max-width: 56.25em) {
    .composition__photo--p1 {
        top: 0;
        transform: scale(1.2);
    }
}

.composition__photo--p2 {
    right: -3rem;
    top: 4rem;
}

@media (max-width: 56.25em) {
    .composition__photo--p2 {
        top: -1rem;
        transform: scale(1.3);
        z-index: 100;
    }
}

.composition__photo--p3 {
    left: 20%;
    top: 13rem;
}

@media (max-width: 56.25em) {
    .composition__photo--p3 {
        top: 1rem;
        left: 0;
        transform: scale(1.1);
    }
}

.composition__photo:hover {
    outline: 1.5rem solid #55c57a;
    transform: scale(1.05) translateY(-0.5rem);
    box-shadow: 0 2.5rem 4rem rgba(0, 0, 0, 0.5);
    z-index: 20;
}

.composition:hover .composition__photo:not(:hover) {
    transform: scale(0.95);
}

.hero {
    background-image: linear-gradient(to right bottom, rgba(126, 213, 111, 0.8), rgba(40, 180, 133, 0.8));
}

.btn, .btn:link, .btn:visited {
    text-decoration: none;
    padding: 1rem 3rem;
    display: inline-block;
    border-radius: 11rem;
    transition: all .2s;
    position: relative;
    font-size: 1.3rem;
    border: none;
    cursor: pointer;
}

.btn:hover {
    transform: translateY(-3px);
    box-shadow: 0 1rem 2rem rgba(0, 0, 0, 0.2);
}

.btn:hover::after {
    transform: scaleX(1.5) scaleY(1.6);
    opacity: 0;
}

.btn:active .btn:focus {
    outline: none;
    transform: translateY(-1px);
    box-shadow: 0 0.5rem 1rem rgba(0, 0, 0, 0.2);
}

.btn--white {
    background-color: #fff;
    color: #777;
}

.btn--white::after {
    background-color: #fff;
}

.btn--green {
    background-color: #55c57a;
    color: #fff;
}

.btn--green::after {
    background-color: #55c57a;
}

.btn::after {
    content: "";
    display: inline-block;
    height: 100%;
    width: 100%;
    border-radius: 10rem;
    position: absolute;
    top: 0;
    left: 0;
    z-index: -1;
    transition: all .4s;
}

.btn--animated {
    animation: moveInBottom .5s ease-out .75s;
    animation-fill-mode: backwards;
}

.take__action {
    display: flex;
    margin: 100px auto 50px;
}

.take__action-1 {
    flex: 1;
}

.take__action-1 img {
    max-width: 400px;
    box-shadow: 0 1.5rem 4rem rgb(0 0 0 / 40%);
}

.title {
    font-size: 45px;
    color: #4a4a4a;
    margin-bottom: 50px;
    text-shadow: 0 1.5rem 4rem rgb(0 0 0 / 10%);
}

.download {
    margin-bottom: 30px;
}

.list {
    font-size: 25px;
}

li {
    margin-bottom: 30px;
}

.footer {
    background-color: #333;
}

.info {
    color: #fff;
}





.butts-img {
    text-align: center;
    padding-right: 5em;
}

.cig-2 {
    align-items: center;
    display: flex;
    padding: 5em;
}

@media screen and (max-width: 768px) {
    .butts-img {
        padding-right: 0;
    }

    .cig-2 {
        padding: 1em;
    }
}
</style>
