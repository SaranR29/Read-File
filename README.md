# readfile
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>HTML Course</title>
    <link rel="icon" href="images/RightSkill.png" type="images/x-icon" />
    <script defer src="./quizz.js"></script>
    <style>
      body {
        margin: 0px;
        background: linear-gradient(
          to right,
          rgba(40, 157, 240, 0.944),
          hsl(166, 97%, 73%),
          rgba(40, 157, 240, 0.944)
        );
      }
      .navv {
        display: block;
        background-color: #2453ef;
      }

      .home2 {
        display: inline-flex;
        width: 2%;
        margin-right: 10px;
      }
      .point2 {
        display: inline-flex;
        width: 2%;
        border-radius: 100%;
      }
      .user2 {
        display: inline-flex;
        width: 2%;
        border-radius: 100%;
        float: right;
        margin-right: 10px;
      }
      .head1 {
        font-family: Merriweather;
        display: block;
        font-weight: 1000;
        font-size: 3rem;
        text-align: center;
      }
      .para1 {
        font-family: Oswald;
        display: flex;
        font-weight: 900;
        color: black;
        font-size: 1.5rem;
        margin-left: 150px;
      }
      .img1 {
        display: flex;
        position: absolute;
        width: 30%;
        right: 35%;
      }
      .img2 {
        display: flex;
        margin-top: 300px;
        position: absolute;
        width: 30%;
        right: 35%;
      }
      .vid1 {
        margin-left: 150px;
      }
      .next1 {
        display: flex;
        min-width: 70px;
        background-color: #eae31a;
        border-radius: 10%;
        box-shadow: 2px 2px 2px rgb(1, 40, 91);
        border-color: #011949;
        padding: 5px 12px;
        font-family: roboto;
        font-weight: 900;
        font-size: 20px;
        transition: color 0.2s;
        transition: background-color 0.1s;
        margin-top: 730px;
        margin-left: 710px;
      }
      .next1:hover {
        background-color: #f7f4a2;
        color: rgb(0, 0, 0);
        box-shadow: 2px 4px 2px rgba(2, 17, 61, 0.618);
        cursor: pointer;
      }
      .htmlt1 {
        margin-left: 430px;
      }

      .wrapper {
        display: flex;
        justify-content: center;
        align-items: center;
        width: 100vw;
        height: 100vh;
      }

      .quiz {
        display: grid;
        grid-template-rows: 60px auto;
        width: 600px;
        height: 500px;
        border-radius: 50px;
      }

      .quiz_header {
        display: flex;
        justify-content: space-between;
        border-bottom-left-radius: 3px;
        border-bottom-right-radius: 3px;
        background-color: #fff;
        box-shadow: 0px 2px 5px 1px rgba(0, 0, 0, 0.1);
        z-index: 1;
      }

      .quiz_user {
        display: flex;
        align-items: center;
        height: 100%;
        padding-left: 30px;
      }

      .quiz_body {
        padding: 20px 30px;
        background-color: skyblue;
      }

      .option_group {
        list-style-type: none;
        margin: 30px 0;
      }

      .option {
        display: block;
        width: 300px;
        background-color: #fff;
        margin-bottom: 20px;
        padding: 15px 20px;
        border-radius: 50px;
        border: 2px solid transparent;
        transition: 0.4s all;
      }

      .option:hover {
        cursor: pointer;
        border: 2px solid #341f97;
        color: #341f97;
      }

      .option.active {
        background-color: #341f97;
        color: #fff;
      }

      .btn-next {
        border: none;
        padding: 15px 35px;
        background-color: #341f97;
        color: #fff;
        border-radius: 50px;
        transition: 0.4s all;
        margin-left: 40px;
      }
      .btn-next2 {
        border: none;
        padding: 15px 35px;
        background-color: #341f97;
        color: #fff;
        border-radius: 50px;
        transition: 0.4s all;
        margin-left: 20px;
      }

      .btn-next:hover {
        cursor: pointer;
        background-color: greenyellow;
        color: #000;
      }
      .btn-next2:hover {
        cursor: pointer;
        background-color: greenyellow;
        color: #000;
      }

      .award_icon {
        display: block;
        font-size: 300px;
        color: #fff;
      }

      .username,
      .userpoints {
        color: #fff;
        text-align: center;
        margin-top: 15px;
      }

      .border {
        height: 500px;
        width: 500px;
        display: block;
        justify-content: center;
        margin: 0px 400px;
        border-radius: 10px;
        top: 100px;
        border-color: transparent;
      }
      .quizz1 {
        visibility: hidden;
      }
    </style>
  </head>
  <body>
    <div class="navv">
      <a href="courses.html"><img src="images/back.png" class="home2" /></a>
      <a href="score.html"><img src="images/points.png" class="point2" /></a>
      <a href="profile.html"><img src="images/user.png" class="user2" /></a>
    </div>
    <div id="test1">
      <h1 class="head1">HTML Basics Course:</h1>
    </div>
    <div id="test2">
      <p class="para1">
        Before the start of this course, it is recommended that you follow the
        instructions given below to get off to a better start.
      </p>
      <p class="para1">
        1.Download Vscode from the store.<br />
        2.Install the extension called "Live server".<br />
        You can follow the images below:
      </p>
      <img class="img1" src="images/vscode1.png" alt />
      <img class="img2" src="images/vscode2.png" alt />
      <button onclick="htmlpg2()" class="next1">Next</button>
    </div>
    <div class="quizz1" id="q1">
      <div class="wrapper">
        <div class="quiz">
          <div class="quiz_header">
            <div class="quiz_user">
              <h4>WELCOME ! <span class="name"></span></h4>
            </div>
          </div>

          <div class="quiz_body">
            <div id="questions">
              <!-- <ul class="option_group">
              <li class="option">option 1</li>
              <li class="option">option 2</li>
              <li class="option">option 3</li>
              <li class="option">option 4</li>
              </ul> -->
            </div>

            <button class="btn-next" onclick="next()">Next Question</button>
            <button class="btn-next2" onclick="show1()">Show Points</button>
          </div>
        </div>
      </div>
    </div>
  </body>
</html>
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>HTML Course</title>
    <link rel="icon" href="images/RightSkill.png" type="images/x-icon" />
    <script defer src="./quizz.js"></script>
    <style>
      body {
        margin: 0px;
        background: linear-gradient(
          to right,
          rgba(40, 157, 240, 0.944),
          hsl(166, 97%, 73%),
          rgba(40, 157, 240, 0.944)
        );
      }
      .navv {
        display: block;
        background-color: #2453ef;
      }

      .home2 {
        display: inline-flex;
        width: 2%;
        margin-right: 10px;
      }
      .point2 {
        display: inline-flex;
        width: 2%;
        border-radius: 100%;
      }
      .user2 {
        display: inline-flex;
        width: 2%;
        border-radius: 100%;
        float: right;
        margin-right: 10px;
      }
      .head1 {
        font-family: Merriweather;
        display: block;
        font-weight: 1000;
        font-size: 3rem;
        text-align: center;
      }
      .para1 {
        font-family: Oswald;
        display: flex;
        font-weight: 900;
        color: black;
        font-size: 1.5rem;
        margin-left: 150px;
      }
      .img1 {
        display: flex;
        position: absolute;
        width: 30%;
        right: 35%;
      }
      .img2 {
        display: flex;
        margin-top: 300px;
        position: absolute;
        width: 30%;
        right: 35%;
      }
      .vid1 {
        margin-left: 150px;
      }
      .next1 {
        display: flex;
        min-width: 70px;
        background-color: #eae31a;
        border-radius: 10%;
        box-shadow: 2px 2px 2px rgb(1, 40, 91);
        border-color: #011949;
        padding: 5px 12px;
        font-family: roboto;
        font-weight: 900;
        font-size: 20px;
        transition: color 0.2s;
        transition: background-color 0.1s;
        margin-top: 730px;
        margin-left: 710px;
      }
      .next1:hover {
        background-color: #f7f4a2;
        color: rgb(0, 0, 0);
        box-shadow: 2px 4px 2px rgba(2, 17, 61, 0.618);
        cursor: pointer;
      }
      .htmlt1 {
        margin-left: 430px;
      }

      .wrapper {
        display: flex;
        justify-content: center;
        align-items: center;
        width: 100vw;
        height: 100vh;
      }

      .quiz {
        display: grid;
        grid-template-rows: 60px auto;
        width: 600px;
        height: 500px;
        border-radius: 50px;
      }

      .quiz_header {
        display: flex;
        justify-content: space-between;
        border-bottom-left-radius: 3px;
        border-bottom-right-radius: 3px;
        background-color: #fff;
        box-shadow: 0px 2px 5px 1px rgba(0, 0, 0, 0.1);
        z-index: 1;
      }

      .quiz_user {
        display: flex;
        align-items: center;
        height: 100%;
        padding-left: 30px;
      }

      .quiz_body {
        padding: 20px 30px;
        background-color: skyblue;
      }

      .option_group {
        list-style-type: none;
        margin: 30px 0;
      }

      .option {
        display: block;
        width: 300px;
        background-color: #fff;
        margin-bottom: 20px;
        padding: 15px 20px;
        border-radius: 50px;
        border: 2px solid transparent;
        transition: 0.4s all;
      }

      .option:hover {
        cursor: pointer;
        border: 2px solid #341f97;
        color: #341f97;
      }

      .option.active {
        background-color: #341f97;
        color: #fff;
      }

      .btn-next {
        border: none;
        padding: 15px 35px;
        background-color: #341f97;
        color: #fff;
        border-radius: 50px;
        transition: 0.4s all;
        margin-left: 40px;
      }
      .btn-next2 {
        border: none;
        padding: 15px 35px;
        background-color: #341f97;
        color: #fff;
        border-radius: 50px;
        transition: 0.4s all;
        margin-left: 20px;
      }

      .btn-next:hover {
        cursor: pointer;
        background-color: greenyellow;
        color: #000;
      }
      .btn-next2:hover {
        cursor: pointer;
        background-color: greenyellow;
        color: #000;
      }

      .award_icon {
        display: block;
        font-size: 300px;
        color: #fff;
      }

      .username,
      .userpoints {
        color: #fff;
        text-align: center;
        margin-top: 15px;
      }

      .border {
        height: 500px;
        width: 500px;
        display: block;
        justify-content: center;
        margin: 0px 400px;
        border-radius: 10px;
        top: 100px;
        border-color: transparent;
      }
      .quizz1 {
        visibility: hidden;
      }
    </style>
  </head>
  <body>
    <div class="navv">
      <a href="courses.html"><img src="images/back.png" class="home2" /></a>
      <a href="score.html"><img src="images/points.png" class="point2" /></a>
      <a href="profile.html"><img src="images/user.png" class="user2" /></a>
    </div>
    <div id="test1">
      <h1 class="head1">HTML Basics Course:</h1>
    </div>
    <div id="test2">
      <p class="para1">
        Before the start of this course, it is recommended that you follow the
        instructions given below to get off to a better start.
      </p>
      <p class="para1">
        1.Download Vscode from the store.<br />
        2.Install the extension called "Live server".<br />
        You can follow the images below:
      </p>
      <img class="img1" src="images/vscode1.png" alt />
      <img class="img2" src="images/vscode2.png" alt />
      <button onclick="htmlpg2()" class="next1">Next</button>
    </div>
    <div class="quizz1" id="q1">
      <div class="wrapper">
        <div class="quiz">
          <div class="quiz_header">
            <div class="quiz_user">
              <h4>WELCOME ! <span class="name"></span></h4>
            </div>
          </div>

          <div class="quiz_body">
            <div id="questions">
              <!-- <ul class="option_group">
              <li class="option">option 1</li>
              <li class="option">option 2</li>
              <li class="option">option 3</li>
              <li class="option">option 4</li>
              </ul> -->
            </div>

            <button class="btn-next" onclick="next()">Next Question</button>
            <button class="btn-next2" onclick="show1()">Show Points</button>
          </div>
        </div>
      </div>
    </div>
  </body>
</html>

