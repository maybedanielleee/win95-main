<template>
<div>
    <img class="self" src="@/assets/Biography/danielleHeadshot.jpg" />
    <h2 class="header">Danielle Chaffin</h2>
    <h4 class="subtitle" style="padding-bottom: 10px">
        Solutions Engineer | 3rd Generation in Logistics | Occasional Pot Stirrer
    </h4>
    <h4 class="subtitle">Tennessee📍</h4>
    <div class="badge-grid">
        <img class="badge" alt="Swift" src="https://img.shields.io/badge/-Swift-orange" />
        <img class="badge" alt="Python" src="https://img.shields.io/badge/-Python-blue" />
        <img class="badge" alt="JavaScript" src="https://img.shields.io/badge/-Javascript-yellow" />
        <img class="badge" alt="SQL" src="https://img.shields.io/badge/-SQL-lightgrey" />
        <img class="badge" alt="Git" src="https://img.shields.io/badge/-Git-critical" />
        <img class="badge" alt="HTML/CSS" src="https://img.shields.io/badge/-HTML%2FCSS-yellowgreen" />
        <img class="badge" alt="SwiftUI" src="https://img.shields.io/badge/-SwiftUI-3e8bc3" />
        <img class="badge" alt="React Native" src="https://img.shields.io/badge/-React Native-blue" />
        <img class="badge" alt="Vue" src="https://img.shields.io/badge/-VueJS-61b083" />
        <img class="badge" alt="Flask" src="https://img.shields.io/badge/-Flask-406893" />
        <img class="badge" alt="MongoDB" src="https://img.shields.io/badge/-MongoDB-4ca158" />
        <img class="badge" alt="SQLite" src="https://img.shields.io/badge/-SQLite-64a2c9" />
        <img class="badge" alt="Figma" src="https://img.shields.io/badge/-Figma-8c5aee" />
    </div>
    <div class="inner-content">
        <h3 class="heading"><b>About Me</b></h3>
        <p class="paragraph">
            Hello. Hi. Welcome! My name is Danielle Chaffin and I'm Revenova's Solutions Engineer. 
            at Ministry of Defence Singapore, working on exciting projects with React Native and Vue3.
        </p>
        <p class="paragraph">
            Danielle comes from a family that has been in trucking for three
            generations. She loves thinking ahead and finding new, creative
            ideas. Danielle really wants to help people do well. She's good at
            solving tricky problems and making things better with her clever
            ideas. Plus, Danielle knows all about using Salesforce to make
            businesses work better. She's always learning more to keep things
            moving forward!
            <br>
            Danielle wrote this in third-person.
        </p>
    </div>
        <p class="paragraph">
            Check out my YouTube channel
            <a style="color: #ff5733" href="https://www.youtube.com/@maybedanielleee">here</a>!
        </p>
        <p class="paragraph">
            And request a Revenova demo
            <a style="color: #ff5733" href="https://revenova.com/request-a-demo/">here</a>!
        </p>
    </div>

    <!-- <div class="inner-content">
                            <div class="heading"><b>Interests and Hobbies</b></div>
                            <div class="paragraph">Analog photography and colorizing of historical photos have always interested me and some of my photographic works are displayed <span style="cursor: pointer; color: #FF5733;" v-on:click="showPhotos">here</span> while you can find my colorization portfolio <span style="cursor: pointer; color: #FF5733;" v-on:click="showColorization">here</span>.</div>
                        </div> -->
</template>

<style scoped>
.badge-grid {
    display: table;
    align-items: center;
    margin-top: 20px;
}

.badge {
    width: auto;
    height: 20px;
    border-radius: 0px;
    font-size: 12px;
    padding-right: 10px;
    /* box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.12), 0 6px 20px 0 rgba(0, 0, 0, 0.1); */
}

.self {
    width: 100%;
    height: auto;
    /* border-radius: 5px; */
}

.subtitle {
    font-size: 12px;
    color: gray;
}

.heading {
    padding-bottom: 5px;
}

.header {
    padding-top: 20px;
    padding-bottom: 20px;
}

.inner-content {
    padding-top: 30px;
}

h2,
h4,
h3 {
    padding: 0;
    margin: 0;
}
</style>
