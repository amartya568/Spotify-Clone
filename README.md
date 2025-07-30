# Spotify-Clone

# HTML codes:- 
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Spotify - Web Player: Music for everyone</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" href="utility.css">
</head>

<body>
    <div class="container flex bg-black">
        <div class="left">
            <div class="close">
                <img width="30" class="invert" src="img/close.svg" alt="">
            </div>
            <div class="home bg-grey rounded m-1 p-1">
                <div class="logo"><img width="110" class="invert" src="img/logo.svg" alt=""></div>
                <ul>
                    <li><img class="invert" src="img/home.svg" alt="home">Home</li>
                    <li><img class="invert" src="img/search.svg" alt="search">Search</li>
                </ul>
            </div>
            <div class="library bg-grey rounded m-1 p-1">
                <div class="heading">
                    <img class="invert" src="img/playlist.svg" alt="">
                    <h2>
                        Your Library
                    </h2>
                </div>
                <div class="songlist">
                    <ul>
                    </ul>
                </div>
                <div class="footer">
                    <div><a href="https://www.spotify.com/jp/legal/"><span>Legal</span></a></div>
                    <div><a href="https://www.spotify.com/jp/privacy/"><span>Privacy Center</span></a></div>
                    <div><a href="https://www.spotify.com/jp/legal/privacy-policy/"><span>Privacy Policy</span></a>
                    </div>
                    <div><a href="https://www.spotify.com/jp/legal/cookies-policy/"><span>Cookies</span></a></div>
                    <div><a href="https://www.spotify.com/jp/legal/privacy-policy/#s3"><span>About Ads</span></a></div>
                    <div><a href="https://www.spotify.com/jp/accessibility/"><span>Accessibility</span></a></div>
                </div>
            </div>
        </div>
        <div class="right bg-grey rounded">
            <div class="header">
                <div class="nav">
                    <div class="hamburgerContainer">
                        <img width="40" class="invert hamburger" src="img/hamburger.svg" alt="">
                        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path
                                d="M15 6L9.70711 11.2929C9.37377 11.6262 9.20711 11.7929 9.20711 12C9.20711 12.2071 9.37377 12.3738 9.70711 12.7071L15 18"
                                stroke="#ffffff" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                        </svg>
                        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                            <path
                                d="M9 18L14.2929 12.7071C14.6262 12.3738 14.7929 12.2071 14.7929 12C14.7929 11.7929 14.6262 11.6262 14.2929 11.2929L9 6"
                                stroke="#ffffff" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                        </svg>
                    </div>
                </div>
                <div class="buttons">
                    <button class="signupbtn">Sign up</button>
                    <button class="loginbtn">Log in</button>
                </div>
            </div>
            <div class="SpotifyPlaylists">
                <h1>Spotify Playlists</h1>
                <div class="cardContainer"> </div>
                <div class="playbar">
                    <div class="seekbar">
                        <div class="circle">
                        </div>
                    </div>
                    <div class="abovebar">
                        <div class="songinfo">
                        </div>
                        <div class="songbuttons">
                            <img width="35" id="previous" src="img/prevsong.svg" alt="">
                            <img width="35" id="play" src="img/play.svg" alt="">
                            <img width="35" id="next" src="img/nextsong.svg" alt="">
                        </div>
                        <div class="timevol">
                            <div class="songtime">
                            </div>
                            <div class="volume">
                                <img width="25" src="img/volume.svg" alt="">
                                <div class="range">
                                    <input type="range" name="volume" id=""> 
                                </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <script src="script.js"></script>
</body>
</html>

# CSS codes :-
# 1. style.css :
@import url('https://fonts.googleapis.com/css2?family=Lato:wght@700&family=Roboto:ital,wght@0,100;0,300;0,400;0,500;0,700;0,900;1,100;1,300;1,400;1,500;1,700;1,900&display=swap');

:root{
    --a:0;
}

* {
    margin: 0px;
    padding: 0px;
    font-family: 'Roboto', sans-serif;
}

.close {
    display: none;
}

body {
    background-color: black;
    color: white;
}

.left {
    width: 25vw;
    padding: 10px;
}

.right {
    width: 75vw;
}

/* .home {} */

.home ul li {
    width: 14px;
    display: flex;
    list-style: none;
    gap: 15px;
    padding-top: 14px;
    font-weight: bold;

}

.heading {
    width: 100%;
    display: flex;
    gap: 15px;
    padding-top: 14px;
    padding: 23px 14px;
    font-weight: bold;
    align-items: center;
    font-size: 13px;
}

.heading img {
    width: 20px;
}

.library {
    min-height: 90vh;
    position: relative;
}

.footer {
    display: flex;
    font-size: 9.2px;
    color: grey;
    gap: 13px;
    position: absolute;
    bottom: 0;
    padding: 10px 0;
}

.footer a {
    color: grey;
}

.right {
    margin: 16px 0;
    position: relative;
}

.header {
    display: flex;
    justify-content: space-between;
    background-color: rgb(34, 34, 34);
}

.header>* {
    padding: 20px;
}

.bg-black {
    background-color: black;
    color: white;
}

.SpotifyPlaylists {
    padding: 16px;
}

.SpotifyPlaylists h1 {
    padding: 16px;
}

.cardContainer {
    margin: 30px;
    display: flex;
    gap: 10px;
    flex-wrap: wrap;
    overflow-y: auto;
    max-height: 60vh;
}

.card {
    width: 200px;
    padding: 10px;
    border-radius: 5px;
    background-color: #252525;
    position: relative;
    transition: all .9s;
}

.card:hover{
    background-color: rgb(105, 103, 103);
    cursor: pointer;
    --a: 1;
}

.card>* {
    padding-top: 10px;
}

.card img {
    width: 100%;
    object-fit: contain;
    border-radius: 5px;
}

.play {
    width: 48px;
    height: 48px;
    border-radius: 50%;
    background-color: #1fdf64;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 6px;
    box-sizing: border-box;
    position: absolute;
    top: 168px;
    right: 17px;
    opacity: var(--a);
    transition: all 1s ease-out;
}

.buttons>* {
    margin: 0 12px;
}

.signupbtn {
    background-color: rgb(34, 34, 34);
    color: rgb(156, 148, 148);
    font-weight: bold;
    border: none;
    outline: none;
    cursor: pointer;
    font-size: 16px;
}

.signupbtn:hover {
    font-size: 1.01rem;
    color: white;
}

.loginbtn {
    background-color: white;
    border-radius: 21px;
    padding: 10px;
    color: black;
    font-weight: bold;
    width: 79px;
    cursor: pointer;
    font-size: 16px;
}

.loginbtn:hover {
    font-weight: bold;
    font-size: 17px;
}

.playbar {
    position: fixed;
    bottom: 30px;
    filter: invert(1);
    background: #dad5d5;
    border-radius: 10px;
    width: 90%;
    min-height: 40px;
    padding: 12px;
    width: 70vw;
}

.songbuttons {
    display: flex;
    justify-content: center;
    gap: 16px;
}

.songlist ul {
    padding: 0 12px;
}

.songlist ul li {
    list-style-type: decimal;
    display: flex;
    gap: 12px;
    cursor: pointer;
    padding: 12px 0;
    border: 1px solid white;
    margin: 12px 0;
    padding: 8px;
    border-radius: 5px;
    justify-content: space-between;
}

.songlist {
    height: 544px;
    margin-bottom: 44px;
    overflow: auto;
}

.hamburger {
    display: none;
    cursor: pointer;
}

.hamburgerContainer {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 14px;
}

.info div {
    word-break: break-all;
}

.songlist .info {
    font-size: 13px;
    width: 344px;
}

.playnow {
    display: flex;
    justify-content: center;
    align-items: center;

}

.playnow span {
    font-size: 15px;
    width: 64px;
    padding: 12px;
}

.seekbar {
    height: 4px;
    width: 100%;
    background: black;
    border-radius: 10px;
    position: absolute;
    bottom: -5%;
    margin: 6px;
    left: 0%;
    cursor: pointer;
}

.circle {
    width: 13px;
    height: 13px;
    border-radius: 13px;
    background-color: black;
    position: relative;
    bottom: 6px;
    left: 0%;
    transition: left 0.5s;
}

.songbuttons img {
    cursor: pointer;
}

.timevol {
    display: flex;
    justify-content: space-evenly;
    align-items: center;
}

.songinfo {
    color: black;
    padding: 0 12px;
    width: 250px;
}

.songtime {
    width: 125px;
    color: black;
    padding: 0 12px;
}

.volume {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 12px;
    cursor: pointer;
}

.range input{
    cursor: pointer;
}

.abovebar {
    display: flex;
    justify-content: space-between;
    margin: 20px 0;
}

@media (max-width: 1200px) {
    .left {
        position: absolute;
        left: -120%;
        transition: all .3s;
        z-index: 1;
        width: 373px;
        background-color: black;
        padding: 0;
    }
    .songinfo,
    .songtime {
        width: auto;
    }
    .left .close {
        position: absolute;
        right: 31px;
        top: 25px;
        width: 29px;
    }
    .timevol {
        display: flex;
        justify-content: space-evenly;
        align-items: center;
        flex-direction: column;
        gap: 13px;
    }
    .right {
        width: 100vw;
    }
    .playbar {
        width: calc(100vw - 75px);
    }
    .seekbar {
        width: calc(100vw - 120px);
    }
    .hamburger {
        display: block;
    }
    .right {
        margin: 0;
    }
    .card {
        width: 44vw;
    }
    .cardContainer {
        margin: 0;
        justify-content: center;
    }
    .close {
        display: block;
    }
    .abovebar {
        flex-direction: column;
        gap: 23px;
        align-items: center;
    }

}

@media (max-width: 400px) {
    .card{
        width: 84vw;
    }
    .header>* {
        margin: 0 6px;
    }
    .buttons>*{
        margin: 0 6px;
    }
}

# 2. Utility.css :
.border{
    border: 2px solid red;
    margin: 3px;
}

.flex{
    display: flex;
}

.justify-center{
    justify-content: center;
}

.item-center{
    align-items: center;
}

.invert{
    filter: invert(1);
}

.bg-grey{
    background-color: #121212;
}

.rounded{
    border-radius: 7px;
}

.m-1{
    margin: 5px;
}

.p-1{
    padding: 10px;
}


/* For WebKit browsers */
::-webkit-scrollbar {
  width: 10px;
  height: 10px;
}

::-webkit-scrollbar-track {
  background: #1e1e1e;  /* Dark background */
}

::-webkit-scrollbar-thumb {
  background: #555;      /* Darker thumb */
  border-radius: 5px;
}

::-webkit-scrollbar-thumb:hover {
  background: #888;      /* Lighter on hover */
}

/* For Firefox */
* {
  scrollbar-width: thin;
  scrollbar-color: #555 #1e1e1e;
}


# Java Script codes :-
console.log("Lets write the Java Script...")
let currentSong = new Audio();
let songs;
let currFolder;

function secondsToMinutesSeconds(seconds) {
    if (isNaN(seconds) || seconds < 0) {
        return "00:00";
    }
    const minutes = Math.floor(seconds / 60);
    const remainingSeconds = Math.floor(seconds % 60);
    const formattedMinutes = String(minutes).padStart(2, '0');
    const formattedSeconds = String(remainingSeconds).padStart(2, '0');
    return `${formattedMinutes}:${formattedSeconds}`;
}


async function getSongs(folder) {
    currFolder = folder;
    let a = await fetch(`/${folder}/`)
    let response = await a.text();
    let div = document.createElement("div")
    div.innerHTML = response;
    let as = div.getElementsByTagName("a")
    songs = []
    for (let index = 0; index < as.length; index++) {
        const element = as[index];
        if (element.href.endsWith(".mp3")) {
            songs.push(element.href.split(`/${folder}/`)[1])
        }
    }
    // Show all the songs playlist //             
    let songUL = document.querySelector(".songlist").getElementsByTagName("ul")[0]
    songUL.innerHTML = ""
    for (const song of songs) {
        songUL.innerHTML = songUL.innerHTML + `<li><img class="invert" width="34" src="img/music.svg" alt="">
                            <div class="info">
                                <div>${song.replaceAll("%20", " ")}</div>
                                <div>Amartya</div>
                            </div>
                            <div class="playnow">
                                <span>Play Now</span>
                                <img class="invert" src="img/play.svg" alt="">
                            </div> </li>`;
    }
    //Attach an event lessener to each song //
    Array.from(document.querySelector(".songlist").getElementsByTagName("li")).forEach(e => {
        e.addEventListener("click", element => {
            // console.log(e.querySelector(".info").firstElementChild.innerHTML)
            playMusic(e.querySelector(".info").firstElementChild.innerHTML.trim())
        })
    })
    return songs
}

const playMusic = (track, pause = false) => {
    currentSong.src = `/${currFolder}/` + track;
    currentSong.addEventListener('loadeddata', () => {
        if (!pause) {
            currentSong.play();
            document.getElementById("play").src = "img/pause.svg";
        }
    }, { once: true });
    document.querySelector(".songinfo").innerHTML = decodeURI(track);
    document.querySelector(".songtime").innerHTML = "00:00 / 00:00";
};


async function displayAlbums() {
    let a = await fetch(`http://127.0.0.1:3000/songs/`)
    let response = await a.text();
    let div = document.createElement("div")
    div.innerHTML = response;
    let anchors = div.getElementsByTagName("a")
    let cardContainer = document.querySelector(".cardContainer")
    // console.log(anchors)
    let array = Array.from(anchors)
    for (let index = 0; index < array.length; index++) {
        const e = array[index];
        if (e.href.includes("/songs")) {
            let folder = (e.href.split("/").slice(-2)[0])
            // Get the meta data of the folder //
            let a = await fetch(`http://127.0.0.1:3000/songs/${folder}/info.json`)
            let response = await a.json();
            // console.log(response)
            cardContainer.innerHTML = cardContainer.innerHTML + `<div data-folder="${folder}" class="card">
                        <div class="play">
                            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"
                                fill="none">
                                <path fill-rule="evenodd" clip-rule="evenodd"
                                    d="M5.25 5.78987C5.25 4.42081 6.7512 3.58195 7.91717 4.29947L18.0091 10.5099C19.1196 11.1933 19.1196 12.8074 18.0091 13.4907L7.91717 19.7011C6.7512 20.4187 5.25 19.5798 5.25 18.2107V5.78987Z"
                                    fill="#141B34" />
                            </svg>
                        </div>
                        <img src="/songs/${folder}/cover.jpg" alt="">
                        <h2>${response.title}</h2>
                        <p>${response.description}</p>
                    </div>`
        }
    }
    // Load the playlist whenever card is clicked //
    Array.from(document.getElementsByClassName("card")).forEach(e => {
        e.addEventListener("click", async item => {
            // console.log(item.target, item.currentTarget.dataset)
            songs = await getSongs(`songs/${item.currentTarget.dataset.folder}`)
            playMusic(songs[0])
        })
    })
}

async function main() {
    // Get the list of all the songs //
    await getSongs("songs/ncs")
    // await getSongs("songs/cs")  // Load folder //
    playMusic(songs[0], true)
    // console.log("Songs loaded:", songs);
    // Display all the albums on the page //
    displayAlbums()
    //Attach an event lessener to previous, play, next //
    play.addEventListener("click", () => {
        if (currentSong.paused) {
            currentSong.play()
            play.src = "img/pause.svg"
        }
        else {
            currentSong.pause()
            play.src = "img/play.svg"
        }
    })
    // Listen for timeupdate event //
    currentSong.addEventListener("timeupdate", () => {
        // console.log(currentSong.currentTime, currentSong.duration);
        document.querySelector(".songtime").innerHTML = `${secondsToMinutesSeconds(currentSong.currentTime)} / ${secondsToMinutesSeconds(currentSong.duration)}`
        document.querySelector(".circle").style.left = (currentSong.currentTime / currentSong.duration) * 100 + "%";
    })
    // Add an event listener to seekbar
    document.querySelector(".seekbar").addEventListener("click", (e) => {
        let percent = (e.offsetX / e.target.getBoundingClientRect().width) * 100;
        document.querySelector(".circle").style.left = percent + "%";
        currentSong.currentTime = ((currentSong.duration) * percent) / 100
    })
    // Add an event listner for hamburger //
    document.querySelector(".hamburger").addEventListener("click", () => {
        document.querySelector(".left").style.left = "0"
    })
    // Add an event listner for close button //
    document.querySelector(".close").addEventListener("click", () => {
        document.querySelector(".left").style.left = "-120%"
    })
    // Add an event listner for previous and next..... //
    // Add an event listner for previous //
    previous.addEventListener("click", () => {
        currentSong.pause()
        console.log("Previous clicked")
        let index = songs.indexOf(currentSong.src.split("/").slice(-1)[0])
        if ((index - 1) >= 0) {
            playMusic(songs[index - 1])
        }
    })
    // Add an event listener to next
    next.addEventListener("click", () => {
        currentSong.pause()
        console.log("Next clicked")
        let index = songs.indexOf(currentSong.src.split("/").slice(-1)[0])
        if ((index + 1) < songs.length) {
            playMusic(songs[index + 1])
        }
    })
    // Add an event to volume //
    document.querySelector(".range").getElementsByTagName("input")[0].addEventListener("change", (e) => {
        console.log("setting volume to", e.target.value, "/ 100")
        currentSong.volume = parseInt(e.target.value) / 100
    })
    // Add event listner to mute the track //
    document.querySelector(".volume>img").addEventListener("click", e => {
        if (e.target.src.includes("volume.svg")) {
            e.target.src = e.target.src.replace("volume.svg", "mute.svg")
            currentSong.volume = 0;
            document.querySelector(".range").getElementsByTagName("input")[0].value = 0;
        }
        else {
            e.target.src = e.target.src.replace("mute.svg", "volume.svg")
            currentSong.volume = .10;
            document.querySelector(".range").getElementsByTagName("input")[0].value = 10;
        }
    })

}

main()
