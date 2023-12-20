<script lang="ts">
    import me from "../images/IMG_3126.jpg"
    import cat from "../images/cat1.gif"
    import game from "../images/game.png"

    
</script>

<div class="background-image">
    <!--About Me-->
    <div class="about-me-card common-outer-style">
        <div class="dan-pic">
        <img
        src = {me}
        class = "me"
        alt = "young man"
        >
        </div>

        <div class="about-me-text common-inner-style">
            <h1><b>About Me</b></h1>
            <p>Hi! I'm Daniel, an undergrad at Northeastern University majoring in Computer Science and Math!
                I'm currently interested in algorithms, machine learning, and full-stack development.
                In my free time, I enjoy reading, weightlifting, and exploring.
                You can reach me at ma.daniel004@gmail.com.
            </p>
        </div>

    </div>

    <!--Recent Work-->
    <div class="recent-work-card common-outer-style">

        <div class="recent-work-text common-inner-style">
            <h1>Recent Work</h1>
            <p>I recently finished my first semester in college, where I completed a plethora of projects, including: </p>
                <ul class="list">
                    <li>A binary square game in Python</li>
                    <li>A fun visual pipe game in Racket</li>
                    <li>A Leetcode to VSCode port with Typescript</li>
                    <li>and many more!</li>
                </ul>
            <p>Check them all out at my Github!</p>
        </div>
        <div class="recent-work-image">
            <img
            src = {game}
            class = "proj"
            alt = "project pictures"
            >
        </div>
    </div>

    <!--Contact-->
    <div class="contact-card common-outer-style">
        <div class="cat">
            <img
            src = {cat}
            class = "cat"
            alt = "shh.. the cat is sleeping"
            >
        </div>
        
        <div class="contact-text common-inner-style">
            <h1>Contact</h1>
            <p>Take a look at my projects or connect with me here.</p>
            <div class="links">
                <a href="https://github.com/danielma4" target="_blank">
                    <svg xmlns="http://www.w3.org/2000/svg" width="50" height="50" viewBox="0 0 24 24">
                        <path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/></svg>
                </a>
                <a href="https://www.linkedin.com/in/daniel-ma-765a32277/" target="_blank">
                    <svg xmlns="http://www.w3.org/2000/svg" width="50" height="50" viewBox="0 0 24 24">
                        <path d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.764s.784-1.764 1.75-1.764 1.75.79 1.75 1.764-.783 1.764-1.75 1.764zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z"/></svg>
                </a>
            </div>
        </div>
    </div>
</div>


<style lang="css">
    p {
        font-family: "Work Sans";
        font-size: 20px;
    }
    h1 {
        font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
        color: black;
        font-size: 30px;
    }
    .dan-pic img {
        height: 260px;
        width: 180px;
    }
    .background-image {
        flex-direction: column;
        background-image: url("../images/boston2.jpg");
        background-size: cover;
        background-repeat: no-repeat;
        background-position: center;
        height: 100vh;
        width: 100vw;
        overflow: hidden;
    }
    .common-outer-style {
        background-color: rgba(255, 255, 255, 0.8);
        display: flex;
        justify-content: center;
        align-items: center;
        height: 30vh;
        width: 100vw;
        border-radius: 15px;
    }
    .common-inner-style {
        width: 30%;
        padding: 20px;
        text-align: center;
        font-family: sans-serif;
    }
    .about-me-card {
        margin-bottom: 40px;
    }
    .about-me-text {
        line-height: 2;
    }
    .recent-work-card {
        margin-bottom: 40px;
    }
    .contact-text {
        width: 25%;
    }
    .list {
        list-style: none;
        padding: 0;
    }
    .list li {
        margin: 8px 0;
        font-family: Georgia, 'Times New Roman', Times, serif;
        font-size: 20px;
    }
    .cat {
        width:100px;
        height: 100px;
    }

    @media screen and (max-width: 1200px) {
        .common-inner-style {
            padding: 10px;
            width: 60%;
        }
        .dan-pic img, .recent-work-image img {
            max-width: 40%;
            height: auto;
        }
        .about-me-card, .recent-work-card {
            margin: 20px auto;
        }
        h1 {
            font-size: 25px;
        }
        .common-inner-style p {
            font-size: 12px;
        }
        .list li {
            font-size: 12px;
        }
    }
    @media screen and (max-width: 450px) {
        .common-inner-style {
            padding: 10px;
            width: 80%;
        }
        .dan-pic img, .recent-work-image img {
            max-width: 50%;
            height: auto;
        }
        .about-me-card, .recent-work-card {
            margin: 20px auto;
        }
        h1 {
            font-size: medium;
        }
        .common-inner-style p {
            font-size: small;
            padding: 10px 0;
        }
        .list li {
            font-size: small;
        }
    }
</style>