<h1 align="center">Hi 👋, I'm Ayan ahmed</h1>
<h3 align="center">A  student and passionate frontend developer </h3>
<img  align="left end" width="400" src="https://cdn.dribbble.com/users/1162077/screenshots/3848914/programmer.gif" alt="coding">
<p align="left"> <img src="https://komarev.com/ghpvc/?username=crypton0305&label=Profile%20views&color=0e75b6&style=flat" alt="crypton0305" /> </p>


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        /* HOLD THE ASTRONAUT */

.card {
  position: relative;
  width: 19em;
  height: 25em;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  background-color: #171717;
  color: white;
  font-family: Montserrat;
  font-weight: bold;
  padding: 1em 2em 1em 1em;
  border-radius: 20px;
  overflow: hidden;
  z-index: 1;
  row-gap: 1em;
}
.card img {
  width: 12em;
  margin-right: 1em;
  animation: move 10s ease-in-out infinite;
  z-index: 5;
}
.image:hover {
  cursor: -webkit-grab;
  cursor: grab;
}

.icons svg {
  width: 20px;
  height: 20px;
}

.card::before {
  content: "";
  position: absolute;
  width: 100%;
  height: 100%;
  inset: -3px;
  border-radius: 10px;
  background: radial-gradient(#858585, transparent, transparent);
  transform: translate(-5px, 250px);
  transition: 0.4s ease-in-out;
  z-index: -1;
}
.card:hover::before {
  width: 150%;
  height: 100%;
  margin-left: -4.25em;
}
.card::after {
  content: "";
  position: absolute;
  inset: 2px;
  border-radius: 20px;
  background: rgb(23, 23, 23, 0.7);
  transition: all 0.4s ease-in-out;
  z-index: -1;
}

.heading {
  z-index: 2;
  transition: 0.4s ease-in-out;
}
.card:hover .heading {
  letter-spacing: 0.025em;
}

.heading::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 2px;
  height: 2px;
  border-radius: 50%;
  opacity: 1;
  box-shadow: 220px 118px #fff, 280px 176px #fff, 40px 50px #fff,
    60px 180px #fff, 120px 130px #fff, 180px 176px #fff, 220px 290px #fff,
    520px 250px #fff, 400px 220px #fff, 50px 350px #fff, 10px 230px #fff;
  z-index: -1;
  transition: 1s ease;
  animation: 1s glowing-stars linear alternate infinite;
  animation-delay: 0s;
}
.icons::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 2px;
  height: 2px;
  border-radius: 50%;
  opacity: 1;
  box-shadow: 140px 20px #fff, 425px 20px #fff, 70px 120px #fff, 20px 130px #fff,
    110px 80px #fff, 280px 80px #fff, 250px 350px #fff, 280px 230px #fff,
    220px 190px #fff, 450px 100px #fff, 380px 80px #fff, 520px 50px #fff;
  z-index: -1;
  transition: 1.5s ease;
  animation: 1s glowing-stars linear alternate infinite;
  animation-delay: 0.4s;
}
.icons::after {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 2px;
  height: 2px;
  border-radius: 50%;
  opacity: 1;
  box-shadow: 490px 330px #fff, 420px 300px #fff, 320px 280px #fff,
    380px 350px #fff, 546px 170px #fff, 420px 180px #fff, 370px 150px #fff,
    200px 250px #fff, 80px 20px #fff, 190px 50px #fff, 270px 20px #fff,
    120px 230px #fff, 350px -1px #fff, 150px 369px #fff;
  z-index: -1;
  transition: 2s ease;
  animation: 1s glowing-stars linear alternate infinite;
  animation-delay: 0.8s;
}
.card:hover .heading::before,
.card:hover .icons::before,
.card:hover .icons::after {
  filter: blur(3px);
}

.image:active {
  cursor: -webkit-grabbing;
  cursor: grabbing;
}
.image:active + .heading::before {
  box-shadow: 240px 20px #9b40fc, 240px 25px #9b40fc, 240px 30px #9b40fc,
    240px 35px #9b40fc, 240px 40px #9b40fc, 242px 45px #9b40fc,
    246px 48px #9b40fc, 251px 49px #9b40fc, 256px 48px #9b40fc,
    260px 45px #9b40fc, 262px 40px #9b40fc;
  animation: none;
  filter: blur(0);
  border-radius: 2px;
  width: 0.45em;
  height: 0.45em;
  scale: 0.65;
  transform: translateX(9em) translateY(1em);
}
.image:active ~ .icons::before {
  box-shadow: 262px 35px #9b40fc, 262px 30px #9b40fc, 262px 25px #9b40fc,
    262px 20px #9b40fc, 275px 20px #9b40fc, 275px 24px #9b40fc,
    275px 28px #9b40fc, 275px 32px #9b40fc, 275px 36px #9b40fc,
    275px 40px #9b40fc, 275px 44px #9b40fc, 275px 48px #9b40fc;
  animation: none;
  filter: blur(0);
  border-radius: 2px;
  width: 0.45em;
  height: 0.45em;
  scale: 0.65;
  transform: translateX(9em) translateY(1em);
}
.image:active ~ .icons::after {
  box-shadow: 238px 60px #9b40fc, 242px 60px #9b40fc, 246px 60px #9b40fc,
    250px 60px #9b40fc, 254px 60px #9b40fc, 258px 60px #9b40fc,
    262px 60px #9b40fc, 266px 60px #9b40fc, 270px 60px #9b40fc,
    274px 60px #9b40fc, 278px 60px #9b40fc, 282px 60px #9b40fc,
    234px 60px #9b40fc, 234px 60px #9b40fc;
  animation: none;
  filter: blur(0);
  border-radius: 2px;
  width: 0.45em;
  height: 0.45em;
  scale: 0.65;
  transform: translateX(9em) translateY(1.25em);
}

.heading::after {
  content: "";
  top: -8.5%;
  left: -8.5%;
  position: absolute;
  width: 7.5em;
  height: 7.5em;
  border: none;
  outline: none;
  border-radius: 50%;
  background: #f9f9fb;
  box-shadow: 0px 0px 100px rgba(193, 119, 241, 0.8),
    0px 0px 100px rgba(135, 42, 211, 0.8), inset #9b40fc 0px 0px 40px -12px;
  transition: 0.4s ease-in-out;
  z-index: -1;
}
.card:hover .heading::after {
  box-shadow: 0px 0px 200px rgba(193, 119, 241, 1),
    0px 0px 200px rgba(135, 42, 211, 1), inset #9b40fc 0px 0px 40px -12px;
}

.icons {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: row;
  column-gap: 1em;
  z-index: 1;
}

.instagram,
.x,
.discord {
  position: relative;
  transition: 0.4s ease-in-out;
}
.instagram:after,
.x:after,
.discord:after {
  content: "";
  position: absolute;
  width: 0.5em;
  height: 0.5em;
  left: 0;
  background-color: white;
  box-shadow: 0px 0px 10px rgba(233, 233, 233, 0.5),
    0px 0px 10px rgba(192, 192, 192, 0.5);
  border-radius: 50%;
  z-index: -1;
  transition: 0.3s ease-in-out;
}
.instagram svg path,
.x svg path,
.discord svg path {
  stroke: #808080;
  transition: 0.4s ease-in-out;
}
.instagram:hover svg path {
  stroke: #cc39a4;
}
.x:hover svg path {
  stroke: black;
}
.discord:hover svg path {
  stroke: #8c9eff;
}
.instagram svg,
.x svg,
.discord svg {
  transition: 0.3s ease-in-out;
}
.instagram:hover svg {
  scale: 1.4;
}
.x:hover svg,
.discord:hover svg {
  scale: 1.25;
}
.instagram:hover:after,
.x:hover:after,
.discord:hover:after {
  scale: 4;
  transform: translateX(0.09em) translateY(0.09em);
}

.instagram::before {
  content: "";
  position: absolute;
  top: -700%;
  left: 1050%;
  rotate: -45deg;
  width: 5em;
  height: 1px;
  background: linear-gradient(90deg, #ffffff, transparent);
  animation: 4s shootingStar ease-in-out infinite;
  transition: 1s ease;
  animation-delay: 1s;
}
.x::before {
  content: "";
  position: absolute;
  top: -1300%;
  left: 850%;
  rotate: -45deg;
  width: 5em;
  height: 1px;
  background: linear-gradient(90deg, #ffffff, transparent);
  animation: 4s shootingStar ease-in-out infinite;
  animation-delay: 3s;
}
.discord::before {
  content: "";
  position: absolute;
  top: -2100%;
  left: 850%;
  rotate: -45deg;
  width: 5em;
  height: 1px;
  background: linear-gradient(90deg, #ffffff, transparent);
  animation: 4s shootingStar ease-in-out infinite;
  animation-delay: 5s;
}
.card:hover .instagram::before,
.card:hover .x::before,
.card:hover .discord::before {
  filter: blur(3px);
}
.image:active ~ .icons .instagram::before,
.image:active ~ .icons .x::before,
.image:active ~ .icons .discord::before {
  animation: none;
  opacity: 0;
}

@keyframes shootingStar {
  0% {
    transform: translateX(0) translateY(0);
    opacity: 1;
  }
  50% {
    transform: translateX(-55em) translateY(0);
    opacity: 1;
  }
  70% {
    transform: translateX(-70em) translateY(0);
    opacity: 0;
  }
  100% {
    transform: translateX(0) translateY(0);
    opacity: 0;
  }
}

@keyframes move {
  0% {
    transform: translateX(0em) translateY(0em);
  }
  25% {
    transform: translateY(-1em) translateX(-1em);
    rotate: -10deg;
  }
  50% {
    transform: translateY(1em) translateX(-1em);
  }
  75% {
    transform: translateY(-1.25em) translateX(1em);
    rotate: 10deg;
  }
  100% {
    transform: translateX(0em) translateY(0em);
  }
}

@keyframes glowing-stars {
  0% {
    opacity: 0;
  }

  50% {
    opacity: 1;
  }

  100% {
    opacity: 0;
  }
}

    </style>
</head>
<body>
    <div class="card">
        <img
          src="https://uiverse.io/build/_assets/astronaut-WTFWARES.png"
          alt=""
          class="image"
        />
        <div class="heading">We're on Social Media</div>
        <div class="icons">
          <a href="https://www.instagram.com/uiverse.io/" class="instagram">
            <svg
              width="24"
              height="25"
              viewBox="0 0 24 25"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M17.0459 7.5H17.0559M3.0459 12.5C3.0459 9.986 3.0459 8.73 3.3999 7.72C3.71249 6.82657 4.22237 6.01507 4.89167 5.34577C5.56096 4.67647 6.37247 4.16659 7.2659 3.854C8.2759 3.5 9.5329 3.5 12.0459 3.5C14.5599 3.5 15.8159 3.5 16.8269 3.854C17.7202 4.16648 18.5317 4.67621 19.201 5.34533C19.8702 6.01445 20.3802 6.82576 20.6929 7.719C21.0459 8.729 21.0459 9.986 21.0459 12.5C21.0459 15.014 21.0459 16.27 20.6929 17.28C20.3803 18.1734 19.8704 18.9849 19.2011 19.6542C18.5318 20.3235 17.7203 20.8334 16.8269 21.146C15.8169 21.5 14.5599 21.5 12.0469 21.5C9.5329 21.5 8.2759 21.5 7.2659 21.146C6.37268 20.8336 5.56131 20.324 4.89202 19.6551C4.22274 18.9862 3.71274 18.1751 3.3999 17.282C3.0459 16.272 3.0459 15.015 3.0459 12.501V12.5ZM15.8239 11.94C15.9033 12.4387 15.8829 12.9481 15.7641 13.4389C15.6453 13.9296 15.4304 14.392 15.1317 14.7991C14.833 15.2063 14.4566 15.5501 14.0242 15.8108C13.5917 16.0715 13.1119 16.2439 12.6124 16.318C12.1129 16.392 11.6037 16.3663 11.1142 16.2422C10.6248 16.1182 10.1648 15.8983 9.76082 15.5953C9.35688 15.2923 9.01703 14.9123 8.76095 14.4771C8.50486 14.0419 8.33762 13.5602 8.2689 13.06C8.13201 12.0635 8.39375 11.0533 8.99727 10.2487C9.6008 9.44407 10.4974 8.91002 11.4923 8.76252C12.4873 8.61503 13.5002 8.86599 14.3112 9.46091C15.1222 10.0558 15.6658 10.9467 15.8239 11.94Z"
                stroke="currentColor"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
            </svg>
          </a>
          <a href="https://twitter.com/uiverse_io" class="x">
            <svg
              width="24"
              height="24"
              viewBox="0 0 24 24"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M19.8003 3L13.5823 10.105L19.9583 19.106C20.3923 19.719 20.6083 20.025 20.5983 20.28C20.594 20.3896 20.5657 20.4969 20.5154 20.5943C20.4651 20.6917 20.3941 20.777 20.3073 20.844C20.1043 21 19.7293 21 18.9793 21H17.2903C16.8353 21 16.6083 21 16.4003 20.939C16.2168 20.8847 16.0454 20.7957 15.8953 20.677C15.7253 20.544 15.5943 20.358 15.3313 19.987L10.6813 13.421L4.64033 4.894C4.20733 4.281 3.99033 3.975 4.00033 3.72C4.00478 3.61035 4.03323 3.50302 4.08368 3.40557C4.13414 3.30812 4.20536 3.22292 4.29233 3.156C4.49433 3 4.87033 3 5.62033 3H7.30833C7.76333 3 7.99033 3 8.19733 3.061C8.38119 3.1152 8.55295 3.20414 8.70333 3.323C8.87333 3.457 9.00433 3.642 9.26733 4.013L13.5833 10.105M4.05033 21L10.6823 13.421"
                stroke="currentColor"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
            </svg>
          </a>
          <a href="https://discord.gg/KD8ba2uUpT" class="discord">
            <svg
              width="25"
              height="25"
              viewBox="0 0 25 25"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M11.5989 6.5003H14.2919C14.3851 6.5003 14.4764 6.47427 14.5555 6.42515C14.6347 6.37603 14.6985 6.30577 14.7399 6.2223L15.4179 4.8543C15.4664 4.75358 15.5488 4.67313 15.6506 4.62706C15.7524 4.58098 15.8673 4.57222 15.9749 4.6023C16.6309 4.7903 18.0049 5.2433 19.1029 6.0003C22.9669 8.8973 22.6069 15.3903 22.5779 16.7603C22.5765 16.8444 22.5541 16.9269 22.5129 17.0003C20.5299 20.5003 17.0899 20.5003 17.0899 20.5003L15.9239 18.0743M15.9239 18.0743C16.4479 17.9163 17.0029 17.7253 17.6029 17.5003M15.9239 18.0743C13.4799 18.8093 11.7219 18.8083 9.27791 18.0733M13.5989 6.5003H10.9109C10.8179 6.50039 10.7266 6.47451 10.6475 6.42557C10.5683 6.37664 10.5044 6.30659 10.4629 6.2233L9.77991 4.8533C9.73146 4.75279 9.64925 4.6725 9.54762 4.62644C9.446 4.58038 9.33142 4.57148 9.22391 4.6013C8.56891 4.7893 7.19291 5.2433 6.09391 6.0003C2.23091 8.8973 2.59091 15.3903 2.61991 16.7603C2.62132 16.8445 2.64366 16.9269 2.68491 17.0003C4.66791 20.5003 8.10791 20.5003 8.10791 20.5003L9.27791 18.0733M9.27791 18.0733C8.75491 17.9163 8.19891 17.7253 7.59891 17.5003M10.6009 12.5003C10.6009 12.7655 10.4956 13.0199 10.308 13.2074C10.1205 13.3949 9.86612 13.5003 9.60091 13.5003C9.33569 13.5003 9.08134 13.3949 8.8938 13.2074C8.70626 13.0199 8.60091 12.7655 8.60091 12.5003C8.60091 12.2351 8.70626 11.9807 8.8938 11.7932C9.08134 11.6057 9.33569 11.5003 9.60091 11.5003C9.86612 11.5003 10.1205 11.6057 10.308 11.7932C10.4956 11.9807 10.6009 12.2351 10.6009 12.5003ZM16.6029 12.5003C16.6029 12.7655 16.4976 13.0199 16.31 13.2074C16.1225 13.3949 15.8681 13.5003 15.6029 13.5003C15.3377 13.5003 15.0833 13.3949 14.8958 13.2074C14.7083 13.0199 14.6029 12.7655 14.6029 12.5003C14.6029 12.2351 14.7083 11.9807 14.8958 11.7932C15.0833 11.6057 15.3377 11.5003 15.6029 11.5003C15.8681 11.5003 16.1225 11.6057 16.31 11.7932C16.4976 11.9807 16.6029 12.2351 16.6029 12.5003Z"
                stroke="currentColor"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
              ></path>
            </svg>
          </a>
        </div>
      </div>
      
</body>
</html>

<h3 align="left">Languages and Tools:</h3>
<p align="left"> <a href="https://www.w3schools.com/css/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original-wordmark.svg" alt="css3" width="40" height="40"/> </a> <a href="https://www.w3.org/html/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original-wordmark.svg" alt="html5" width="40" height="40"/> </a> <a href="https://www.java.com" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original.svg" alt="java" width="40" height="40"/> </a> <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"/> </a> <a href="https://www.mysql.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg" alt="mysql" width="40" height="40"/> </a> <a href="https://www.python.org" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="python" width="40" height="40"/> </a> <a href="https://reactjs.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original-wordmark.svg" alt="react" width="40" height="40"/> </a> <a href="https://www.typescriptlang.org/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/typescript/typescript-original.svg" alt="typescript" width="40" height="40"/> </a> </p>

<p><img align="left" src="https://github-readme-stats.vercel.app/api/top-langs?username=crypton0305&show_icons=true&locale=en&layout=compact" alt="crypton0305" /></p>

<p>&nbsp;<img align="left center" src="https://github-readme-stats.vercel.app/api?username=crypton0305&show_icons=true&locale=en" alt="crypton0305" /></p>

<p><img align="center" src="https://github-readme-streak-stats.herokuapp.com/?user=crypton0305&" alt="crypton0305" /></p>
