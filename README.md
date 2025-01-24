<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Be My Valentine</title>
    <style>
        body {
            text-align: center;
            margin-top: 30px;
            font-family: 'Courier';
			background-color:#FFF5E4;
            color: #FF9494;
        }
        #valentineQuestion {
            font-size: 50px;
            margin-bottom: 10px;
        }
        .answerButton {
            padding: 10px 20px;
            font-size: 18px;
            cursor: pointer;
            margin: 10px;
            font-family: 'courier';
            margin-bottom: 20px;
            background-color:#FFE3E1;
            color: #e67373;
            border-radius: 12px;
            border: 2px solid #FFE3E1;
        }
    </style>
</head>
<body>
    <div id="valentineQuestion"><b>Will you be my valentine?</b></div>
    <button class="answerButton" onclick="location.href='thankyou.html'">Yes</button>
    <button class="answerButton" id="noButton">No</button>
    <button class="answerButton" id="noButton">I no no wanna o(╥﹏╥)o</button>
    <br>
    <img src ='cat.gif' alt = 'cat asking question' class="responsive">

	<script>
        document.getElementById('noButton').addEventListener('click', function() {
            var yesButton = document.querySelector('button[onclick*="thankyou.html"]');
            var currentFontSize = parseInt(window.getComputedStyle(yesButton).fontSize);
            yesButton.style.fontSize = (currentFontSize + 10) + 'px'; // Increase font size by 5px
        });
    </script>
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>Document</title>
	<style>
		body {
			text-align: center;
            margin-top: 30px;
            font-family: 'Courier';
            background-color:#FFF5E4;
            color: #FF9494;
		}
		#activityquestion {
			font-size: 50px;
            margin-bottom: 30px;
		}
.activity-item {
            display: inline-block;
            margin: 10px;
            vertical-align: top;
			color: #FF9494;
        }
        .activity-item img {
            width: 220px; 
            height: auto;
			padding: 10px;
        }
        .activity-item label {
            display: block;
        }
	</style>
</head>
<body>
	<div id="activityquestion"><u><b>What are we doing after?</b></u>
	<div id="activityquestion"><b>What are we doing after?</b>
	</div>
	<div class = "activities-selection">
		<div class="activity-item">
			<img src="activities/aquarium.jpeg" alt ="aquarium">
			<label><input type="checkbox" name="activities" value ="aquarium">aquarium</label>
		</div>
<div class="activity-item">
			<img src="activities/arcade.jpeg" alt ="arcade">
			<label><input type="checkbox" name="activities" value ="arcade">arcade</label>
		</div>
		<div class="activity-item">
			<img src="activities/cinema.jpeg" alt ="cinema">
			<label><input type="checkbox" name="activities" value ="cinema">cinema</label>
		</div>
		<div class="activity-item">
			<img src="activities/keramika.jpeg" alt ="ceramics">
   <label><input type="checkbox" name="activities" value ="ceramics">ceramics</label>
		</div>
		<div class="activity-item">
			<img src="activities/kunsthalle.jpeg" alt ="kunsthalle">
			<label><input type="checkbox" name="activities" value ="kunsthalle">exhibition</label>
		</div>
		<div class="activity-item">
			<img src="activities/park.jpeg" alt ="park.jpeg">
			<label><input type="checkbox" name="activities" value ="park.jpeg">park</label>
		</div>
	</div>
	<button onclick="location.href='lastpage.html'">Last page</button>
 </body>
</html>
