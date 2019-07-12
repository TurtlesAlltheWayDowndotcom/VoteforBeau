<!DOCTYPE html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
body {font-family: Arial;}
h1 {
    color: white;
}body {background-color:#384855;}

/* Style the tab */
.tab {
    overflow: hidden;
    border: 1px solid #ccc;
    background-color: #f1f1f1;
}
}
.tabcontent {
    animation: fadeEffect 1s; /* Fading effect takes 2 second */
}

/* Go from zero to full opacity */
@keyframes fadeEffect {
    from {opacity: 0;}
    to {opacity: 1;}
}

/* Style the buttons inside the tab */
.tab button {
    background-color: inherit;
    float: left;
    border: none;
    outline: none;
    cursor: pointer;
    padding: 14px 16px;
    transition: 0.3s;
    font-size: 17px;
}

/* Change background color of buttons on hover */
.tab button:hover {
    background-color: #ddd;
}

/* Create an active/current tablink class */
.tab button.active {
    background-color: #ccc;
}

/* Style the tab content */
.tabcontent {
    display: none;
    background-color: #ffffff;
    padding: 6px 12px;
    border: 1px solid #ccc;
    border-top: none;
}
</style>
</head>
<body>

<h1>Beau for President</h1>


<div class="tab">
  <button class="tablinks" onclick="openCity(event, 'About')">About</button>
  <button class="tablinks" onclick="openCity(event, 'Platform')">Platform</button>
  <button class="tablinks" onclick="openCity(event, 'Contact')">Contact</button>
</div>

<div id="About" class="tabcontent">
  Born in rural Pennsylvannia in 2011, Beau had humble beginnings.She was wandering along a back country road where she was found chasing after her orange brother.
  Beau was caught but her brother was too quick and she never saw him again.  She was taken in and covered in fleas but happy to be somewhere warm.<br><p>
  Over time she became involved in community projects and helping out her fellow man.  Beau has organized countless fundraisers to stop declawing and the fur trade. 
  She never forgot her roots and how lucky she was to have a home with kibble and cable.
</div>

<div id="Platform" class="tabcontent">
<p>In order to form a more purrfect union
  <hr>
<ul>
 <li>Has caught the red dot twice</li>

 <li>Knock things off shelves</li>

 <li>Will keep rodent population in check</li>

 <li>Debate skills (fighting)</li>

 <li>Opponent is not a good boy</li>

 <li>Can stand at podium without scratching</li>

 <li>Smoked catnip in college but did not inhale</li>

 <li>Passionate about animal rights</li>

 <li>Street cat veteran</li>

 <li>Spayed so she cannot be involved in sex scandals</li>

 <li>Vote for Beau right meow!</li></ul></p> 
</div>

<div id="Contact" class="tabcontent">
   <a href="mailto:arc18370@hawkmail.hacc.edu" data-rel="external">Email</a><br />
</div>

<script>
function openCity(evt, cityName) {
    var i, tabcontent, tablinks;
    tabcontent = document.getElementsByClassName("tabcontent");
    for (i = 0; i < tabcontent.length; i++) {
        tabcontent[i].style.display = "none";
    }
    tablinks = document.getElementsByClassName("tablinks");
    for (i = 0; i < tablinks.length; i++) {
        tablinks[i].className = tablinks[i].className.replace(" active", "");
    }
    document.getElementById(cityName).style.display = "block";
    evt.currentTarget.className += " active";
}
</script>
     
</body>
</html> 

